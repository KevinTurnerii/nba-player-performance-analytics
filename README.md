# NBA 2023 Playoff Player Performance Modeling Framework  
Multivariate Analysis • Composite Metric Engineering • Unsupervised Learning (PCA + KMeans)

---

## 🚀 Modeling & Insights Snapshot

- Engineered **composite performance index using z-score normalization** across 5 key metrics  
- Ranked players using **balanced multi-dimensional scoring (PTS, AST, TRB, STL, BLK)**  
- Identified **top performers (Jokić, Booker, Durant, Tatum, Davis)** via standardized modeling  
- Applied **PCA (63% variance retained)** to reduce dimensional complexity  
- Segmented players into **Superstars, Starters, Role Players using KMeans (K=3)**  
- Built **end-to-end pipeline (R → Power BI)** for modeling + executive reporting  

---

## 📑 Table of Contents

- [Project Overview](#project-overview)
- [Business Problem](#business-problem)
- [Core Modeling Framework](#core-modeling-framework--composite-performance-index)
- [Key Insights](#key-insights)
- [Dimensionality Reduction (PCA)](#dimensionality-reduction-pca)
- [Unsupervised Learning — Player Segmentation](#unsupervised-learning--player-segmentation)
- [Power BI Dashboard](#power-bi-dashboard)
- [Visual Gallery](#visual-gallery)
- [Tools & Technologies](#tools--technologies)
- [Skills Demonstrated](#skills-demonstrated)
- [Conclusion](#conclusion)

---

## Project Overview

This project develops a **multivariate performance modeling framework** to evaluate NBA player impact using high-dimensional playoff statistics.

Rather than relying on isolated box score metrics, the system:

- Normalizes performance data across multiple statistical categories  
- Constructs a **composite performance index** for balanced evaluation  
- Applies **dimensionality reduction (PCA)** to simplify complexity  
- Uses **unsupervised learning (KMeans)** to segment player roles  

The result is a **data-driven player evaluation system** that captures total impact rather than single-stat dominance.

---

## Business Problem

Traditional player evaluation often relies on isolated metrics (e.g., points per game), which fails to capture:

- Multi-dimensional player contributions  
- Efficiency trade-offs (assists vs turnovers)  
- Defensive impact across multiple metrics  
- Role differentiation across teams  

This project addresses:

- How to **quantify overall player impact holistically**  
- How to **compare players across positions and play styles**  
- How to **segment players into meaningful performance tiers**  

---

## Core Modeling Framework — Composite Performance Index

A standardized performance index was engineered using:

- Points (PTS)  
- Assists (AST)  
- Total Rebounds (TRB)  
- Steals (STL)  
- Blocks (BLK)  

### Methodology

- All metrics were **z-score normalized**  
- Equal weighting applied (**20% each**)  
- Aggregated into a single composite score  

### Why This Matters

- Eliminates scale bias across metrics  
- Enables cross-position comparison  
- Captures balanced performance contribution  
- Produces a **reproducible ranking system**  

---

## Key Insights

### Top Performers (Composite Model)

1. Nikola Jokić  
2. Devin Booker  
3. Kevin Durant  
4. Jayson Tatum  
5. Anthony Davis  

> Top-ranked players consistently contributed across multiple categories — not just scoring.

---

### Correlation Structure

- **PTS ↔ AST: 0.81**  
- **PTS ↔ DRB: 0.71**  
- **AST ↔ STL: 0.74**  
- **DRB ↔ BLK: 0.65**

**Insight:**  
High-impact players exhibit **multi-dimensional statistical dominance**, not isolated specialization.

---

## Dimensionality Reduction (PCA)

Principal Component Analysis was applied to reduce dimensional complexity.

- **9 input features → 2 principal components**  
- **63% variance retained**

### Outcome

- Simplified visualization of player performance space  
- Preserved statistical relationships  
- Enabled clustering and segmentation  

---

## Unsupervised Learning — Player Segmentation

KMeans clustering (K=3) was applied to PCA-transformed data.

### Segments Identified:

- **Superstars** → High-impact, multi-dimensional players  
- **Starters** → Balanced contributors  
- **Role Players** → Specialized / lower-usage players  

### Why This Matters

- Fully **data-driven segmentation (no manual labels)**  
- Reproducible player archetypes  
- Reflects real-world clustering applications  

---

## Power BI Dashboard

Power BI serves as the **executive reporting layer**, translating modeling outputs into actionable insights.

### Dashboard Includes:

- Top Performers (Composite Score Ranking)  
- Scoring Breakdown (2PT / 3PT / FT)  
- Playmaking Efficiency (AST vs TOV)  
- Defensive Metrics (STL, BLK, PF)  
- Rebounding Analysis (ORB vs DRB)  
- Player Role Segmentation (Cluster Visualization)  

All visuals are driven directly from validated modeling outputs.

---

## Visual Gallery

These visuals represent key modeling outputs across scoring, defense, clustering, and performance evaluation.

### PCA Clustering (Player Roles)
![PCA Clustering](visuals_nba_2023_playoffs/pca_clustering_roles.png)

### Composite Score — Top Players Breakdown
![Top Players](visuals_nba_2023_playoffs/top_overall_weighted.png)

### Scoring Breakdown (2PT, 3PT, FT)
![Scoring Breakdown](visuals_nba_2023_playoffs/top_scorers_shooting.png)

### Assist vs Turnover Analysis
![Assist Leaders](visuals_nba_2023_playoffs/assist_turnover.png)

### Steals vs Fouls
![Steals](visuals_nba_2023_playoffs/steals_fouls.png)

### Blocks vs Fouls
![Blocks](visuals_nba_2023_playoffs/blocks_fouls.png)

### Rebounding Breakdown (ORB vs DRB)
![Rebounds](visuals_nba_2023_playoffs/rebound_breakdown.png)

### Correlation Heatmap
![Correlation](visuals_nba_2023_playoffs/correlation_heatmap.png)

### Power BI Executive Dashboard
![Dashboard](dashboard_preview_nba_2023.png)

---

## Tools & Technologies

- **R / RStudio** — Data analysis, modeling, clustering  
- **tidyverse / dplyr** — Data wrangling  
- **ggplot2 / ggcorrplot / factoextra** — Visualization & PCA  
- **KMeans / PCA** — Unsupervised learning  
- **Power BI (DAX)** — Dashboard & reporting  

---

## Skills Demonstrated

- Multivariate Statistical Analysis  
- Feature Engineering & Normalization  
- Composite Metric Development  
- Dimensionality Reduction (PCA)  
- Unsupervised Learning (KMeans)  
- Correlation Analysis  
- Data Visualization & Storytelling  
- Cross-platform workflow (R → Power BI)  

---

## Conclusion

This project demonstrates the ability to transform high-dimensional performance data into a structured analytical system using statistical modeling and machine learning techniques.

By combining:

- Composite metric engineering  
- PCA-based dimensional reduction  
- Unsupervised clustering  

The framework delivers a **reproducible, data-driven approach to player evaluation** aligned with real-world analytics and modeling workflows.
