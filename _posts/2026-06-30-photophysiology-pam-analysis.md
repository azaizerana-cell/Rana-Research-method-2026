---
layout: post
title: "Photophysiological Analysis of Marine Macroalgae Collected from the Rocky Shore at Sdot Yam"
date: 2026-06-30
categories: [Research Methods, Photophysiology]
tags: [PAM Fluorometry, Macroalgae, Marine Biology, Photosynthesis, R]
---

# Photophysiological Analysis of Marine Macroalgae Collected  from the Rocky Shore  at Sdot Yam

## Aim

The aim of this exercise was to survey marine macroalgal communities in the shallow rocky shore at Sdot Yam, estimate the relative abundance and percent cover of algal species along different transects, and collect representative specimens for photophysiological measurements. The collected photophysiological data were subsequently analyzed to examine variation among the sampled algal species and to provide preliminary insight into how habitat may influence algal photophysiology.

---
## Study Species

The practical exercise focused on common marine macroalgae collected from the shallow rocky shore at Sdot Yam. The field identification guide provided during the course was used to assist species identification during sampling and subsequent laboratory analyses.




The practical exercise focused on common marine macroalgae collected from the shallow rocky shore at Sdot Yam. The field identification guide provided during the course was used to assist species identification during sampling and subsequent laboratory analyses.

![](/images/experimental_setup2.jpeg)
![](/Rana-Research-method-2026/images/experimental_setup2.jpeg)


**Figure1.** Representative macroalgal species included in the field identification guide provided during the practical course. The guide was used to assist species identification during field sampling at the Sdot Yam rocky shore.

## Experimental Design

The study combined a field survey with laboratory-based photophysiological measurements. Students were divided into four groups of three to four participants, and each group surveyed a different transect orientation (North–South, South–North, East–West, or West–East) along the shallow rocky shore at Sdot Yam. A measuring tape approximately 40 m long was deployed along each transect, and sampling was performed every 5 m using a 0.5 × 0.5 m quadrat.

Within each quadrat, the percent cover of algal species and other visible substrates was visually estimated and recorded. Representative algal specimens were collected from the surveyed area for subsequent laboratory measurements. Following the field survey, the observations from all groups were combined into a single dataset that was used for data organization and analysis.

---

# Materials and Methods

## Sampling

Field sampling was conducted at the shallow rocky shore of Sdot Yam. Four transects representing different directions were surveyed. A 0.5 × 0.5 m quadrat was placed every 5 m along each transect, and the percent cover of algal species and other visible substrates (e.g., rock and sand) was visually estimated and recorded on waterproof data sheets. Representative algal specimens were collected manually, labeled, and transported to the laboratory in buckets containing seawater.

## Species Identification

Algal specimens were identified using the field identification guide provided during the course. When species identification could not be completed in the field, specimens were documented and identified later using the same identification resources.

## Laboratory Procedures

After transportation to the laboratory, the collected algal specimens were maintained in seawater until photophysiological measurements were performed. Each specimen was measured according to the laboratory protocol provided during the practical exercise.

## PAM Measurements

Photophysiological measurements were performed using a PAM fluorometer. Both the Light and Dark measurement protocols were applied according to the laboratory protocol. Four photophysiological parameters were estimated from the fitted photosynthesis–irradiance (P–I) curves:

- **Am** – maximum electron transport rate (ETRmax)
- **AQY** – apparent quantum yield (initial slope of the light-response curve)
- **Rd** – dark respiration (curve intercept)
- **Ik** – saturation irradiance, calculated as Am/AQY

These parameters were used for subsequent statistical analyses.

## Data Analysis (R)

All data analyses were performed in **R (RStudio)** using the script provided during the practical exercise. The working directory was set to the folder containing the metadata and photophysiology data files (**light.csv**, **dark.csv**, and **Photophysiology_metadata.csv**). The required R packages included **dplyr, tidyr, lubridate, hms, ggplot2, purrr, broom,** and **patchwork**.

The metadata and photophysiology datasets were imported into R and inspected to verify their structure and formatting. Date and time variables were converted to appropriate formats using the **lubridate** and **hms** packages. Electron transport rate (ETR) measurements were transformed from wide to long format using **pivot_longer()**, allowing subsequent statistical analyses and visualization. Metadata, including sample identity and taxonomic classification, were matched to each measurement.

Initial quality-control plots were generated to inspect the photosynthesis–irradiance (P–I) curves. Zero ETR values recorded after illumination had begun (PAR > 0), which represented the end of measurements rather than biological observations, were replaced with missing values (NA). Two Light samples (**Light_3** and **Light_9**) showing incomplete or poor-quality response curves were excluded from the Light dataset before curve fitting, following the practical protocol.

Photosynthesis–irradiance (P–I) curves were fitted using nonlinear least-squares (NLS) regression. The fitted curves were plotted together with the measured data for both the Light and Dark treatment groups. Estimated photophysiological parameters for each sample were exported as CSV files (**light_group_photo_parameters.csv** and **dark_group_photo_parameters.csv**). The combined P–I curves were exported as **Figure1_PI_curves.png**.

The parameter estimates from both treatment groups were merged into a single dataset. Descriptive statistics, including sample size (n), mean, standard deviation, minimum, first quartile, median, third quartile, and maximum, were calculated for each photophysiological parameter. The summary table was exported as **Table2_Photophysiology_parameters.csv**.

Data distributions were evaluated using Q–Q plots. Boxplots were generated to compare the Light and Dark treatment groups for each photophysiological parameter, and the final figure was exported as **Figure2_Boxplots.png**. Additional figures comparing parameter differences and Light/Dark ratios among algal taxa were also generated for exploratory analysis.

Finally, paired comparisons between Light and Dark measurements were performed using the paired Wilcoxon signed-rank test. To account for multiple testing, p-values were adjusted using the Benjamini–Hochberg (BH) correction.

### R Script

The complete R script used for data import, preprocessing, quality control, curve fitting, statistical analyses, figure generation, and automatic export of tables and figures is provided in the supplementary materials.

---
# Results

The results obtained from the photophysiological analyses are presented in the following tables and figures.

---

## Table 1. Metadata


**Table 1.** Metadata describing all algal samples included in the experiment. The table presents the experimental treatment (Light or Dark), sample number, taxonomic identification, and the corresponding Sample ID used throughout the analysi
=======
**Table 1.** Metadata describing all algal samples included in the experiment. The table presents the experimental treatment (Light or Dark), sample number, taxonomic identification, and the corresponding Sample ID used throughout the analysis.

![](/images/Table1_Metadata.png)
![](/Rana-Research-method-2026/images/Table1_Metadata.png)


---

## Table 2. Photophysiology Parameters

**Table 2.** Summary statistics of the estimated photophysiological parameters for the Light and Dark treatment groups. For each parameter (Am, AQY, Ik, and Rd), the table reports the sample size (n), mean, standard deviation (SD), minimum, first quartile (Q25), median, third quartile (Q75), and maximum values.

The summary statistics indicate differences between the Light and Dark treatment groups across all four photophysiological parameters. The Light treatment generally exhibited higher Am and Ik values, whereas AQY and Rd showed treatment-dependent variation.

![](/images/Table2_Photophysiology_Parameters.png)
![](/Rana-Research-method-2026/images/Table2_Photophysiology_Parameters.png)


---

## Figure 2. Photosynthesis–Irradiance (P–I) Curves

**Figure 2.** Photosynthesis–irradiance (P–I) curves for algal samples from the Light and Dark treatment groups. Points represent the measured electron transport rate (ETR) values at different irradiance (PAR) levels, while the solid lines represent the nonlinear least-squares (NLS) fitted curves used to estimate the photophysiological parameters.

The fitted curves show the expected increase in electron transport rate with increasing irradiance until saturation is reached. Differences in curve shape and maximum ETR are evident among algal taxa and between the Light and Dark treatment groups.

![](/images/figure1_PI_curves.png)
![](/Rana-Research-method-2026/images/figure1_PI_curves.png)

---

## Figure 3. Comparison of Photophysiological Parameters

**Figure 3.** Boxplots comparing the estimated photophysiological parameters (Am, AQY, Ik, and Rd) between the Light and Dark treatment groups. Colored points represent the individual algal taxa included in the paired analysis.

The distributions indicate variation in all four photophysiological parameters between treatments. Overall, the Light group tended to show higher values of Am and Ik, while AQY and Rd displayed different responses among taxa. These results provide an overview of the variability in photophysiological performance under the two experimental conditions.


![](/images/Figure2_Boxplots.png)
![](/Rana-Research-method-2026/images/Figure2_Boxplots.png)
## 6. Interpretation / Discussion

The photophysiological analyses revealed measurable differences between macroalgae exposed to the Light and Dark treatments. The fitted photosynthesis–irradiance (P–I) curves showed the expected increase in electron transport rate (ETR) with increasing irradiance, followed by saturation at higher light intensities.

The estimated photophysiological parameters indicated treatment-dependent variation. Overall, the Light treatment exhibited higher values of **Am** and **Ik**, suggesting greater maximum electron transport capacity and higher irradiance requirements for photosynthetic saturation. In contrast, **AQY** and **Rd** displayed more variable responses among taxa, indicating that photosynthetic efficiency and respiration differed between species and were influenced by the treatment conditions.

Substantial variability was observed among the algal taxa, reflecting species-specific physiological adaptations to different light environments. Such variability is expected because macroalgal species differ in their photosynthetic strategies, pigment composition, and ecological niches.

Although this practical exercise was based on a relatively small number of samples, the workflow successfully demonstrated how nonlinear curve fitting and statistical analyses can be used to estimate biologically meaningful photophysiological parameters and compare treatments in a reproducible manner.

---

## 7. Conclusion

This practical exercise demonstrated how R can be used to analyze photophysiological data obtained from PAM fluorometry. The workflow included data import, preprocessing, quality control, nonlinear curve fitting, statistical analysis, and graphical visualization of the results.

The analysis showed that the Light and Dark treatments differed in several photophysiological parameters, with the Light treatment generally exhibiting higher **Am** and **Ik** values, while **AQY** and **Rd** varied among algal taxa and treatments. These results illustrate how differences in light conditions can influence photosynthetic performance in marine macroalgae.

Beyond the biological findings, this exercise provided practical experience in reproducible data analysis using R. The complete workflow—from raw measurements to summary tables, statistical analyses, and publication-quality figures—demonstrates how computational tools can be integrated into marine photophysiological research.
## 8. Supplementary Files

The following supplementary files are provided together with this report.

### CSV Files

- **Photophysiology_metadata.csv** – Metadata describing all algal samples included in the study.
- **light.csv** – Raw photophysiology measurements collected using the Light protocol.
- **dark.csv** – Raw photophysiology measurements collected using the Dark protocol.

### Excel File with ReadMe

- **Photophysiology_2026.xlsx** – Excel workbook containing the organized photophysiology dataset and a **ReadMe** worksheet describing all measured parameters, their definitions, and measurement units.

### R Script

- **Photophysiology_2026.R** – Complete R script used for data import, preprocessing, quality control, nonlinear curve fitting, statistical analyses, generation of summary tables, and export of figures.
