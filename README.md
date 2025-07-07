 
# Capability Indices in Statistical Quality Control

This repository contains the final project for the course **Statistical Quality Control** at the Europa-Univärsitet Viadrina. The work combines theoretical depth with practical implementation in **R**, using real process data to analyze and visualize **process capability indices (PCIs)**.

## Author
**Anastasiia Apatenko**  
Date of completion: June 23, 2025

## Project Description

The paper explores the role of **process capability indices** such as:

- **Cp** – Basic process spread
- **Cpk** – Considers process centering
- **Cpm** – Introduces the target value (Taguchi loss function)
- **Cpmk** – Combines centering and target deviation
- **k index** – Measures process centering separately

It includes both:
- A detailed **literature-based theoretical foundation** (Six Sigma, Taguchi loss, bias/variance effects),
- A **practical implementation in R**, including custom functions and visualizations.

---

## Tools & Libraries

- **R** libraries used for statistical computing:
  - `qcc` – for control charts and capability analysis
  - `SixSigma` – for dataset and process data
  - Base R (`shapiro.test`, `mean`, etc.)

---

## Files Included

| File | Description |
|------|-------------|
| `theoretical-part.pdf` | Full paper with theoretical background and practical analysis |
| `practical-part.pdf` | Extracted and annotated version of the R-based practical section |


---

## Highlights of the Practical Work

- Used `ss.data.bolts` dataset (50 bolt diameters) from the `SixSigma` R package.
- Verified all four PCI assumptions:
  - Normality (via Shapiro-Wilk test)
  - Statistical control (via `qcc` charts)
  - Centered process mean (𝜇 = 𝑚)
  - Target value located at midpoint (𝑇 = 𝑚)
- Calculated Cp, Cpk, Cpm, Cpmk using both package tools and **custom R functions**.
- Demonstrated how changes in process variation and target location affect capability indices.

---

## Key Insights

- All initial indices (Cp, Cpk, Cpm, Cpmk) ≈ 1 → meets **minimum quality standards**.
- Widening specification limits can **increase capability** (to 1.33 or 2.0) but is **not a valid real-world strategy**.
- The **Cpmk index** was computed manually and shown to drop significantly when target shifts from center.
- Emphasized the importance of checking all PCI assumptions before applying capability analysis.

---

## Conclusion

This project highlights the **importance and limitations of capability indices** in quality control. It combines **mathematical rigor with practical R implementation**, making it a useful reference for both academic and industrial contexts.

---


