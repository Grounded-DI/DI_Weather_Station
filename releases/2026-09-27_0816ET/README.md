# DI Weather Station — Polo / separate Nolo evidence lane

Final archive packaging: 27 September 2026. Evidence-state scan: **08:16 AM ET**; hard source cutoff: **12:05 UTC / 08:05 AM ET**. This is a frozen documentary handoff, not a live forecast or executable weather runtime.

## Start here

1. Read `CURRENT_STATE.md` (inside the ZIP) and `CURRENT_STATE.json` for the latest packaged Polo state.
2. Read `evidence_states/DI_Weather_Station_Polo_Nolo_8_16AM_ET_Full_Dual_Storm_Scan_2026-09-27.pdf` for the controlling scan.
3. Read `evidence_states/NOLO_EVIDENCE_STATE_2026-09-27_0816ET.json` separately; Nolo is not merged into Polo's state.
4. Use earlier scans only at their stated historical cutoffs. Scheduled next-scan times are historical instructions, not evidence that a later scan occurred.

## Four preserved PDFs

- `DI_Weather_Station_Hurricane_Polo_ENTERPRISE_SAFE_v2.pdf` — earlier enterprise-safe baseline/handoff.
- `evidence_states/Hurricane_Polo_7_12AM_ET_Follow_Up_Scan.pdf` — earlier follow-up.
- `evidence_states/Hurricane_Polo_1_03AM_ET_Full_Source_Bound_Scan_2026-09-27.pdf` — September 27, 01:03 AM ET scan.
- `evidence_states/DI_Weather_Station_Polo_Nolo_8_16AM_ET_Full_Dual_Storm_Scan_2026-09-27.pdf` — September 27, 08:16 AM ET scan.

Both September 27 PDFs were already present in the supplied ZIP and remain byte-identical. Earlier scan records, current-state records and visual files are also unchanged.

## Evidence and visual scope

This packaging pass did not retrieve or independently reverify weather sources. Official values, DI inferences, reconstructed quantities and unresolved states retain the classifications in the reports. The older `LIVE_SOURCE_REFERENCES_2026-09-26_0000ET.json` supports that historical scan, not every later state.

The `visuals/` bundle belongs to the September 25, 20:46 UTC report. It is not current observational imagery. As documented in `visuals/VISUALS_SOURCE_README.md`, `01_extreme_core.png` includes an AI-generated conceptual illustration; the other figures are report-derived charts and diagrams. Consult their original source notes and labels.

This is not an official NHC/NOAA warning or emergency directive. Operational decisions require current official products.

## Integrity and continuity

`SHA256SUMS.txt` covers every packaged file except itself. After extraction, run `sha256sum -c SHA256SUMS.txt`. `PACKAGE_MANIFEST.json` records source ZIP identity, PDF inventory and release scope. `SOURCE_LINEAGE.json` points to the latest packaged state. Original superseded packaging metadata is retained under `provenance/input_metadata/`.

For future updates, append new scans without rewriting prior evidence. Update current-state pointers and regenerate manifest/checksums. Hashes establish byte identity, not the truth of weather claims.

## Download

[DI_Weather_Station_Polo_Nolo_2026-09-27_0816ET_FINAL.zip](DI_Weather_Station_Polo_Nolo_2026-09-27_0816ET_FINAL.zip)
