# 📊 Data Visualization Project — Online Violence in Israel

**Course:** Data Visualization and Cognition  
**Institution:** Technion – Israel Institute of Technology  

📈 [Public Tableau Dashboard](https://public.tableau.com/views/Project_Group25/2025DemographicDashboard)  

---

## 🧭 Overview

This project analyzes **online violence in Israel** based on *Israeli Internet Association (ISOC-IL)* survey data (2022–2025).  
We designed three interactive dashboards and one narrative story in Tableau, exploring **demographics**, **exposure to online harm**, and **temporal evolution** of online violence.

Our approach emphasized **clarity, neutrality, and cognitive accessibility**, following Munzner’s *Why / What / How* visualization design framework.

---

## 📂 Data Sources

We worked with three official survey datasets:

| Year | Source | Rows | Columns |
|------|---------|-------|----------|
| 2025 | [Google Sheet](https://docs.google.com/spreadsheets/d/1buSatpfDOubuezXV6xscLYcVUfRx-G_n/edit?usp=drive_link) | 1002 | 226 |
| 2024 | [Drive file](https://drive.google.com/file/d/126oFvu3iCLlU2G4gUR1V2mRyA1ry0-Po/view?usp=drive_link) | 1004 | 67 |
| 2022 | [Drive file](https://drive.google.com/file/d/1m2T5nmTI_UkKYkKohGDH1BCbam1z03WA/view?usp=drive_link) | 802 | 68 |

---

## 🧮 Data Preparation (Excel Workflow)

Before importing to Tableau, all datasets were **cleaned and reformatted in Excel** to ensure a long-form, analysis-ready structure.

**Main steps:**
1. Extracted relevant sheets (`Coded_Data` and `Labeled_Data`).  
2. Converted wide tables to long format (`Question`, `Answer`, `RespondentID`).  
3. Split multi-response columns (e.g., `Q12_X_Y`) into separate variables.  
4. Standardized demographic fields (Gender, Age, Religion, etc.).  
5. Unified formats and categories across years (2022–2025).  
6. Created a merged dataset for longitudinal comparison.  

All transformations were manual and formula-based within Excel to preserve survey integrity.

📘 *The cleaned Excel dataset can be provided upon request.*  
If you are interested in exploring or reproducing this work, please reach out.

---

## 🧱 Tableau Structure

| Type | Name | Purpose | Color |
|------|------|----------|-------|
| Dashboard | *Demographic Dashboard 2025* | Population overview | 🔵 Blue |
| Dashboard | *Dashboard 2025* | Online violence exposure & reactions | 🟤 Brown |
| Dashboard | *Selected vs Others* | Subgroup comparison | 🟠 Yellow |
| Story | *Online Violence in Israel (2022–2025)* | Longitudinal narrative | 🔴 Red |

---

## 🎨 Dashboard Summaries

### 1️⃣ **Demographic Dashboard 2025**
Displays respondent demographics: Gender, Age, Religion, Language, Education, Region, and more.  
Horizontal bar charts with 0–100% scaling ensure clear comparisons.  
Neutral grayscale palette ensures unbiased interpretation.  
**Design task:** `{Present, Distribution}`

---

### 2️⃣ **Dashboard 2025**
Focuses on **exposure to online violence** and **reactions** (reporting, blocking, ignoring).  
Includes frequency of harassment, doxxing, and fear of expression.

Visual encodings:
- Stacked bars (frequency)
- Multi-set bars (reaction vs. type)
- Heatmaps (platform × violence type)  

**Design task:** `{Present, Distribution}`

---

### 3️⃣ **Selected vs Others**
Compares a user-selected subgroup (e.g., Arab population) against all others using **dumbbell charts**.  
Displays differences for key indicators and relative sample size.  
**Design task:** `{Compare values}`

---

### 4️⃣ **Story: Online Violence in Israel (2022–2025)**
Narrative dashboard connecting all insights:  
- Trends in exposure (32.8% → 52.4%)  
- Rise in harassment and shaming  
- Highest increases among Youth, Haredi, and Arab respondents.  

**Design task:** `{Present, Trends}`  
Uses diverging palette (warm/cool) to emphasize key contrasts.

---

## 🧠 Design Principles

Following **Munzner’s Visualization Framework (Why / What / How):**

| Dimension | Application |
|------------|--------------|
| **Why** | Enable transparent exploration of online violence data |
| **What** | Nominal, ordinal, and quantitative attributes |
| **How** | Position for ordered attributes, color luminance for magnitude, hue for categories |

**Cognitive Design Choices:**
- Ordered encodings (ordinal → position, categorical → hue)  
- Consistent color palette across dashboards  
- Clear legends, titles, and scales  
- Avoided emotive colors for sensitive topics  

---

## ⚙️ Tools & Technologies

| Tool | Purpose |
|------|----------|
| **Microsoft Excel** | Data cleaning, normalization, merging (wide → long) |
| **Tableau Desktop** | Dashboard and storytelling design |
| **Google Drive / Sheets** | Collaboration and source hosting |
| **Tableau Public** | Online publication |


---

## 📁 Repository Structure

```text
│
├── Project_Group25.twbx      # Tableau packaged workbook
│
└── README.md
