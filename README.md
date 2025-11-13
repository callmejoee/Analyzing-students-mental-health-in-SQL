# 🧠 Exploring Mental Health of International Students Using PostgreSQL

### 📘 Study Overview

A 2018 survey conducted at a Japanese international university explored whether **studying abroad affects students’ mental health**.  
The research found that:
- **International students** are at a higher risk of mental health challenges compared to the general population.  
- **Social connectedness** (feeling part of a community) and **acculturative stress** (stress from adapting to a new culture) are strong predictors of depression levels.

In this project, we use **PostgreSQL** to explore the provided student dataset and see if we can **arrive at similar conclusions**.  
Additionally, we’ll investigate whether the **length of stay in Japan** contributes to mental health outcomes.

---

### 🧾 Dataset Description

| Field Name | Description |
|-------------|-------------|
| `inter_dom` | Type of student (International or Domestic) |
| `japanese_cate` | Japanese language proficiency |
| `english_cate` | English language proficiency |
| `academic` | Current academic level (Undergraduate or Graduate) |
| `age` | Age of the student |
| `stay` | Current length of stay (in years) |
| `todep` | Total score of depression (PHQ-9 test) |
| `tosc` | Total score of social connectedness (SCS test) |
| `toas` | Total score of acculturative stress (ASISS test) |

---

### 🧩 Objective

- Analyze how **length of stay** relates to depression, social connectedness, and acculturative stress among **international students**.  
- Identify patterns that may explain mental health differences in international learners.

---

### 🗃️ Load the Data

```sql
-- Load the CSV file into PostgreSQL as a table
SELECT * 
FROM students;
