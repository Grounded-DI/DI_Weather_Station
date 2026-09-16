# DI Weather Station — Deterministic Weather and Corridor Analysis Record

A public Grounded DI LLC archive of StormWise / DI Weather Station scans, event audits, forecast comparisons, formulas, and dated weather observations.

## Overview

This repository preserves 20 public artifacts spanning April 17, 2025 through July 31, 2026. The repository itself was created on April 5, 2026; the dates in the collection belong to the individual forecasts, observations, reports, and public-record captures.

The collection documents a weather-control vocabulary built around local corridors, temporal windows, visual and radar signals, explicit thresholds, binary decisions, and evidence-preserving work products. It includes both contemporaneous case records and later audit documents. The original StormWise and DI² terminology is retained as part of that history.

This is an artifact archive, not the complete weather runtime. It gives a reviewer a dated record of the recorded control paths, their outputs, and the boundaries each artifact states.

## Why It Matters

Weather decisions often depend on a place, a time window, and a practical threshold rather than a county-wide percentage. The records in this repository show how a localized event can be framed as a testable decision: define the endpoint, preserve the pre-event forecast, compare it with observations, and record what passed, what was partial, and what remained unresolved.

## What the Repository Contains

| Collection | Representative files | Record type |
| --- | --- | --- |
| Event audits | `StormWise_DI2_West_Chester_PA_4-4-26_Audit_SHA.pdf`, `DI_Weather_Station_Audit_West_Chester_Area_July_18_2026.pdf`, `DI2_Weather_Station_Belmar_Beach_Cloud_Cover_Decision_Audit_2026-07-31.pdf` | Chronological forecast-to-observation assessments |
| Sealed work products | `StormWise_Artifact_Spring_Convective_Microcell_Passage_Cherry_Hill_4-20-26.pdf`, `StormWise_Spring_Convection_Boundary_Test.pdf` | DWP-style weather artifacts with constraints, outputs, and verification blocks |
| Forecast and observation records | `Snow_Scan_Ideal_Forecast_19341_PA_Jan_17_2026_with_Appendix.pdf`, `Spring_Rain_Scan_5-10-26_PA.pdf`, `StormWise_Proof_Jan_2026_Philly.pdf` | Dated snow, rain, and corridor scans |
| Visual/public records | `DI_Weather_Station_Spring_Temporal_Precision_Rain_Event_PA.jpeg`, `Hyper_Local_High_Temperature_Forecast_Direct_Hit.jpg`, `DI_Weather_Map_of_Public_Forecast_Delta_PA_1-22-2026 copy.png` | Forecast cards, screenshots, and comparison graphics |
| Historical and research records | `Case004_The_555_Trigger_8-13-2025.md`, `Blizzard_Season_Intro_10-18-2025.pdf`, `DI_Weather_Station_Category_6_Hurricane_Proposed_Formula_and_Calculation.pdf` | Contemporaneous case language, season introduction, and a proposed compound-risk formula |

## What the Record Demonstrates

The statuses below are the statuses recorded inside the named artifacts. They describe those events and documents; they are not a claim of model-wide weather performance.

| Artifact | Recorded result |
| --- | --- |
| `StormWise_Artifact_Spring_Convective_Microcell_Passage_Cherry_Hill_4-20-26.pdf` | Arrival window **3–10 minutes**; observed arrival **6–8 minutes**. Duration window **5–15 minutes**; observed duration **about 14–15 minutes**. The artifact records **Full deterministic validation (timing + duration)**, with morphology, radar alignment, edge fragmentation, timing, duration, and severe-structure checks marked `PASS`; energy continuity is `PARTIAL`. Final output: `RAIN EVENT — VERIFIED`. |
| `StormWise_DI2_West_Chester_PA_4-4-26_Audit_SHA.pdf` | Scan at **1:46 PM** followed by direct onset evidence at approximately **1:50 PM**, inside the stated `T+0–10` leading-edge window. The audit records a 3–4 minute error margin for this event and preserves archive hash `69197694b6e4516043a87e16baa9609fbc3e8a8eb94c0e11588074397e321235`. |
| `Snow_Scan_Ideal_Forecast_19341_PA_Jan_17_2026_with_Appendix.pdf` | Exton, PA: recorded forecast range **1.0–1.3 inches**; measured total **1.3 inches**. The artifact states the range was met with no audit violations and marks the work product `FINAL/SEALED`. |
| `StormWise_Spring_Convection_Boundary_Test.pdf` | A borderline convection scan recorded tracking value **13%** and output `RAIN EVENT — NO`. Morphology and clustering are `PASS`; vertical growth is `PARTIAL`; radar and energy continuity are `FAIL`; the documented rule path downgraded the initial signal after radar non-confirmation. |
| `DI_Weather_Station_Audit_West_Chester_Area_July_18_2026.pdf` | Day-scale updated forecast: `VERIFIED`. First visible local drops at **12:47 PM EDT**: `VERIFIED`. Broad 2–7 PM window: `PARTIALLY VERIFIED`; first measurable rainfall: `UNRESOLVED`; audit integrity: `VERIFIED`. |
| `DI2_Weather_Station_Belmar_Beach_Cloud_Cover_Decision_Audit_2026-07-31.pdf` | The pre-event `GO` decision is `VERIFIED`; peak timing is `SUPPORTED`; exact 52% peak magnitude is `PARTIALLY VERIFIED`; literal proof that the peak stayed below 60% is `UNRESOLVED`. The document explicitly treats the operational decision as the consequential endpoint. |
| `Case004_The_555_Trigger_8-13-2025.md` | A contemporaneous StormWise case record states that risk moved from **75% to 85% by 4:23 PM** and that rain arrived at **5:55 PM**. It is preserved as a dated case narrative, not as a multi-event benchmark. |
| `DI_Weather_Station_Category_6_Hurricane_Proposed_Formula_and_Calculation.pdf` | A research artifact calculates `CFRI = 179.625` against a **proposed** threshold of `178.0`. It expressly states that this is not an official NHC wind-category designation. |

## Recorded Control Model

Across the sealed work products, the documented execution pattern is:

```text
local observations and forecast context
        → visual / radar / temporal signal extraction
        → constraints and threshold checks
        → event classification or GO / NO-GO routing
        → timestamped, sealed, or audit-preserved record
```

The artifacts use terms such as `Scroll-Sealed`, `Entropy`, `DriftIndex`, `FastPath`, and `Tier`. These are project terms preserved from the source documents. They should be read together with each artifact's own verification block and scope statement.

## Technical Highlights

- Event-specific endpoints are separated: day, window, first visible drop, measurable rain, clearing, and decision outcome are not collapsed into one score.
- Forecasts and observations remain separate records; the July 18 audit explicitly preserves the original Friday forecast alongside the later Saturday diagnostic.
- Several work products record explicit constraints, threshold routing, artifact IDs, replay keys, entropy bands, drift fields, and evidence registers.
- The April 4 West Chester audit links a near-term scan to a timestamped image sequence and a stated archive hash.
- The Cherry Hill artifact records both timing and duration windows, rather than only an event/no-event label.

## How to Review

For the clearest evidence path, start with:

1. `StormWise_Artifact_Spring_Convective_Microcell_Passage_Cherry_Hill_4-20-26.pdf` — sealed timing-and-duration work product.
2. `StormWise_DI2_West_Chester_PA_4-4-26_Audit_SHA.pdf` — same-day onset sequence and archive hash.
3. `DI_Weather_Station_Audit_West_Chester_Area_July_18_2026.pdf` — forecast revision and endpoint-specific status language.
4. `DI2_Weather_Station_Belmar_Beach_Cloud_Cover_Decision_Audit_2026-07-31.pdf` — threshold decision with exact-value restraint.
5. `Case004_The_555_Trigger_8-13-2025.md` and the visual records — early public terminology and contemporaneous examples.

## Validation and Testing

No executable source tree, package manifest, or test harness is included in this repository, so there is no repository test command to run. `PASS`, `VERIFIED`, `PARTIALLY VERIFIED`, `SUPPORTED`, and `UNRESOLVED` below are the classifications printed by the individual artifacts. The repository does not independently rerun the weather analyses or supply a sensor-feed replay environment.

The strongest checks are therefore the recorded event-specific checks: the Cherry Hill timing and duration pass, the West Chester April onset window, the January snow-range match, and the endpoint-separated July audits.

## Commercial and Integration Context

The archive can support technical evaluation or a proof-of-concept discussion around localized weather-event monitoring, corridor-specific risk decisions, forecast quality review, and evidence-preserving operational reports. Any production integration would require a separate runtime, data-source agreements, validation plan, and domain review.

Evaluation, licensing, integration, and research inquiries can be opened through the [Grounded DI GitHub organization](https://github.com/Grounded-DI).

## Authorship and Provenance

The artifacts identify Grounded DI LLC and, in the August 2025 case record, Mark Weinstein as operator. The repository preserves dated PDFs, images, screenshots, artifact IDs, and source-bound evidence registers. A file hash identifies the bytes to which it is applied; it does not independently establish the substantive truth of every statement in those bytes.

## Repository Scope

This repository is a public documentary and demonstration record. It is not the complete private implementation, weather-data pipeline, SDK, sensor integration, or validation environment. Results are event-specific. The artifacts themselves identify where exact measurements, broader calibration, measurable rainfall, or universal forecasting skill remain unresolved.

No open-source license is currently provided in this repository. Copyright and other rights remain with Grounded DI LLC and applicable authors except where expressly stated otherwise.

## Status

The repository is an expanding public artifact archive. Its strongest evidence consists of dated event records and sealed work products; it should not be read as a claim that a complete production weather service is distributed here.

## Contact

Use the [Grounded DI GitHub organization](https://github.com/Grounded-DI) for collaboration, evaluation, licensing, or integration inquiries.
