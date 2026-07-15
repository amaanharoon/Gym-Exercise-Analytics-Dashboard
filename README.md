# 🏋️ Gym Exercise Analytics Dashboard

[![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![Data Source](https://img.shields.io/badge/Dataset-Kaggle-blue?style=for-the-badge)](https://www.kaggle.com/)
[![UX Design](https://img.shields.io/badge/UX/UI-Custom_App_Layout-10B981?style=for-the-badge)](#)

An interactive, custom-designed 4-page Power BI diagnostic application analyzing a comprehensive database of **2,918 unique gym exercises**. This dashboard shifts away from the rigid "default" Power BI aesthetic, delivering a sleek, cohesive, modern app-like experience with fluid custom navigation.

---

## 🎨 UI/UX Design & Theme System

The application relies on a strict, professional design language curated specifically for readability, visual hierarchy, and polished presentation.

| Design Element | Choice / Hex Code | Purpose |
| :--- | :--- | :--- |
| **Primary Theme Color** | `#10B981` (Emerald Green) | Denotes active states, user navigation, and high-satisfaction rating metrics. |
| **Secondary Neutral** | `#111827` (Obsidian Dark) | Structural charts, high-volume categorical distributions, and key headers. |
| **Muted Accents** | `#64748B` (Slate Gray) | Unselected navigation buttons, descriptive subtitles, and supporting legends. |
| **Canvas Background** | `#EEF2F6` (Light Slate Gray) | Soft, premium background that reduces screen glare and increases card contrast. |
| **Cards & Visual Containers** | `#FFFFFF` (Pure White) | Features a custom `12px` rounded border and subtle bottom-right drop shadows for a "floating" layer effect. |

---

## 📱 Dashboard Architecture & Pages

### 1. Overview Page
*   **Purpose:** Establishes the macro-level scale of the dataset and surfaces immediate critical findings.
*   **Key Elements:**
    *   **KPI Cards:** Displaying Total Exercises (**2.909K**), Rated Exercises (**1.031K**), Average User Rating (**5.92**), and Unique Equipment Types (**13**).
    *   **Quick Insights Panel:** Highlights key actionable trends (e.g., Strength training dominates at 87%, Bodyweight is the most accessible equipment type, and a 64% rating gap exists).

### 2. Equipment & Types Page
*   **Purpose:** Cross-examines physical equipment requirements with different training methodologies.
*   **Key Elements:**
    *   *What are the most popular equipment categories?* (Clustered Bar Chart featuring Obsidian bars mapping "Body Only" and "Dumbbell" dominance).
    *   *How are exercises categorized by style?* (Custom Donut Chart isolating "Strength" vs. "Plyometrics" vs. "Stretching" ratios).

### 3. Muscle Groups Page
*   **Purpose:** Maps the anatomical targeting distribution and evaluates target-specific user satisfaction.
*   **Key Elements:**
    *   *Which body parts have the most exercises?* (Obsidian horizontal bar chart highlighting Abdominal and Quadriceps target dominance).
    *   *Which target muscle exercises have the highest user satisfaction?* (Emerald horizontal bar chart tracking average rating benchmarks; blank-rating rows filtered out to prevent data skew).

### 4. Difficulty & Quality Page
*   **Purpose:** Visualizes catalog depth across skill levels and discovers how mechanical difficulty impacts user satisfaction.
*   **Key Elements:**
    *   *How are exercises distributed by difficulty level?* (Vertical Clustered Column Chart mapping volume; heavily weighted towards Intermediate exercises).
    *   *Average user rating across difficulty levels* (Emerald Green column chart proving that Expert exercises, despite low availability, yield the highest user ratings).

---

## ⚡ Technical Implementations & Custom Engineering

*   **Custom Page Navigation (App-Like Logic):** Built completely custom page-state button menus. Utilizing separate active/inactive button state formatting configurations (White/Gray unselected vs. Emerald/White selected), the menu behaves like a dynamic web application.
*   **No-Blank Filtering Logic:** Applied strict visual-level filters targeting ratings (`Rating is not blank`) on performance-metric charts, ensuring average calculations are unpolluted by unrated data.
*   **Perfect Grid Alignment:** Followed strict container spacing guidelines, keeping consistent padding gaps between visuals and aligning headers across all four canvases to maintain visual flow during page transitions.

---

## 📊 Core Data Insights

1.  **Strength Dominates:** Over **87% (2,545 exercises)** of the entire physical database is focused strictly on strength-building routines.
2.  **Equipment Accessibility:** "Body Only" is the single most frequent equipment type with **1,078 exercises**, followed closely by traditional "Dumbbells" (**516 exercises**).
3.  **The Rating Gap:** Only **1,031 out of 2,918 exercises** have historically been rated, exposing a significant portion (~64%) of unrated movement assets in the catalog.
4.  **Difficulty Paradox:** While "Intermediate" workouts make up the vast majority of the catalog, "Expert" exercises average the highest user ratings at **8.4 / 10**, showing highly targeted satisfaction for specialized training.
