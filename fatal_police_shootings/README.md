# Fatal Police Shootings in the United States — EDA

An exploratory data analysis of fatal shootings by on-duty police officers in the United States, based on data compiled by **The Washington Post**.

---

## 📌 Project Overview

This project investigates patterns and disparities in fatal police shootings across the United States from 2015 to 2021. The analysis explores racial demographics, geographic distribution, weapon involvement, mental illness, body camera usage, and trends over time.

---

## 📂 Dataset

- **Source:** [The Washington Post — Fatal Force Database](https://github.com/washingtonpost/data-police-shootings)
- **File:** `fatal-police-shootings-data.csv`
- **Records:** 6,349 incidents
- **Period:** January 2015 – June 2021

### Columns

| Column | Description |
|---|---|
| `id` | Unique identifier for each incident |
| `name` | Name of the individual involved |
| `date` | Date the incident occurred |
| `manner_of_death` | How the individual died (e.g., shot, shot and Tasered) |
| `armed` | Type of weapon, if any, found on the individual |
| `age` | Age of the individual at the time of the incident |
| `gender` | Gender of the individual |
| `race` | Race or ethnicity of the individual |
| `city` | City where the incident took place |
| `state` | State where the incident took place |
| `signs_of_mental_illness` | Whether the individual showed signs of mental illness |
| `threat_level` | Perceived threat level as assessed by officers |
| `flee` | Whether the individual was attempting to flee |
| `body_camera` | Whether the incident was recorded by a body camera |
| `longitude` | Longitude coordinate of the incident location |
| `latitude` | Latitude coordinate of the incident location |
| `is_geocoding_exact` | Whether the geographic coordinates are precisely accurate |

---

## 🔍 Key EDA Areas

- **Temporal trends** — How have fatal shootings changed year over year?
- **Geographic distribution** — Which states and cities have the highest incidents?
- **Racial disparities** — How are different racial groups represented relative to population share?
- **Armed vs unarmed** — What proportion of individuals were unarmed?
- **Mental illness** — How often was mental illness a factor?
- **Body camera coverage** — How frequently was the incident recorded?
- **Flee behavior** — What was the individual's behavior at the time of the shooting?

---

## 🛠️ Tools & Libraries

- **Python 3**
- `pandas` — data manipulation
- `numpy` — numerical operations
- `matplotlib` — visualizations
- `seaborn` — statistical plots
- `folium` — geographic mapping *(optional)*

---

## 🚀 Getting Started

1. Clone the repository
```bash
git clone https://github.com/your-username/fatal-police-shootings-eda.git
cd fatal-police-shootings-eda
```

2. Install dependencies
```bash
pip install pandas numpy matplotlib seaborn
```

3. Open the notebook
```bash
jupyter notebook fatal_police_shootings_eda.ipynb
```

---

## ⚠️ Data Limitations

- **Race is missing for ~10%** of records and cannot be imputed
- **Names are missing for ~3.7%** of records
- Data covers only incidents reported to The Washington Post and may not capture every case
- The dataset does not represent legal findings — individuals are suspects, not convicted criminals

---

## 📄 License

The dataset is published by The Washington Post under their data journalism initiative. Please refer to their [repository](https://github.com/washingtonpost/data-police-shootings) for usage terms.

---

## 🙏 Acknowledgements

- [The Washington Post](https://www.washingtonpost.com/graphics/investigations/police-shootings-database/) for compiling and maintaining the Fatal Force database
