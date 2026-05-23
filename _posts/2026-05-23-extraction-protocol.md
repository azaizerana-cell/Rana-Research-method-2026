---
layout: post
title: "Carbon uptake and metabolite extraction protocol in Prochlorococcus"
date: 2026-05-23
---

# Carbon uptake and metabolite extraction protocol in *Prochlorococcus*

## Experimental setup: carbon uptake and metabolites in *Prochlorococcus* under nitrogen starvation

This protocol aims to quantify **metabolic activity** and **nutrient uptake dynamics** in *Prochlorococcus* strain MED4 under nitrogen starvation.

The experiment combines stable isotope labeling with **NaH¹³CO₃**, metabolite extraction, and LC-MS/MS analysis. Cultures are grown to mid-exponential phase and exposed to NaH¹³CO₃ in order to track carbon incorporation into intracellular metabolites over time.

The protocol also aims to determine the timing of ¹³C incorporation into cells, characterize changes in the ¹³C/¹²C ratio over time, and identify the minimal sample volume that can be used without compromising analytical sensitivity or data quality.

<u>All work with chloroform and methanol must be performed under a chemical fume hood.</u>

---

## Background

### Biological reason

The original extraction protocol was developed for *Chlamydomonas reinhardtii*, which has a larger cell size and higher biomass than *Prochlorococcus*.

### Chemical reason

*Chlamydomonas reinhardtii* grows in freshwater, whereas *Prochlorococcus* grows in marine conditions. Therefore, salinity and osmotic conditions may affect metabolite extraction efficiency.

---

## Experimental design

Eighteen glass culture tubes of *Prochlorococcus* strain MED4 were grown in 25 mL culture volume.

For each tube, 1 mL of culture was transferred into 24 mL of Low Nitrogen 1/8 medium. Cultures were incubated until they reached the mid-exponential growth phase.

Date: 30/04/2026

### Culture tube organization

| Tube number | Sample name | ¹³C treatment | Time point | Replicate | Purpose |
|-------------|-------------|---------------|------------|-----------|---------|
| 1 | Control A | Without ¹³C | Control | A | Negative control |
| 2 | Control B | Without ¹³C | Control | B | Negative control |
| 3 | 0 H A | Without ¹³C | 0 H | A | Time-zero sample |
| 4 | 0 H B | Without ¹³C | 0 H | B | Time-zero sample |
| 5 | 2 H A | With ¹³C | 2 H | A | Labeling sample |
| 6 | 2 H B | With ¹³C | 2 H | B | Labeling sample |

---

## Figure

![Experimental setup]({{ site.baseurl }}/images/experimental_setup.jpg)

Figure 1: Experimental setup and sample organization for the ¹³C labeling experiment in *Prochlorococcus* MED4.

---

## ¹³C labeling experiment

On 5/5/2026, once the cultures reached the mid-exponential phase, culture tubes 5–16 received 25 µL of NaH¹³CO₃.

Samples were collected at different time points:

- 0 H
- 2 H
- 4 H
- 6 H
- 10 H
- 12 H
- 24 H

For flow cytometry analysis, 100 µL of culture was mixed with 900 µL of filtered seawater and fixed with 5 µL of glutaraldehyde.

In parallel, samples 3–16 were filtered onto GF/F filters at the different time points. The filters were stored in 1 mL MeOH at −80°C.

Samples 17 and 18 were used as efficiency controls. They were filtered onto GF/F filters and stored in 1 mL seawater at −80°C.

---

## Additional flask experiment

In addition to the 18 glass tubes, two 200 mL flasks of *Prochlorococcus* strain MED4 were grown in Low Nitrogen 1/8 medium.

For each 200 mL flask, 10 mL of culture was transferred into 190 mL medium.

The two flasks were named:

- Flask cell culture A
- Flask cell culture B

Samples were filtered onto GF/F filters using different culture volumes:

- 10 mL
- 25 mL
- 50 mL
- 75 mL

The filters were stored in 1 mL MeOH at −80°C.

---

## Important experimental note

The 12-hour time point and one replicate from the DDW control were omitted because a new fresh NaH¹³CO₃ solution was prepared.

The first NaH¹³CO₃ solution was suspected to have been prepared incorrectly in terms of volumes. In addition, during the additions, the remaining volume was not sufficient for all samples.

As a result:

- Tubes 13 and 14 became tubes 5 and 6.
- Tube 17 became tube 7.

The positive controls included two replicate tubes from the 24-hour time point that received NaH¹³CO₃, as well as two non-filtered control cultures supplemented with NaH¹³CO₃.

The negative controls consisted of two tubes filtered at time zero that did not receive NaH¹³CO₃.

During filtration, light intensity should be maintained similar to the growth conditions of the cells in order to minimize physiological stress.

---

# Flow cytometry measurement

Before measurement, the bacterial culture was diluted again 10-fold with seawater, resulting in a final dilution of 1:100.

The flow cytometry plate included:

- B = Cleaning agent, 250 µL
- D = DDW, 250 µL
- SW = Seawater, 200 µL
- Bacterial culture, 200 µL

In addition, 1 µL of BIDAS was added to the bacterial culture and seawater mixture.

---

# Table of materials required for preparation

| Material | Volume | Amount | Temperature | Purpose | Notes |
|----------|--------|--------|-------------|---------|-------|
| Low Nitrogen 1/8 medium | 24 mL | 18 tubes | 20–25°C | Culture growth | Marine medium |
| *Prochlorococcus* MED4 culture | 1 mL | 18 tubes | 20–25°C | Inoculation | Mid-exponential phase |
| NaH¹³CO₃ | 25 µL | Samples 5–16 | Room temperature | ¹³C labeling | Carbon uptake tracking |
| Filtered seawater | 900 µL | Per FC sample | Room temperature | Dilution | Used for flow cytometry |
| Methanol | 1 mL | Per filter | −80°C | Quenching | Absolute MeOH |
| GF/F filters | 1 filter | Per sample | −80°C storage | Cell collection | Stored in MeOH |

---

# Extraction protocol of metabolites for LC-MS/MS measurements from *Prochlorococcus*

This protocol is an updated extraction protocol adapted from metabolite extraction for *Chlamydomonas reinhardtii* to metabolite extraction for *Prochlorococcus*.

## Quenching

25 mL culture was filtered through a GF/F filter in absolute MeOH and stored at −80°C until further use.

> **Note:** In the previous protocol, 46% MeOH was used. However, for our bacterial system this condition may need to be adjusted, and absolute MeOH may be more appropriate.

---

# Opening cells by freeze–thaw cycles

Date: 12.5.2026

1. Precool chloroform stock at −20°C.

2. Defrost quenched material at −20°C and then place on ice.

3. Add 200 µL chloroform to 1000 µL sample.

4. Vortex vigorously for 10 seconds for each sample.

Total volume per sample:

1200 µL

Calculation:

x = (1000 µL × 105 µL) / 525 µL = 200 µL

5. Place samples at −20°C for 1 hour.

6. Freeze samples in liquid nitrogen and store at −80°C for 2 hours.

7. Defrost samples on ice for 15 minutes.

8. Vortex vigorously for 15 seconds for each sample.

9. Freeze again at −80°C.

10. Repeat the freeze–thaw cycle three times.

> **Note:** Freezing samples at −80°C takes approximately one hour. Therefore, the freeze–thaw cycles were usually performed on the first day, and the extraction was performed on the second day.

11. Store samples overnight at −80°C.

> **Observation:** After three freeze–thaw cycles, green pigment was observed in the lower chloroform phase.

---

# Chloroform / MeOH / precooled ddH₂O extraction

Date: 13.5.2026

1. Defrost samples on ice for 15 minutes.

2. Remove the filters.

3. Place the filters on a white A4 sheet for visual comparison.

> **Note:** During filter removal, some loss of material may occur. Therefore, not all metabolites of interest are necessarily transferred into the extraction solution. Extraction efficiency is not 100%.

4. Add 533 µL precooled ddH₂O.

5. Vortex.

Calculation:

x = (1200 µL × 280 µL) / 630 µL = 533 µL

Total volume per sample:

1733 µL

6. Centrifuge for 5 minutes at 14000 rpm and 4°C.

7. Collect 1400 µL of the ddH₂O/MeOH upper phase into a new Eppendorf tube. This is the first extraction replicate.

Calculation:

x = (1733 µL × 800 µL) / 910 µL = 1523 µL ≈ 1400 µL

Additional precooled water:

(280 µL × 1400 µL) / 960 µL ≈ 410 µL

8. Add 410 µL ddH₂O to the new Eppendorf tube.

9. Close the tube using punctured caps.

Final volume of the first extraction replicate:

1810 µL

Remaining old sample volume:

333 µL

---

# Second extraction replicate

1. Add 1070 µL precooled ddH₂O to the remaining chloroform phase.

2. Vortex.

Calculation:

x = (560 µL × 210 µL) / 110 µL = 1070 µL

Total volume:

1403 µL

3. Centrifuge for 5 minutes at 14000 rpm and 4°C.

4. Collect 1070 µL of the upper phase into a new Eppendorf tube. This is the second extraction replicate.

Additional precooled water:

(280 µL × 1070 µL) / 960 µL ≈ 310 µL

5. Add 310 µL ddH₂O to the Eppendorf tube.

6. Close the tube using punctured caps.

Final volume of the second extraction replicate:

1380 µL

Remaining old sample volume:

333 µL

---

# Third extraction replicate

1. Repeat the previous extraction step using the remaining chloroform phase.

2. Centrifuge for 5 minutes at 14000 rpm and 4°C.

3. Collect 1070 µL of the upper phase into a new Eppendorf tube. This is the third extraction replicate.

Additional precooled water:

(280 µL × 1070 µL) / 960 µL ≈ 310 µL

4. Add 310 µL ddH₂O to the Eppendorf tube.

5. Close the tube using punctured caps.

Final volume of the third extraction replicate:

1380 µL

Remaining old sample volume:

333 µL

---

# Experimental notes

> **Note:** In the previous experiment, during steps 1–8, the filters were not removed initially because this step was unintentionally missed. Therefore, an additional step was introduced: the material was detached from the filters, followed by vortexing and centrifugation. Subsequently, 1070 µL of the upper phase was collected.

> **Note:** Incomplete phase separation was observed in one Eppendorf tube, which contained visible filter residues and pellet material.

> **Note:** The addition of water prevents bubbling during freeze-drying.

At this stage, three extraction samples are present with the following volumes:

- 1810 µL
- 1380 µL
- 1380 µL

---

# Freeze drying

1. Store samples at −80°C for 1 hour.

2. Freeze-dry samples overnight.

---

# Storage

Date: 14.5.2026

After freeze-drying, samples were removed, wrapped with parafilm, and stored at −80°C.

---

# LC-MS/MS sample organization

| Sample group | Flow cytometry sample | Filtered sample | Extraction replicate 1 | Extraction replicate 2 | Extraction replicate 3 |
|--------------|----------------------|-----------------|------------------------|------------------------|------------------------|
| 0 H A | 0 H A-FC | 3-0 H A-PE | 0 H A-E1 | 0 H A-E2 | 0 H A-E3 |
| 0 H B | 0 H B-FC | 4-0 H B-PE | 0 H B-E1 | 0 H B-E2 | 0 H B-E3 |
| 2 H A | 2 H A-FC | 5-2 H A-PE | 2 H A-E1 | 2 H A-E2 | 2 H A-E3 |
| 2 H B | 2 H B-FC | 6-2 H B-PE | 2 H B-E1 | 2 H B-E2 | 2 H B-E3 |
| 4 H A | 4 H A-FC | 7-4 H A-PE | 4 H A-E1 | 4 H A-E2 | 4 H A-E3 |
| 4 H B | 4 H B-FC | 8-4 H B-PE | 4 H B-E1 | 4 H B-E2 | 4 H B-E3 |

---

# Scientific references

- [Partensky et al. 1999 — *Prochlorococcus*, a marine photosynthetic prokaryote of global significance](https://www.microbiologyresearch.org/content/journal/micro/10.1099/00221287-145-8-1931)

- [Biller et al. 2015 — *Prochlorococcus*: the structure and function of collective diversity](https://www.nature.com/articles/nrmicro3378)

---

# Online protocol and instrument references

- [LC-MS/MS overview — Thermo Fisher Scientific](https://www.thermofisher.com/il/en/home/industrial/mass-spectrometry/liquid-chromatography-mass-spectrometry-lc-ms.html)

- [TRIzol reagent protocol — Thermo Fisher Scientific](https://assets.thermofisher.com/TFS-Assets/LSG/manuals/trizol_reagent.pdf)

---

# Summary

This protocol describes an adapted metabolite extraction workflow for *Prochlorococcus* MED4 under nitrogen starvation. It combines ¹³C labeling, flow cytometry, GF/F filtration, methanol quenching, chloroform–methanol–water extraction, freeze–thaw cycles, lyophilization, and LC-MS/MS analysis.

The workflow is designed to study carbon incorporation into intracellular metabolites and to evaluate how sample volume and extraction efficiency affect downstream LC-MS/MS measurements.