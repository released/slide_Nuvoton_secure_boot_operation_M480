# Web slide verification record

## 2026/11/05 current delivery — Keil-only BSP repositories published

- User authorized simplifying both examples to Library/SampleCode/README/.gitignore
  and publishing them to GitHub. Removed scripts/docs/output and SELF_CHECK from
  the two firmware roots only after verified copies were saved under ignored
  output/internal/bsp_github_20261105. Its manifest preserves original paths,
  file hashes and the protected firmware-source baseline; no engineering history
  was discarded. Machine-generated Keil user/driver settings remain local/ignored.
- Both READMEs now open the actual Keil projects/targets and identify the BINs in
  their obj directories. Updated this slide's build table, deployment file names
  and actual repository source links; existing concepts/anchors/style/screenshots
  and flow diagrams are preserved. This website change is local, not deployed.
- NEW PASS: exported the exact staged Git trees into a newly owned temporary
  directory, without scripts/docs/output or pre-existing object files. Keil6.22
  rebuilt LDROM, APROM and SRAM APROM with0 errors/0 warnings. Existing archived
  validators were run with only their project-root assignment redirected to the
  clean trees; flash/RAM/vector/ROM-wrapper/branch checks passed. All three BINs
  match their prior hashes: LDROM1840 bytes, APROM7080 bytes, SRAM APROM9472 bytes.
- NEW PASS:211 dedicated-LDROM and179 SRAM source files match the pre-cleanup
  SHA256 baseline. Public trees contain213 and181 files, respectively; no build
  output, user Keil settings or engineering records were uploaded. Preserved SDK
  CRLF/whitespace caused the initial all-added-file whitespace audit to flag SDK
  formatting; no vendor source was reformatted. Changed README/.gitignore checks
  pass with CR-at-EOL accounted for.
- Published public repositories released/M480BSP_ISP_HID_20_SecureBoot at
  972c1b317803a2ac611a00bcfb5aa7633ac0f8d8 and
  released/M480BSP_ISP_HID_20_SecureBoot_SRAM at
  4189035c5b426e06fdba18cc34a90d4d320cad41, both main. Remote refs, commit trees,
  root entries and README bytes match the tested local trees; both local worktrees
  are clean and track origin/main. No existing repository was overwritten.
- NEW Chrome156 PASS:37 headings/19 loaded screenshots/3 Mermaid diagrams,
  desktop1440x1000/mobile390x844, valid anchors/README project links, no overflow
  or browser errors, working mobile TOC and print CSS. Build table and README
  desktop/mobile appearance reviewed; path table condensed to remain readable.
- Retain build logs, original records, qa_plan.json, publication.json and final
  verification under the ignored archive; browser evidence remains in
  output/review/bsp_publish_docs_20261105.json. Task-owned clean build tree,
  renderer scripts and captures are retired after review with scoped/hash checks.
- NOT RUN: new board programming, runtime authentication, fault/recovery testing
  or website publication. Earlier user-reported hardware coverage remains the
  evidence for device behavior; this revision changes delivery/docs only.

Earlier records below describe preceding documentation layouts and local-only
firmware repositories; current delivery status is defined above.

## 2026/11/05 current documentation — details owned by the slide

- Final user-directed scope keeps each firmware README to28 lines: purpose, build,
  five quick verification steps and essential limits. Detailed concepts and
  operation remain in this guide, with stable direct links from both READMEs.
- Added the build/toolchain/output section and separated power-on Secure Boot
  authentication from update-time PC-tool/MCU responsibilities. Explained the
  KPROM prompt, successful programming and executable/re-enterable APP as separate
  observable stages. Kept the original style, screenshots and three flow diagrams.
- NEW Chrome156 PASS:1440x1000 and390x844,37 headings/36 TOC links,19 loaded
  screenshots,3 Mermaid diagrams; anchors, mobile TOC navigation, print CSS and
  homepage entry passed with no browser errors or overflow. Both short READMEs
  passed desktop/mobile, five-step and cross-document slide-anchor checks.
  Concept/PC-tool/mobile/README captures were visually reviewed.
- Firmware BIN/HEX hashes match the pre-edit baselines. No firmware source,
  configuration or build was changed/run; no independent board test or publication
  was performed. Earlier seven-section README/34-heading checks below describe
  intermediate documents, not the current public copy.
- Retain output/review/refocus_20261105_browser.json and refocus_20261105_final.json;
  retired test-only scripts/captures are accounted for in the final record. Earlier
  README versions and their hash baselines remain under ignored output/internal.

## 2026/11/05 two vendor ROM API examples and operation READMEs

- Added equal-level dedicated-LDROM and APROM/SRAM example descriptions, build
  file/output names, shared SW2/UART0 digit1 instructions and a complete SRAM
  installation/repeat-update chapter with a third Mermaid/SVG flow. Kept the
  current shared renderer/style, nineteen screenshots, existing anchors and two
  existing diagram bytes. Custom bootloader/MCUboot content remains outside scope.
- The user now reports normal SRAM hardware verification. Updated the current
  guide's applicability/evidence accordingly, while keeping individual trigger,
  version, preservation and failure-recovery coverage qualified. The older scope
  record that removed SRAM is superseded by this explicit example request; the
  custom/customer-LDROM chapter remains archived outside public content.
- Updated the site description/README and the homepage Markdown/HTML entry for
  both examples and SW2/KEY1. Firmware repository URLs are not established yet;
  current example links lead to their operation sections, without invented or
  local-disk download URLs.
- Rewrote both firmware READMEs as neutral, ordered operation guides. Their
  SELF_CHECK files retain engineering history and distinguish new documentation
  checks, reused build evidence and user-reported hardware results.
- NEW browser PASS: Chrome156 desktop1440x1000/mobile390x844,34 headings/33 TOC
  links,19 loaded screenshots,3 Mermaid diagrams; no missing anchors, duplicate
  IDs, document overflow or browser errors. Mobile TOC, print CSS and homepage
  entry checks passed. Desktop example/trigger/SRAM and narrow SRAM captures were
  visually reviewed. Each firmware README also passed desktop/mobile, seven-step,
  one-diagram and content-link checks; rendered desktop captures were reviewed.
- Retain concise evidence examples_20261105_browser.json and
  readmes_20261105_browser.json under ignored output/review. Owned test-only
  scripts/captures are retired after review; pre-existing artifacts are preserved.
  The two loopback preview servers close in their finalizers.
- NOT RUN: new firmware builds, agent-operated board programming or publication.
  Exported firmware hashes remain unchanged. No PDF exists here; PDF refresh is
  N/A. No commit, push or deployment is performed.

The dated records below remain engineering history; current example scope and
SRAM hardware evidence are defined by the update above.

## 2026/11/05 neutral public wording

- Editorial-only update removes the public README's local-validation/no-push
  paragraph and shared-file change-history clause. Existing maintenance records
  retain that historical execution status; this revision does not publish the site.
- Public purpose, sample-key explanation and hardware evidence now use neutral
  language. Preserve the existing reported dedicated-LDROM SW2 and SRAM board
  results and every explicit entry/version/preservation/recovery coverage limit.
  No new independent hardware test or newly broadened acceptance is claimed.
- Existing index/README/diagrams/SELF_CHECK modifications remain the baseline;
  no firmware, screenshot, SVG, UI code, technical constants or anchors are changed.
- PASS targeted source/links/UTF-8/fences/diff checks. Original technical code,
  Mermaid blocks and stable anchors remain exact; public evidence still identifies
  reported board coverage and untested preservation/recovery, without author-work
  history. Shared policies and generated copies agree; approved old phrases gone.
- NEW PASS installed Chrome, private profile: M480/#verification at1366x900 and
 390x844,3 diagrams/13 tables; no missing images, duplicate IDs, broken anchors,
  document overflow or console errors. Actual JavaScript-disabled CAN fallback
  shows neutral text. Changed desktop/narrow/fallback captures visually reviewed.
- Reused the existing Tool test_web_browser runner in memory with only two affected
  routes; redirected all owned output under this project's output/review, not
  sibling projects. The browser connector was unavailable. Existing test/source
  files and shared rendering code were not modified.
- Retired338 generated files /15,606,723 bytes plus the disposable retirement
  manifest; the entire owned run is absent. Exact ownership/hash/path/process
  checks stayed within this project. Long-path empty directories needed extended
  paths; no user/recovery data or original screenshot/SVG was deleted.
- NOT RUN: new app/firmware/hardware acceptance or published-site verification.
  No PDF exists here. No commit/push/deployment is performed by this editorial task.

Latest record: 2026/11/05, Asia/Taipei. Local project: `slide_Nuvoton_secure_boot_operation_M480`.

## 2026/11/05 vendor operation scope

- User requested no custom-bootloader content in the web slide. Removed the customer-LDROM/SRAM architecture chapter, its reading-route/API/configuration/acceptance cross-references, and the third standalone diagram from the public asset tree. Renumbered troubleshooting/acceptance to7/8 while retaining their stable anchors.
- Preserved vendor Mask ROM/BootIspLib explanations, dedicated LDROM/APROM example, ICP/KPROM/SBK screenshots, SecureBootTool flow, SW2/UART1-character entry trigger, all requested official references and the existing shared style. UART trigger and unverified hardware limits remain qualified.
- Updated index.html description and README scope/diagram count. The homepage already describes vendor ICP/HSUSB/LDROM/APROM/SW2/UART operation only, so its existing uncommitted Markdown/HTML were left untouched. Firmware projects were not changed.
- Preserved the removed chapter and its exact SVG under ignored output/internal/scope_20261105, with a purpose/hash manifest. This is engineering recovery material outside the public slide, not discarded user work.
- NEW browser PASS, Chrome156: desktop1440x1000 and mobile390x844, 26 headings/25 TOC links,19 loaded screenshots,2 Mermaid diagrams, no duplicate IDs/broken anchors/document overflow, menu/TOC navigation and print CSS; no console/page/network asset errors. Explicit rendered-text check finds no custom/customer-LDROM/SRAM/MCUboot/I2C0 content.
- NEW visual review PASS: desktop opening scope/TOC, troubleshooting/acceptance and mobile menu preserve the existing appearance and show the revised eight-section flow.
- Static PASS: image-manifest hashes, unchanged remaining SVG/screenshot bytes, requested reference URLs, Markdown fences/links and git diff --check. No PDF exists for this site, so PDF refresh is N/A.
- Test-only preview/captures/script/logs are owned fixtures: close only the loopback preview process, retire them after review, retain concise output/review/scope_20261105_browser.json and scope_20261105_final.json. Prior review artifacts and all unrelated modifications remain untouched.
- NOT RUN: new hardware tests or published-site verification. No commit/push/deployment performed.

The following 2026/11/04 and earlier records are retained engineering history; their three-diagram/custom-integration scope is superseded by the revision above.

## 2026/11/04 concepts, entry methods and SRAM example

- Added the Secure Boot/Secure ISP comparison and all three requested official reference URLs. Clarified configured firmware authentication regions, KPROM authorization, SBK/IB roles and full reset versus the CPU-only loader handoff.
- Documented the dedicated LDROM image's BootIspLib wrappers, HSUSB setup and interrupt forwarding; the main secure engine remains in MCU Mask ROM. The supplied M487 header exposes HSUSBD/UART1 APIs; UART0 ASCII `1` is an application entry trigger, while this example still transfers firmware over HSUSB.
- Added application integration guidance for `secure_update.h`, Init/Request/Poll, custom event triggers and vector/IB/peripheral constraints. Dedicated LDROM reuse is qualified for the same board/configuration; existing customer bootcode requires a separate architecture decision.
- Updated the APROM/SRAM section for the implemented sibling example. It is build/static verified and hardware pending. IB storage location is distinguished from the firmware regions authenticated by that IB.
- Preserved the shared style, all 19 screenshot bytes and the exclusion of customer questionnaires from the rendered teaching guide. Updated the homepage entry description in both Markdown and its HTML projection.
- Current local Git repositories exist for the guide and homepage. The older no-repository observations below describe 2026/11/03 only. No commit, push or deployment was performed during this revision.

| New check | Actual result |
| --- | --- |
| Desktop 1440 x 1000 | PASS: 31 headings, 30 TOC entries, 19 loaded screenshots, 3 Mermaid diagrams, valid anchors and no document overflow |
| Mobile 390 x 844 | PASS: no document overflow; menu and repeat-update TOC navigation work |
| Layout and print CSS | PASS: desktop concept/repeat/integration captures reviewed; shared accent/font preserved; print sidebar/controls hidden |
| Browser errors/assets | PASS: no JavaScript console/page errors or failed content/asset requests |
| Static content/assets | PASS: UTF-8, fences, local links, requested URLs/API text, 19 screenshot hashes, parseable SVGs and synchronization with the three Mermaid source blocks |
| Firmware evidence | NEW PASS: original APROM rebuild and standalone SRAM build/static/C90/negative-bound checks; original LDROM image unchanged. Detailed logs and hashes belong to each firmware project's SELF_CHECK |
| Hardware | REUSED user-reported PASS: original dedicated-LDROM SW2 cycle. NOT RUN: new UART trigger, SRAM USB/authentication/program/reset/reentry, preservation and interrupted-update recovery |
| Interactive device access | Unavailable: read-only inventory returned no apps/browsers and Windows native pipe os error 2; no board/configuration/key operation performed |

Current evidence: `output/review/browser-check.json`, `browser-check-console.txt`, `validation_20261104.txt`, final viewport captures and synchronized SVG exports. Custom UART0/I2C0 transport is recorded as a later engineering phase, not an implemented feature or a demonstrated SecureBootTool compatibility claim.

Final PASS: homepage Markdown/HTML entry descriptions match, both affected repositories pass `git diff --check`, and the owned preview server was stopped with port 8768 confirmed closed. Task-owned firmware renderer temporaries/duplicate log were retired; final web captures and verification evidence remain. Record: `output/review/final_check_20261104.json`.

The following sections retain the 2026/11/03 baseline and its verification history; implementation and repository-state statements in that history are superseded by the current revision above.

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
