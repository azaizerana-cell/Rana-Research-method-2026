---
layout: post
title: "Relative Quantification of Gene Expression Using the ΔΔCt Method"
date: 2026-06-28
categories: [Research Methods, qPCR]
tags: [qPCR, Relative Quantification, Delta-Delta Ct, Gene Expression]
---

# Relative Quantification of Gene Expression Using the ΔΔCt Method

## Introduction

Quantitative real-time PCR (qPCR) is one of the most widely used techniques for measuring changes in gene expression. Unlike absolute quantification, relative quantification compares gene expression between experimental conditions after normalization to a stable reference (housekeeping) gene.

In this class exercise, gene expression was analyzed using the **ΔΔCt (Delta-Delta Ct) method**, also known as the **Livak method** (Livak & Schmittgen, 2001). This method compares the expression of target genes in inhibitor-treated samples relative to a DMSO control after normalization to the housekeeping gene **Tubulin**.

The analysis consisted of four sequential steps:

1. Measure Ct values.
2. Calculate ΔCt for each sample.
3. Calculate ΔΔCt between treatment and control.
4. Calculate Fold Change using the equation **2^-ΔΔCt**.

---

## ΔΔCt Analysis Workflow

The relative quantification workflow is summarized below:

**Step 1:** Measure Ct values for both the target gene and the reference gene.

↓

**Step 2:** Calculate ΔCt.

**ΔCt = Ct(Target Gene) − Ct(Reference Gene)**

↓

**Step 3:** Calculate ΔΔCt.

**ΔΔCt = ΔCt(Treatment) − ΔCt(Control)**

↓

**Step 4:** Calculate Fold Change.

**Fold Change = 2^-ΔΔCt**

↓

**Step 5:** Interpret gene expression changes.

- Fold Change > 1 → Gene is upregulated.
- Fold Change ≈ 1 → No substantial change in gene expression.
- Fold Change < 1 → Gene is downregulated.

---

## Class Data

The Ct (Cycle Threshold) values obtained during the qPCR experiment were provided during the class exercise and were used for all subsequent calculations.

**Table 1. Raw Ct (Cycle Threshold) Values for the Control and Inhibitor-Treated Samples**

![Table 1](/Rana-Research-method-2026/images/table1_qpcr.png)

---

## Step 1 – Calculate ΔCt

The ΔCt value normalizes each target gene to the reference gene (**Tubulin**), reducing technical variation between samples.

**Equation**

**ΔCt = Ct(Target Gene) − Ct(Reference Gene)**

### Example calculation (*NGN*)

**Control**

Ct(Target) = 28.35

Ct(Tubulin) = 23.30

ΔCt = 28.35 − 23.30 = **5.05**

**Treatment**

Ct(Target) = 27.35

Ct(Tubulin) = 23.30

ΔCt = 27.35 − 23.30 = **4.05**

---

## Step 2 – Calculate ΔΔCt

The ΔΔCt compares normalized gene expression between treatment and control.

**Equation**

**ΔΔCt = ΔCt(Treatment) − ΔCt(Control)**

### Example (*NGN*)

ΔΔCt = 4.05 − 5.05

ΔΔCt = **−1.00**

---

## Step 3 – Calculate Fold Change

Relative gene expression was calculated using the Livak equation.

**Equation**

**Fold Change = 2^-ΔΔCt**

### Example (*NGN*)

Fold Change = 2^-(-1.00)

Fold Change = **2.00**

This result indicates that **NGN** expression approximately doubled following inhibitor treatment.

---

## Calculation Results

All calculations were performed using Microsoft Excel, and numerical values were rounded to two decimal places for clarity and consistency.

**Table 2. ΔCt, ΔΔCt, and Fold Change Calculations for Relative Gene Expression**

![Table 2](/Rana-Research-method-2026/images/table2_qpcr.png)

---

## Interpretation of Fold Change

The Fold Change values can be interpreted as follows:

| Fold Change | Interpretation |
|-------------|---------------|
| > 1 | Gene is upregulated |
| ≈ 1 | No substantial change in expression |
| < 1 | Gene is downregulated |

---

## Data Interpretation

Figure 1 presents the relative expression of all analyzed genes after inhibitor treatment compared with the DMSO control.

![Figure 1](/Rana-Research-method-2026/images/foldchange_graph.png)

**Figure 1.** Relative gene expression (Fold Change) calculated using the **2^-ΔΔCt** method.

Genes with Fold Change values greater than 1 were upregulated following inhibitor treatment, whereas genes with values below 1 were downregulated.

Among the analyzed genes, **NGN** exhibited the highest increase in expression (Fold Change = 2.00), followed by **soxC**, **foxA**, and **ascs**. In contrast, **pitx** showed the strongest decrease in expression (Fold Change = 0.24), while **SM30**, **sm50**, and **opt** were also downregulated. Most of the remaining genes displayed relatively small changes in expression compared with the control, suggesting that the inhibitor produced gene-specific rather than uniform transcriptional responses.

---

## Conclusion

The ΔΔCt method provides a simple and reliable approach for relative gene expression analysis by normalizing target genes to a reference gene and comparing treated samples with a control.

In this class exercise, several genes responded differently to inhibitor treatment. **NGN** and **soxC** showed the greatest increase in expression, whereas **pitx**, **SM30**, and **sm50** exhibited the strongest decrease. Most of the remaining genes displayed relatively small changes relative to the control.

Because these data originated from a classroom exercise without biological replicates or statistical analysis, the results should be interpreted as an example of relative gene expression analysis rather than evidence of statistically significant differential gene expression.

---

## References

1. Livak KJ, Schmittgen TD. **Analysis of Relative Gene Expression Data Using Real-Time Quantitative PCR and the 2^-ΔΔCt Method.** *Methods*. 2001;25:402–408.

2. Applied Biosystems. **Guide to Performing Relative Quantitation of Gene Expression Using Real-Time Quantitative PCR.**
