# References & Provenance

This document lists the sources used in this repository and explains the provenance of both (1) the how-to steps extracted from the Kestrel 5400 user guide and (2) formulas/definitions used on the Glossary tab. It also describes how measurement data in `/data/` were produced (to be completed by the user after each session).

---

## 1) Device Guide (extracted operational steps)

**Primary source used for:**
- WBGT configuration (Type: Indoor/Outdoor; Zones/Guide; Alerts) and alert behavior  
- Accurate measurement protocol (8–15 minute equilibration; ~1 m/3 ft height; orientation into wind; tripod/vane; surface/radiation notes)  
- Logging and on-device graphing (Auto Store, Store Rate, Overwrite; Graph/Graph Scale; manual Capture; Data Log Detail)  
- Options & setup (Auto Shutdown; Compass calibration procedure; Backlight; Time & Date; Measurements; Units; Language)  
- Export methods (Kestrel LiNK app; USB LiNK dongle; USB Data Transfer Cable; Data Port setting)

**Citation:**  
Kestrel Instruments. *Kestrel 5400 Heat Stress Tracker — User Guide* (PDF). Kestrel Instruments. (Accessed in this project’s uploads). See also Kestrel’s manuals/downloads index and public manual mirrors for cross-check. :contentReference[oaicite:0]{index=0}

**Provenance (how we used it):**  
- The “How-To Steps” tab (`html/steps.html`) is a paraphrased, ordered extraction from the Kestrel 5400 user guide to create a concise operational checklist.  
- We avoided long verbatim passages and kept terminology consistent with the guide.  
- Where the guide specified times and procedures (e.g., “8–15 minutes” equilibration; compass cal ~3 turns, ~10 s each), those details were retained in paraphrase form.

---

## 2) Standards & public guidance for WBGT

**What these are used for:**  
- Glossary formulas for WBGT (outdoor with sun; indoor/no sun)  
- Definitions of T<sub>nwb</sub>, T<sub>g</sub>, T<sub>a</sub> and their roles in WBGT

**Citations (core):**
- International Organization for Standardization. *ISO 7243:2017 – Ergonomics of the thermal environment — Assessment of heat stress using the WBGT (wet bulb globe temperature) index.* ISO, 2017. Official abstract/landing page. :contentReference[oaicite:1]{index=1}  
- Public preview/hosting of ISO 7243:2017 text for reference (for formula context and clothing adjustment notes). :contentReference[oaicite:2]{index=2}  
- NIOSH (Centers for Disease Control and Prevention). *Criteria for a Recommended Standard: Occupational Exposure to Heat and Hot Environments.* DHHS (NIOSH) Publication No. 2016-106, 2016 (PDF). See WBGT usage and formula context. :contentReference[oaicite:3]{index=3}

**Additional consistent references (formula statement & explanation):**
- National Weather Service (WFO ICT). “Wet Bulb Globe Temperature vs Heat Index.” Equation and component definitions. :contentReference[oaicite:4]{index=4}  
- Lemke, B., & Kjellstrom, T. “Calculating Workplace WBGT from Meteorological Data.” *Industrial Health* 50(4):267-278, 2012. (JNIOSH). Explains WBGT components and usage. :contentReference[oaicite:5]{index=5}

**Provenance (how we used them):**  
- The Glossary tab (`html/glossary.html`) includes the standard WBGT formulas:  
  - **Outdoors with solar load:** WBGT = 0.7·Tₙwb + 0.2·Tg + 0.1·Ta  
  - **Indoors/no sun:** WBGT = 0.7·Tₙwb + 0.3·Tg  
  These equations and component definitions were aligned with ISO/NIOSH and cross-checked with NWS/JNIOSH summaries.

---

## 3) TWL (Thermal Work Limit)

**What this is used for:**  
- Glossary definition and short description of the Kestrel 5400’s TWL readout and work-zone categories (Unrestricted, Acclimatization, Buffer, Withdraw).

**Citations:**  
- Kestrel Instruments. *Kestrel 5400 User Manual (public mirror entry).* TWL description and categories. :contentReference[oaicite:6]{index=6}  
- Kestrel Instruments. *Kestrel 5400 Heat Stress Tracker — product/support pages* (context for TWL feature across Kestrel 5400 materials). :contentReference[oaicite:7]{index=7}

**Provenance (how we used it):**  
- The Glossary summarizes TWL as presented in the Kestrel 5400 materials, clarifying it as a **cooling-capacity** estimate (W/m²) used to drive operational categories, distinct from WBGT (an environmental index).

---

## 4) Data provenance for this repository’s CSVs (fill this out after each run)

> Replace the placeholders below for each uploaded dataset in `/data/`.

**Example template (copy and edit):**
- **File:** `data/2025-09-17_run1.csv`  
- **Collector:** Robert Lehr  
- **Device:** Kestrel 5400 Heat Stress Tracker, firmware v?.?  
- **WBGT Type:** Outdoor | **Zones/Guide:** [name/version] | **Alerts:** [Light/Buzzer settings]  
- **Logging:** Auto Store = On | Store Rate = 10 min | Overwrite = On  
- **Setup:** height ≈ 1 m; vane + tripod; back of unit into wind; surface = asphalt (full sun)  
- **Location & time:** Austin, TX, USA; 2025-09-17 10:00–10:40 local  
- **Export path:** Kestrel LiNK iOS vX.Y → CSV (no post-processing)  
- **Edits:** none (except column renames from `wbgt_outdoor_c` → `WBGT_C`)

---

## Notes on reuse / fair use
Short excerpts and paraphrases from device manuals are included for education/documentation. For full technical details, consult the device guide and the ISO/NIOSH documents referenced above.
