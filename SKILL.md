---
name: patuh
description: Use when building, reviewing, or auditing an official Malaysian public-sector (Agensi Sektor Awam) website or portal (government website, laman web kerajaan, gov.my site, kerajaan portal), or when checking compliance with JDN's Pekeliling Pendigitalan Perkhidmatan Awam Bilangan 1 Tahun 2025. Also use for rasionalisasi (deciding which agency portals to keep/close/merge). Triggers (EN): gov.my website build, audit gov site, government portal compliance, Sektor Awam website requirements, Pekeliling 1 2025, JDN compliance, MyGovernment integration. Triggers (BM): audit laman web kerajaan, patuh pekeliling JDN, semak laman gov.my, laman sektor awam, bina portal kerajaan, rasionalisasi laman web, pekeliling pendigitalan, panduan JDN.
---

# patuh: Malaysian Government Website Compliance

Source of truth: **Pekeliling Pendigitalan Perkhidmatan Awam Bilangan 1 Tahun 2025: Pengurusan Portal/Laman Web Agensi Sektor Awam**, issued by **Jabatan Digital Negara (JDN)**. Every official agency site **MUST use a `gov.my` domain.**

## How to use this skill

Use it in three modes:
- **Build mode**: design and develop a new agency site against the mandatory list before handover.
- **Audit mode**: check an existing agency site and report each item as pass / fail.
- **Rasionalisasi mode**: when an agency has more than one portal/laman web/blog, classify each and decide what to keep, close, consolidate, or exempt (see §5).

Two force levels, never mix them up:
- ✅ **[M] MANDATORY**: the circular's *hendaklah / mesti / mandatori / perlu*. Non-negotiable for compliance.
- 💡 **[R] RECOMMENDED**: the circular's *digalakkan / disarankan / boleh*. Good practice, not a compliance failure if absent. **Never report an [R] miss as a failure.**

Keep all official Malay labels verbatim on the site itself (Jata Persekutuan, Soalan Lazim, Hubungi Kami, Aduan dan Maklum Balas, Peta Laman, Piagam Pelanggan).

### 🛑 Hard-fail short-circuit
**If the site is not on a `gov.my` domain, stop the audit.** JDN treats `gov.my` as the non-negotiable identity of an official agency site. Nothing else matters until the domain is correct. Report this as the single finding and resume once the domain is in place.

### What this skill covers (and what it does not)
**In scope:** site build, site audit, portal rasionalisasi (Pekeliling Bab 3–6).

**Out of scope (refer to the Pekeliling directly):**
- **Tadbir urus / governance (Bab 2)**: establishing the Jawatankuasa Induk + Pasukan Kandungan + Pasukan Teknikal at ministry/department level. This is an organisational task, not a site-build task.

### Audit-mode deliverable format
Produce one Markdown report with these sections, in order:
1. **Hard-fail check**: `gov.my` domain yes/no. If no, stop here.
2. **Per-section findings**: Reka Bentuk → Kefungsian → Kandungan → Keselamatan → Ops → Performance → Must-not. Each [M] item: ✅ pass / ❌ fail / ➖ N/A, plus one-line evidence (URL or quoted text). Skip [R] items unless the user asks for them.
3. **Rasionalisasi check**: only if the agency runs more than one portal/laman web/blog.
4. **Summary table**: total passed / failed / N/A per section.
5. **Top 5 priority fixes**: ordered by user-impact, then compliance risk.

---

## 1. Reka Bentuk (Design)

### ✅ MANDATORY [M]
- The statement **"Portal/Laman Web Rasmi"** appears on the homepage.
- Correct official emblem on the homepage: federal public-service agencies use the **Jata Persekutuan** (federal coat of arms) only; other agencies use the **Jata Negeri** (state crest) or their official agency logo. Special/custom logos only with gazette or approval (ref: Surat Pekeliling Am Bil. 1/2022).
- Consistent look-and-feel across the entire site.
- Core services prioritised; information laid out strategically.
- Font type and size **uniform across all pages**.
- Icons uniform in design and each **≤ 1KB**.
- A search function on **every page**.
- Four main links sit at the **top-right of the homepage** with uniform icons: **Soalan Lazim** (FAQ), **Hubungi Kami** (Contact Us), **Aduan dan Maklum Balas** (Complaints & Feedback), and **Peta Laman** (Site Map).
- "Hubungi Kami" shows **only** the agency's official address and phone.

### 💡 RECOMMENDED [R]
- No more than 3 colours; white background preferred.
- Pop-ups only as needed.
- Follow the Government Digital Service design standard at `standard.digital.gov.my`.

---

## 2. Kefungsian (Function)

### ✅ MANDATORY [M]
- **Bilingual**: Bahasa Melayu + English.
- Content language correct, free of grammar and spelling errors.
- **Soalan Lazim** (FAQ).
- Support links: help, troubleshooting, standard operating procedure (SOP), user manual, and a flowchart or video tutorial.
- Feedback facility **plus automatic acknowledgement with a reference number**.
- User-satisfaction survey.
- Hot-topic / tag-cloud labelling of popular content.
- Information grouped by target audience (e.g. citizen, business, researcher, journalist, student).
- An announcement/publicity section; show **"Tiada Makluman Terkini"** when there is nothing new.
- Latest-info push (email or syndication) for announcements, news, tenders, careers.
- Advanced search.
- A **W3C Disability Accessibility** version covering: colour-blind users (switchable / contrast background + a colour legend), visually impaired users (audio), hearing-impaired users (text or graphic for audio content), and elderly users (resizable font / type).
- Intelligent personalisation capability (welcome-back with last-visit info, topic-based email/SMS notifications, habit analysis).
- Electronic archiving of information older than 1 year, downloadable.
- External links: links to **Portal MyGovernment** (`malaysia.gov.my`) and **Portal Data Terbuka** (`data.gov.my`) are mandatory; links to sister agencies under the Ministry / State Secretary office are required; system/app links as needed.
- **MyGovernment URL upkeep**: keep every URL that MyGovernment has indexed live; **notify MyGovernment of any URL change** so the central gerbang tunggal does not develop broken links into the agency.
- Site map / index (**Peta Laman**).
- A mobile-device version (simplified versus desktop) **plus a QR code** to reach it.
- Key agency policies, **Piagam Pelanggan** (client charter), disclaimer (penafian), privacy & security policy, and copyright notice.
- Supports multiple technologies, devices, and operating-system platforms.
- For online-service authentication, consider/incorporate the **National Digital ID (IDN)**, the national federated identity scheme for secure identity verification across Malaysian government services.

### 💡 RECOMMENDED [R]
- Additional languages beyond BM + English.
- Refer to Dewan Bahasa dan Pustaka for correct Malay terminology.
- An AI chatbot for two-way interaction.
- Emerging tech (AI, blockchain) suited to the agency's function.
- Follow the latest **WCAG** (Web Content Accessibility Guidelines).

---

## 3. Kandungan (Content)

### ✅ MANDATORY [M]
- Corporate info: vision, mission, function, organisation chart, and the head's message.
- **Mengenai Kami** (About Us): introduction, administration, location, facilities.
- **Hubungi Kami** (Contact Us): phone, fax, address, agency email, and webmaster email. Email must be shown as **static text, not a clickable link** (anti-spam). Staff directory shown flexibly (a group or call-centre email is acceptable; protect individual staff details from fraud); the directory must be easy to reach.
- Chief Digital Officer (CDO) info: profile, news, activities.
- Latest info (announcements, news, press cuttings, tenders, vacancies) with **auto-expiry** for time-limited items.
- Downloadable documents, video/audio, and publications relevant to the agency's services.
- Core service info; online service info (e-Permohonan, e-Pembayaran, e-Aduan); and service-delivery channels with a channel icon beside each service.
- Service-delivery achievement metrics and usage %.
- End-to-end online services where applicable.
- **e-Penyertaan** (e-Participation): e-Information, e-Consultation, e-Decision. Consultation and decision records must stay accessible for **at least 6 months**, then be archived and remain downloadable.
- Open data: identify the data, confirm no legal restriction, get the head's approval, publish in a machine-readable format, and keep it updated (contact `dataterbuka@jdn.gov.my`).
- Use media (images/video) fit for the message; obtain the owner's permission if it is not the agency's own.
- Social media governed by an appointed admin: no content conflicting with government policy; moderate public comments; use the official agency email; carry a per-platform disclaimer; keep wording concise.

---

## 4. Keselamatan (Security), Operations & Maintenance

### ✅ MANDATORY [M]: Security
- Store/display **only official information + open data**. Secret-official information must be referred to the **CGSO** (Chief Government Security Office) first.
- Protect data in motion with a current, secure server digital certificate from **GPKI** (Government Public Key Infrastructure), JDN, or a local Certificate Authority (i.e. serve over **HTTPS**).
- Cyber-attack protection: firewall + **IPS** (intrusion prevention system); **WAF** (web application firewall); real-time anti-malware / anti-ransomware.
- Keep security patches current for the operating system, database, **CMS** (content management system), **all** CMS modules/plug-ins, and related apps.
- Build, maintain, and **periodically test** data backups and a **DRP** (Disaster Recovery Plan).
- Periodic information-security testing to find and fix vulnerabilities.
- Activate, maintain, and retain log files / audit trails for troubleshooting and ICT forensics.
- Report any cyber-security incident to the agency **CSIRT** (Computer Security Incident Response Team) or to NC4 / **NACSA** (National Cyber Security Agency).
- Periodically review content, configuration, and technology against current laws, policies, and directives.
- Protect data under **CIA**: Confidentiality, Integrity, Availability.

### ✅ MANDATORY [M]: Operations & Maintenance
- Adequate resources: software, hardware, licences, manpower, training, and transfer of technology (**TOT**).
- Backup + restore capability.
- Continuous information updates.
- Uptime and performance monitoring.
- A help desk.
- Complete documentation (manuals / user guides).
- Bug fixing, patching, and tuning.

---

## 5. Rasionalisasi Portal/Laman Web

Every agency is permitted **only one** official portal. When an agency runs more than one portal/laman web/blog, each must be classified into one of four categories (Pekeliling Bab 5):

| Category | Apply when… | Action |
|---|---|---|
| **Dikekalkan** (Retain) | Single official agency portal | Keep, one per agency |
| **Ditutup** (Close) | Duplicate · No longer needed · **Not maintained for > 6 months** | Close the site **and retire the domain** |
| **Dikonsolidasi** (Consolidate) | Branch / unit / division / section portal · Static or rarely updated · No dedicated admin | Merge into the parent agency portal as a **subdomain** or **subdirectory**; retire the standalone domain |
| **Dikecualikan** (Exempt) | Special-purpose, national-impact portal (e.g. `data.gov.my`, `myidentity.gov.my`) | Requires approval from the **Jawatankuasa Induk Pengurusan Portal/Laman Web Kementerian/Negeri** and notification to **JDN** |

**Approval flow:** Agensi Pelaksana proposes → JK Pengurusan Jabatan approves → JK Induk Kementerian/Negeri endorses → execute → report back to Agensi Induk → Agensi Induk submits latest list to JDN. (Flow chart and checklists are in Lampiran A5–A7 of the Pekeliling.)

---

## ⛔ TIDAK DIBENARKAN / MUST NOT

The site **must not**:
- Advertise third-party services. *Exception:* allowed only if it genuinely adds value to the agency's core/support services **and** a MOU/contract exists, with the agency carrying full liability.
- Display sensitive issues (religion, politics, race).
- Carry content unrelated to the agency's core/support services.
- Carry statements that could damage the government's image.

---

## 📊 Prestasi / Performance Targets

- Page display in **under 5 seconds** per click.
- **Click depth ≤ 3 clicks** to reach any information or service.
- Track and report: availability/uptime %, online-service transaction counts, feedback resolved within Piagam Pelanggan timeframes, and latest-info updated before its expiry date.

---

## Pre-launch / Audit Checklist (every [M] item)

Tick every box before handover, or mark pass/fail when auditing.

**Domain & identity**
- [ ] Site is on a `gov.my` domain
- [ ] "Portal/Laman Web Rasmi" shown on homepage
- [ ] Correct emblem (Jata Persekutuan / Jata Negeri / approved agency logo)

**Reka Bentuk (Design)**
- [ ] Consistent look-and-feel sitewide
- [ ] Core services prioritised; strategic information layout
- [ ] Uniform font type and size on all pages
- [ ] Uniform icons, each ≤ 1KB
- [ ] Search function on every page
- [ ] Four main links (Soalan Lazim, Hubungi Kami, Aduan dan Maklum Balas, Peta Laman) with uniform icons, top-right of homepage
- [ ] "Hubungi Kami" link shows only official address and phone

**Kefungsian (Function)**
- [ ] Bilingual BM + English
- [ ] Content language correct, no grammar/spelling errors
- [ ] FAQ (Soalan Lazim)
- [ ] Support links (help, troubleshooting, SOP, user manual, flowchart or video)
- [ ] Feedback facility + auto-acknowledgement with reference number
- [ ] User-satisfaction survey
- [ ] Hot-topic / tag-cloud
- [ ] Information grouped by target audience
- [ ] Announcement section; "Tiada Makluman Terkini" shown when empty
- [ ] Latest-info push (email/syndication)
- [ ] Advanced search
- [ ] W3C accessibility version (colour-blind, visually impaired, hearing impaired, elderly)
- [ ] Intelligent personalisation capability
- [ ] E-archiving of info older than 1 year, downloadable
- [ ] Mandatory external links to Portal MyGovernment + Portal Data Terbuka
- [ ] MyGovernment URL upkeep: change notifications in place to prevent broken links
- [ ] Links to sister agencies under Ministry / State Secretary office
- [ ] Site map (Peta Laman)
- [ ] Mobile version + QR code to it
- [ ] Key policies, Piagam Pelanggan, disclaimer, privacy & security policy, copyright notice
- [ ] Multi-technology / multi-device / multi-OS support
- [ ] National Digital ID (IDN) considered/incorporated for online-service identity verification

**Kandungan (Content)**
- [ ] Corporate info (vision, mission, function, org chart, head's message)
- [ ] Mengenai Kami (intro, administration, location, facilities)
- [ ] Hubungi Kami (phone, fax, address, agency email, webmaster email; email as static text; flexible directory)
- [ ] CDO info (profile, news, activities)
- [ ] Latest info with auto-expiry for time-limited items
- [ ] Downloadable documents / video / audio / publications
- [ ] Core + online service info (e-Permohonan, e-Pembayaran, e-Aduan) with channel icons
- [ ] Service-delivery achievement metrics and usage %
- [ ] End-to-end online services where applicable
- [ ] e-Participation (e-Information, e-Consultation, e-Decision); records accessible ≥ 6 months
- [ ] Open data (identified, legally clear, head-approved, machine-readable, kept updated)
- [ ] Media fit for purpose with owner permission
- [ ] Social media governance (admin, policy-compliant, moderated, official email, disclaimer, concise)

**Keselamatan (Security)**
- [ ] Only official info + open data stored/displayed (CGSO referral for secret-official)
- [ ] HTTPS via GPKI / JDN / local CA digital certificate
- [ ] Firewall + IPS, WAF, real-time anti-malware/ransomware
- [ ] Current patches (OS, database, CMS, all plug-ins, related apps)
- [ ] Backup + DRP built, maintained, and periodically tested
- [ ] Periodic information-security testing
- [ ] Log files / audit trails activated, maintained, retained
- [ ] Incident reporting path to CSIRT / NC4 / NACSA
- [ ] Periodic review of content, config, technology vs current laws/policies
- [ ] Data protected under CIA (Confidentiality, Integrity, Availability)

**Operations & Maintenance**
- [ ] Adequate resources (software, hardware, licences, manpower, training, TOT)
- [ ] Backup + restore
- [ ] Continuous information updates
- [ ] Uptime + performance monitoring
- [ ] Help desk
- [ ] Complete documentation (manuals / user guides)
- [ ] Bug fixing, patching, tuning

**Performance**
- [ ] Page display < 5 seconds per click
- [ ] Click depth ≤ 3 clicks
- [ ] Uptime %, transactions, feedback resolution, and info-update tracking in place

**Must-not (final pass)**
- [ ] No third-party ads (unless value-add + MOU, agency liable)
- [ ] No sensitive issues (religion, politics, race)
- [ ] No content unrelated to core/support services
- [ ] No statements that could damage the government's image

**Rasionalisasi (only if agency runs >1 portal/laman web/blog)**
- [ ] Every portal/laman web/blog classified: Dikekalkan / Ditutup / Dikonsolidasi / Dikecualikan
- [ ] Only one portal marked Dikekalkan
- [ ] Portals not maintained > 6 months marked Ditutup (site + domain)
- [ ] Branch/unit/division portals marked Dikonsolidasi (merged into parent as subdomain or subdirectory)
- [ ] Exempt portals (Dikecualikan) approved by JK Induk and notified to JDN
- [ ] Approval flow recorded: JK Pengurusan Jabatan → JK Induk Kementerian/Negeri → execution → report to Agensi Induk → list submitted to JDN

---

## Source & Versioning

**Source of truth:** Pekeliling Pendigitalan Perkhidmatan Awam **Bilangan 1 Tahun 2025: Pengurusan Portal/Laman Web Agensi Sektor Awam**. Issued by **Jabatan Digital Negara (JDN)**, Kementerian Digital. Ref `JDN.100-1/3/2(2)`, **Ogos 2025**. Effective immediately upon issuance.

This skill replaces guidance from the six circulars revoked by Pekeliling 1/2025, including the previously dominant **PKPA Bil. 2 Tahun 2015: Pengurusan Laman Web Agensi Sektor Awam**.

**Maintenance:** if JDN issues a new Pekeliling or amendment, the source-of-truth PDF in `pdf/` must be replaced and every section in this skill re-verified against the new text. The frontmatter `description` and Source block should be bumped to the new bilangan/tahun.

**Official pertanyaan:** Pengarah, Bahagian Kerajaan Digital, JDN. Email `bkdjdn@jdn.gov.my` · https://www.jdn.gov.my
