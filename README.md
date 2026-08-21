# ☀️ Techno-Economic Design & Simulation of a 5 MWp PV + BESS Utility-Scale Plant

[![PVsyst](https://img.shields.io/badge/Simulation-PVsyst_v7.4-blue.svg)](https://www.pvsyst.com/)
[![Documentation](https://img.shields.io/badge/Report-LaTeX%20%2F%20XeLaTeX-green.svg)]()
[![Author](https://img.shields.io/badge/Author-Konstantinos_Xirogiannis-orange.svg)](https://www.linkedin.com/in/konstantinosxirogian/)

> **Comprehensive engineering study and financial assessment of a 5.03 MWp grid-connected PV plant equipped with a 3.84 MWh Battery Energy Storage System (BESS) under grid injection constraints in Thessaly, Greece.**

---

## 📑 Direct Documentation Links

* 📄 **[Download Full Engineering Report (PDF)](./Final%20Report.pdf)**
* 📊 **[Download PVsyst Simulation Summary (PDF)](./PVsyst_Report_5MWp.pdf)**

---

## 📌 Executive Summary

This project investigates the techno-economic optimization of a **5.03 MWp utility-scale solar PV plant** located in **Karditsa, Greece**. With grid congestion leading to strict injection limits (curtailments), the study evaluates the integration of a **behind-the-meter industrial Battery Energy Storage System (BESS)** operating under a **Peak Shaving** strategy.

The analysis transitions from an initial theoretical baseline scenario to a fully realistic model incorporating **3D Near Shadings (Linear)**, **Detailed Thermal/Ohmic Losses**, and **Project Financing (PPA vs Merchant sensitivity)**.

---

## ⚙️ Key Technical Specifications

| Parameter | Specification | Details |
| :--- | :--- | :--- |
| **Location** | Karditsa, Thessaly, Greece | Lat: $39.36^\circ\text{N}$, Lon: $21.92^\circ\text{E}$, Alt: 102 m |
| **Nominal DC Power** | **5,028 kWp** | 8,450 $\times$ JinkoSolar 595 Wp (JKM-595N-72HL4-V) |
| **Nominal AC Power** | **3,850 kWac** | 13 $\times$ Huawei SUN2000-300KTL-H0 (300 kW string inverters) |
| **DC/AC Overload Ratio** | **1.306** | Overload clipping loss limited to 0.4% |
| **Orientation & Tilt** | Fixed Tilted Plane | Tilt: $30^\circ$, Azimuth: $0^\circ$ (South) |
| **BESS Capacity** | **3.84 MWh (usable)** | LiFePO4 (LFP), 6,250 Ah @ 768 V, 80% DOD (20%–95% SOC) |
| **Grid Power Limit** | **3.50 MW** | Applied at Global Injection Point (Peak Shaving) |

---

## 📊 Comparative Performance & Financial KPIs

| Metric | Base Case (VC0 - Theoretical) | PV + BESS (VC1 - Theoretical) | **PV + BESS (VC1 - Realistic + 3D)** |
| :--- | :---: | :---: | :---: |
| **Annual Energy Yield** | 7,730 MWh/yr | 7,698 MWh/yr | **7,333 MWh/yr** |
| **Specific Production** | 1,538 kWh/kWp/yr | 1,531 kWh/kWp/yr | **1,458 kWh/kWp/yr** |
| **Performance Ratio (PR)**| 87.3% | 87.0% | **82.9%** |
| **Total CAPEX** | €2.94M | €4.04M | **€4.04M** |
| **Levelized Cost (LCOE)** | €0.0403/kWh | €0.0608/kWh | **€0.0705/kWh** |
| **Net Present Value (NPV)**| €2.72M | €1.15M | **€405,404** |
| **IRR (Equity)** | 29.9% | 13.24% | **8.61%** |
| **Payback Period** | 9.5 years | 14.5 years | **18.8 years** |

---

## 🛠️ Visual Highlights

### 1. 3D Scene & Shading Modeling
13 sheds $\times$ 650 modules (2 portrait $\times$ 325) with an 11.0 m pitch spacing to optimize land use while keeping inter-row shading losses minimal.

<p align="center">
  <img src="figures/shadings_3d_view.png" alt="3D Shading Scene" width="75%">
</p>

### 2. Detailed Loss Diagram (Final Realistic Simulation)
Comprehensive breakdown of thermal (-3.36%), near-shading (-2.49%), soiling (-1.50%), and BESS conversion losses.

<p align="center">
  <img src="figures/final_loss_diagram.png" alt="Final Loss Diagram" width="55%">
</p>

### 3. Financial Cashflows & Sensitivity Analysis
25-year lifetime financial modeling (70% Debt at 5.50% interest, 30% Equity) evaluating corporate PPA pricing and curtailment risk.

<p align="center">
  <img src="figures/final_financials.png" alt="Financial Results" width="80%">
</p>

---

## 🌿 Carbon Footprint & ESG Balance

* **Lifecycle Offset:** **137,863 tons of $\text{CO}_2$** over 30 years.
* **Carbon Payback Time:** The embodied emissions from manufacturing and construction are fully offset within **2.0 years** of operation.

---

## 📁 Repository Structure

```text
├── Final Report.pdf            # Full technical report (compiled from LaTeX)
├── PVsyst_Report_5MWp.pdf      # Detailed PVsyst simulation export
├── figures/                    # High-resolution simulation diagrams & plots
└── README.md                   # Project landing page & documentation
