# Patuh

A Claude Code skill that checks Malaysian government websites against **Pekeliling Pendigitalan Perkhidmatan Awam Bilangan 1 Tahun 2025**, JDN's circular on portal/laman web management.

Claude skill yang semak laman web sektor awam Malaysia ikut **Pekeliling Pendigitalan Perkhidmatan Awam Bilangan 1 Tahun 2025** keluaran Jabatan Digital Negara, pekeliling rasmi pengurusan portal/laman web agensi kerajaan.

## What It Does

Three modes, one source of truth:

- **Build**: walks a team through every mandatory requirement before launching a new agency portal.
- **Audit**: checks an existing `gov.my` site and produces a structured pass/fail report with the top fixes ranked by priority.
- **Rasionalisasi**: classifies multiple agency portals (keep / close / consolidate / exempt) and steps through the JDN approval flow.

Every requirement is tagged:

- ✅ **[M] Mandatory**: the Pekeliling's *hendaklah / mesti / mandatori*. Non-negotiable.
- 💡 **[R] Recommended**: *digalakkan / disarankan / boleh*. Good practice, but **never flagged as a compliance failure**.

If the site isn't on a `gov.my` domain, the skill short-circuits the audit and reports that as the single finding. Nothing else matters until the domain is correct.

## Why I Built This

I got tired of seeing PKPA 2/2015 cited in compliance reports.

Pekeliling 1/2025 dropped in August 2025 and quietly replaced **six** older circulars. PKPA 2/2015 was the big one. But most agency teams, vendors, and even some auditors are still working from the old reference. They never read past the cover letter, or they read it once and forgot the details by the time they had to build or audit something.

It's a 68-page document in classical pekeliling-Malay. Nobody wants to re-read 68 pages every time they check a site. So they don't. They cite the old circular, miss the new requirements, ship anyway.

The other thing that kept bugging me: auditors flagging *digalakkan* items as compliance failures. The Pekeliling is precise. *Hendaklah* means mandatori, *digalakkan* means good practice. Conflating the two is the fastest way to get a compliance report ignored by the people who have to act on it.

So I built Patuh:
- **30-second audits**: point it at a `gov.my` site, get a prioritised pass/fail report
- **[M] vs [R] tagging**: mandatori vs digalakkan, never conflated
- **Three modes**: Build for new portals, Audit for existing sites, Rasionalisasi for portal-portfolio decisions
- **Hard-fail on non-`gov.my`**: if the domain is wrong, nothing else matters yet

## Who This Is For

- Public-sector portal teams across PAP, PAN, BBP, BBN, and PBT
- Vendors and ICT contractors delivering `gov.my` sites
- Internal auditors and JDN compliance officers
- Anyone evaluating a Malaysian government website against the current circular

## Installation

### Claude Code

Clone directly into Claude Code's skills directory:

```
mkdir -p ~/.claude/skills
git clone https://github.com/abualif120/patuh.git ~/.claude/skills/patuh
```

### OpenCode

Clone directly into OpenCode's skills directory:

```
mkdir -p ~/.config/opencode/skills
git clone https://github.com/abualif120/patuh.git ~/.config/opencode/skills/patuh
```

> **Note:** OpenCode also scans `~/.claude/skills/` for compatibility, so a single clone into `~/.claude/skills/patuh/` works for both tools.

## Usage

Invoke directly:

```
/patuh
```

…or just describe the task and let the skill auto-trigger:

- **Build:** *"I'm building the new website for Jabatan X. Walk me through every mandatory item before launch."*
- **Audit:** *"Audit https://www.<agency>.gov.my and give me the top 5 compliance fixes."*
- **Rasionalisasi:** *"Kami ada 4 portal di jabatan. Klasifikasi setiap satu dan draf kertas kelulusan."*

The skill responds in the language the user asks in, Bahasa Melayu or English.

## Source of Truth

**Pekeliling Pendigitalan Perkhidmatan Awam Bilangan 1 Tahun 2025**
*Pengurusan Portal/Laman Web Agensi Sektor Awam*

Issued by **Jabatan Digital Negara (JDN), Kementerian Digital**, Ogos 2025.
Reference: `JDN.100-1/3/2(2)`. Effective immediately upon issuance.

This circular **replaces six earlier documents**, most notably **PKPA Bilangan 2 Tahun 2015: Pengurusan Laman Web Agensi Sektor Awam**.

Official queries: `bkdjdn@jdn.gov.my` · https://www.jdn.gov.my

The full source PDF and a section-by-section analysis live in [`references/`](references).

## Repo Layout

```
.
├── SKILL.md                    The skill itself, source of truth for behaviour
├── README.md                   This file
├── LICENSE                     MIT
└── references/
    ├── pekeliling-1-2025.pdf   JDN Pekeliling (authoritative source)
    ├── surat-iringan-ksn.pdf   KSN cover letter
    ├── pekeliling-1-2025.txt   Plain-text extract (grep-friendly)
    ├── surat-iringan-ksn.txt   Plain-text extract
    └── analysis.md             Section-by-section analysis of the Pekeliling
```

## Maintenance

When JDN issues a new pekeliling or amendment:

1. Replace the PDF in `references/` with the new version.
2. Re-verify every section in `SKILL.md` against the new text.
3. Update the `description` frontmatter and the **Source & Versioning** footer in `SKILL.md` with the new bilangan/tahun.
4. Regenerate the plain-text extracts:
   ```
   pdftotext -layout references/pekeliling-1-2025.pdf references/pekeliling-1-2025.txt
   ```
5. Refresh `references/analysis.md`.
6. Tag the repo with the new pekeliling version (e.g. `v2026.1`).

## Contributing

Spot a missing [M] item, a misclassified [R], or a stale reference? Open an issue or PR.

Please cite the relevant Pekeliling section (e.g. *"Bab 3.3 perenggan j"*) in the description so reviewers can verify against the source.

## Disclaimer

This is an **unofficial, community-maintained skill**. The authoritative source is JDN's Pekeliling itself, and the Pekeliling supersedes anything in this repo in case of conflict. For binding interpretation, refer to JDN directly.

The PDFs in `references/` are Malaysian Government public documents, reproduced here in their original form for source-of-truth verification only.

## License

[MIT](LICENSE). Fork it.
