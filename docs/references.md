# References & Provenance

## Kestrel 5400 Guide (extracted steps)
- Kestrel 5400 Heat Stress Tracker User Guide, sections: WBGT setup (Type, Zones/Guide, Alerts), alerts behavior, equilibration (8–15 min), measurement height (~1 m), wind orientation, surface/radiation notes, Memory Options (Auto Store/Rate/Overwrite), Graph/Graph Scale, Auto Shutdown, Compass Cal (3 rotations ~10 s), Backlight, Time & Date, Measurements, Units, Language, manual capture, graph/log details, exports (LiNK dongle/USB).

**Provenance:** Steps reproduced/abstracted from the uploaded PDF; extracted on <DATE> for field protocol documentation.

## WBGT Formulas (standards)
- NIOSH Criteria for a Recommended Standard (Heat Stress) – WBGT formulas.
- ISO 7243:2017 – Assessment of heat stress using WBGT (details as above).

Formulas:
- Outdoors with sun: `WBGT = 0.7·Tnwb + 0.2·Tg + 0.1·Ta`
- Indoors/no sun:  `WBGT = 0.7·Tnwb + 0.3·Tg`

## TWL Overview
- Kestrel materials describing TWL categories (Unrestricted, Acclimatization, Buffer, Withdraw).

## Data Provenance (example for your CSVs)
- Device: Kestrel 5400, WBGT Type: Outdoor, Zones: [Guide X], Alerts: [Light+Buzzer],  
  Logging: Auto Store=On, Rate=10 min, Overwrite=On;  
  Location: <City, site>, Height: ~1 m, Mount: vane+tripod;  
  Export: Kestrel LiNK (iOS vX.X) → CSV; Post-processing: none (except column renames).
