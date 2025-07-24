# 🦇 HIT140 Group Project - Bat and Rat Behaviour Analysis (2025)


https://deepnote.com/workspace/CDU-PROJECT-a61a9091-f959-456d-9fa1-960e3207a1a9/project/Avery-Doans-Untitled-project-74c414ef-560d-420d-b4af-809d2b670979/notebook/Notebook-1-f8610b95e75245d99f9b3a185ffb717d?utm_source=share-modal&utm_medium=product-shared-content&utm_campaign=notebook&utm_content=74c414ef-560d-420d-b4af-809d2b670979

Welcome to our group project for **HIT140: Foundations of Data Science**. In this project, we act as data detectives to support zoologists investigating the interactions between bats and rats at a shared food platform.

---

## 📌 Project Overview

We aim to answer two key scientific investigations using real-world surveillance data:

### 🔍 Investigations
- **Investigation A**: Do bats perceive rats as competitors or predators?  
- **Investigation B**: How do bat-rat interactions change across seasons?

---

## 🗂️ Datasets Used

## 📁 Dataset 1: `dataset1.csv` — Individual Bat Landings

Each row represents a **single bat landing event** at the food platform. It captures the context of the event, the bat’s response, and whether it got a reward.

| Column Name              | What it Means |
|--------------------------|---------------|
| `start_time`             | When the bat landed on the platform (timestamp). |
| `bat_landing_to_food`    | How long (in seconds) it took the bat to start approaching food after landing. A longer delay may indicate caution or fear. |
| `habit`                  | Description of the environment or situation during the event (e.g. how noisy, crowded, etc.). |
| `rat_period_start`       | The time when the rats first arrived on the platform. |
| `rat_period_end`         | The time when the rats left the platform. |
| `seconds_after_rat_arrival` | Time (in seconds) between rat arrival and bat landing. Negative = bat landed before rats. |
| `risk`                   | Did the bat take a risk? (0 = avoided risk, 1 = took risk, e.g. attacking or approaching rats). |
| `reward`                 | Did the bat get a reward (e.g. food)? (0 = no, 1 = yes). |
| `month`                  | The month the landing occurred (e.g. "June"). |
| `sunset_time`            | The time of sunset on the observation day. |
| `hours_after_sunset`     | Time (in hours) after sunset that the bat landed. |
| `season`                 | Season of the observation (e.g. "Winter", "Spring"). |

---

## 📁 Dataset 2: `dataset2.csv` — 30-Minute Observation Periods

Each row represents a **30-minute surveillance period** at the food platform. It summarizes how many bats and rats were observed, and how much food remained.

| Column Name              | What it Means |
|--------------------------|---------------|
| `time`                   | Start time of the 30-minute observation period. |
| `month`                  | The month the observation occurred. |
| `hours_after_sunset`     | Time (in hours) after sunset when the observation started. |
| `bat_landing_number`     | Total number of bat landings during the 30-minute period. |
| `food_availability`      | Estimated amount of food remaining at the end of the period (unit not specified). |
| `rat_minutes`            | Total minutes rats were seen on the platform during the 30 minutes. |
| `rat_arrival_number`     | Number of distinct rat arrivals during the 30-minute observation window. |


---

## 🧭 Project Timeline & Tasks

### 🔹 Phase 1: Setup and Planning (Week 1)
- Understand project objectives
- Assign team roles (Analyst, Cleaner, Visualizer, Presenter, Writer)
- Create shared workspace (Google Drive / GitHub)
- Download datasets from Learnline

### 🔹 Phase 2: Data Exploration & Cleaning (Week 2)
- Inspect data types, missing values, and outliers
- Clean and preprocess data ethically
- Perform exploratory data analysis (EDA)
- Create summary stats and graphs

### 🔹 Phase 3: Investigation A – Bat Perception of Rats (Week 3–4)
- Feature engineering: Rat presence, response time, risk-taking
- Descriptive stats: Behaviour with vs without rats
- Inferential analysis: t-tests, chi-square tests
- Visualizations: Boxplots, bar graphs, timelines
- Deliverable: Team video presentation (Assessment 2)

### 🔹 Phase 4: Investigation B – Seasonal Behaviour Changes (Week 5–6)
- Filter datasets by `season` and `month`
- Analyze seasonal trends in bat and rat activity
- Compare behaviour across winter vs spring
- Optional: incorporate external environmental data
- Deliverable: Analytical content for group report (Assessment 3)

### 🔹 Phase 5: Group Report Writing (Week 6–7)
- Structure the report:
  - Introduction
  - Methodology
  - Results
  - Discussion
  - Conclusion
  - References (APA style)
  - AI tools usage declaration
- Peer review & editing

### 🔹 Phase 6: Final Submission (Week 8)
- Review Learnline instructions
- Final polish and formatting
- Submit report and forms on time

---

## 🧰 Tools & Libraries

- Python: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy.stats`, `statsmodels`
- Jupyter Notebook for analysis
- GitHub / Google Drive for collaboration
- PowerPoint + OBS/Zoom for presentation

---

## 📎 Notes

- Ethical analysis is required — no altering of original data values to suit desired outcomes.
- Feature engineering is encouraged.
- Expect real-world “dirty” data: missing, inconsistent, and irregular values.

---

## 📚 Acknowledgement

Project derived from:
Chen, Xing et al. (2025), “Complex competition interactions between Egyptian fruit bats and black rats in the real world”, Mendeley Data, V1, doi: [10.17632/gt7j39b2cf.1](https://doi.org/10.17632/gt7j39b2cf.1) (License CC BY 4.0)

Adapted by Dr Yakub Sebastian for HIT140, CDU.

---
