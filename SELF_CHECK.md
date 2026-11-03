# Web slide verification record

Record: 2026/11/03, Asia/Taipei. Local project: `slide_Nuvoton_secure_boot_operation_M480`.

## Scope and content decisions

- Created a local web guide from the provided image-only directory. Followed `/web/AGENTS.md` and `PUBLIC_CONTENT_GUIDELINES_zh-TW.md`.
- Reused the exact common stylesheet and application script referenced by the existing Nuvoton ISP pages. Preserved their teal accent, typography, sidebar, Markdown rendering and Mermaid theme. Shared files and sibling projects were not edited.
- Canonical content is `index.md`; `index.html` is the common-template shell. Standalone SVGs are projections of the three Mermaid blocks rendered by the same page renderer.
- Covered ICP CONFIG/Boot Loader/Security Lock, forced checked/disabled Secure Key, SBK generation/export/loading, KPROM, and Config/KPROM/Secure Key programming selection.
- Covered SecureBootTool Waiting, Loading, KPROM authentication, Connected, Key Options, first deployment and later APROM-only updates with SW2.
- Customer inquiry material is retained only in `output/internal/CUSTOMER_PROJECT_ASSESSMENT.md`, outside the rendered teaching content and excluded from website Git files. The guide presents operation steps, configuration, applicability and limits.
- Separated the user-confirmed dedicated-LDROM procedure from the unimplemented APROM/SRAM proposal. Documented APROM-only, LDROM-only and combined target cases, IB placement and the potential 144-byte LDROM capacity conflict.

## Files and purposes

| File/group | Purpose |
| --- | --- |
| `index.md` | Single editable operation guide, configuration and applicability/limits |
| `index.html`, `assets/favicon.svg` | Existing-site template shell and matching NU icon |
| `assets/screenshots/` | 19 reviewed website screenshots and source/hash manifest |
| `assets/diagrams/` | Three full-size standalone SVG projections |
| `README.md` | Source locations, local HTTP preview and asset handling |
| `.gitignore`, `.gitattributes` | Exclude original private-path images/local QA; consistent text files |
| `SELF_CHECK.md` | Actual verification, evidence ownership and remaining limits |

## Image handling

- Original `img/` files remain unchanged and are excluded by `.gitignore`. Eighteen website images are exact byte copies of selected originals; the manifest records hashes.
- The user explicitly authorized visible educational SBK/KPROM example values. Those examples remain in the relevant screenshots and are labeled in the guide.
- `icp-main-redacted.png` is a non-destructive privacy edit of `ICP_#000.jpg`, produced with the built-in imagegen tool. Paths in all seven filename fields and the Nu-Link identifier were mosaicked. The resulting UI/configuration and masking were visually reviewed; the page displays the image at the original screenshot's approximate size.
- Remaining used images were reviewed for personal paths. The export screenshot already has its directory portion mosaicked; the visible key BIN filename is part of the procedure.

Prompt used for the privacy edit:

> Edit this exact technical screenshot for a public step-by-step guide. Use case: precise-object-edit, privacy redaction. Preserve the original screenshot composition, buttons, fonts, UI layout, logos and technical settings exactly. Do not redesign or recreate the interface. Apply opaque coarse grayscale pixel mosaic over ONLY (1) every filesystem path value inside all seven File Name input fields (LDROM, APROM, Data Flash, SPROM, SPI Flash, Secure Key, OTP); mosaic the entire contents across the full visible field width, with no readable drive letter or path fragments; and (2) the unique Nu-Link ID digits in the green connection status line. Keep the labels File Name, buttons Secure Key and Setting, CONFIG values, chip M487JIDAE and red annotation intact. Input is 515x652; keep same aspect ratio and readable screenshot quality. Do not add callouts or annotations.

## New local verification

Actual browser: headless Chrome `156.0.8078.49`, using the existing cached Puppeteer runtime. Local HTTP preview served from `/web`, bound to `127.0.0.1:8768`.

| Check | Actual result |
| --- | --- |
| Desktop 1440×1000 | PASS: 28 headings, 27 TOC entries, 19 loaded screenshots, 3 rendered Mermaid diagrams |
| Anchors and IDs | PASS: unique IDs, no missing internal targets; TOC click reaches operation acceptance checks |
| Mobile 390×844 | PASS: no document overflow; menu toggle and TOC navigation follow the existing site's behavior |
| Template comparison | PASS: reference/current screenshots inspected; same shared CSS/JS, accent and font family |
| Image/diagram layout | PASS: final desktop section captures, mobile captures and all three diagram captures visually inspected; shortened labels to preserve readable word wrapping |
| Print media CSS | PASS: sidebar and controls hidden; content left offset removed. This is a stylesheet check, not PDF pagination verification |
| JavaScript/network | PASS: no console/page errors or failed content/asset requests in the final run |
| Markdown/local links | PASS: balanced fences, unique explicit anchors, image and internal links resolve |
| Image manifest | PASS: 19 hashes verified; 18 direct copies match their source bytes |
| Standalone diagrams | PASS: three SVGs parse as XML and return HTTP 200 with image/svg+xml |
| Public text paths | PASS: no personal drive paths in canonical Markdown |

Evidence: `output/review/browser-check.json`, `static-check.txt`, final viewport/diagram PNGs and local verification script. These are new web checks. Input contact sheets are disposable; final review evidence is retained outside the website Git files.

## Reused evidence and verification limits

- Firmware/hardware evidence is reused from the user's supplied screenshots and successful update-cycle report. No new board programming, key submission, CONFIG write, firmware modification or firmware build was performed.
- NOT RUN: custom-LDROM integration, SRAM updater implementation/build/hardware test, general-ISP regression after security enablement, byte-level LDROM/CONFIG preservation and power-loss recovery.
- Native interactive browser access was unavailable. Validation used a local headless browser; no live user-browser interaction is claimed.
- The guide requires the same CDN-provided Marked/Mermaid resources as its reference pages. Their load succeeded during the final local checks; offline packaging was not requested.
- No pre-existing PDF existed in this project. No PDF deliverable or pagination result is claimed.
- No Git repository was initialized, commit/push performed, hosting registered or website deployed. No public URL is asserted.

## Retention and teardown

- Retain source Markdown/HTML, reviewed assets, SVG projections, original input screenshots and final local review evidence.
- Remove task-owned contact sheets after inspection; preserve all original input files and unrelated work.
- PASS: the task-owned local preview server was stopped; port 8768 no longer accepts connections. Both task-owned contact sheets were removed; all 24 original input JPGs remain. Details are recorded in `output/review/teardown-check.json`.

## Teaching scope correction — 2026/11/03

- Removed the customer questionnaire, its navigation/reading links and consultation wording from the public guide and README. Preserved the material separately in the ignored internal document; it is not linked from the teaching page.
- Renumbered the remaining chapters and replaced survey-based instructions with operation prerequisites and acceptance criteria. Kept the distinction between the verified dedicated-LDROM flow and unverified SRAM alternative.
- NEW PASS: final local headless desktop/mobile run confirms no customer/survey content in the rendered guide, 28 headings/27 TOC entries, 19 images, 3 diagrams, working anchors/menu and no console/network errors. Final top/integration screenshots were visually reviewed.
- NEW PASS: `scope-correction-static.txt` records no questionnaire references in public content; all layout/image/SVG hashes and all three Mermaid source blocks match the pre-edit baseline. No shared style, HTML shell, image or diagram content changed.
- Hardware/build results above remain reused evidence. No firmware or device operation, Git push or deployment was performed for this content correction.

## Homepage entry synchronization — 2026/11/03

- Added the operation-guide entry under Nuvoton in the homepage repository's `README.md` and synchronized its `README.html` export. The existing homepage shell loads that Markdown automatically.
- Target path is `/slide_Nuvoton_secure_boot_operation_M480/`. Updated this site's README to record the path and local-only publication state.
- NEW PASS: entry label, description and URL match between Markdown/HTML; local target HTML/Markdown exist; homepage Git diff has no whitespace errors. Evidence: `output/review/homepage-link-check.json`.
- Read-only publication inspection: the homepage is on `main`; the new guide has no Git metadata yet. GitHub CLI is authenticated, and the target new repository was not found. No repository was initialized or created, and no commit/push was executed.
- NOT RUN: publication hooks, remote push and GitHub Pages deployment. The requested publication commands are instructions for the user to execute; they do not constitute a completed publication.
