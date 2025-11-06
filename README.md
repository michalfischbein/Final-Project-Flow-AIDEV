�

---

````markdown
# 🧠 The Super Crew
### Multi-Agent Data Analysis Flow on the *Superstore* Dataset  

> A collaborative data analysis project powered by **CrewAI Flow**, designed to demonstrate intelligent multi-agent collaboration for business insight generation and data visualization.

---

## 📦 Dataset  
**Source:** [Superstore Dataset – Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)  
This dataset contains sales, profit, and discount data for a retail store across multiple regions, categories, and years.

---

## 🔄 Project Flow  

The project runs in three main stages:

```text
1️⃣ EDA (eda.py)
   → Cleans and validates raw data

2️⃣ CrewAI Flow (main.py)
   ├── Data Analysis Crew: statistical & descriptive analysis
   └── Visualization Crew: generates actionable insights & charts
````

---

## ⚙️ Setup Instructions

### Step 1: Clone the repository

```bash
git clone <repo-url>
cd the_super_crew
```

### Step 2: Create a virtual environment

```bash
python3.11 -m venv supercrew_env
source supercrew_env/bin/activate
```

### Step 3: Install dependencies

```bash
pip install -r requirements.txt
```

---

## 🔐 Environment Variables

> ⚠️ The `.env` file is **not included** in the repository for security reasons.
> You must create it manually in the project root before running the project.

Create a new `.env` file:

```bash
touch .env
```

Then add the following lines:

```env
OPENAI_API_KEY=your_openai_api_key_here
SERPER_API_KEY=your_serper_api_key_here
```

These keys are required for:

* OpenAI LLM processing
* Web search (Serper tool)

---

## ▶️ Running the Project

Run data cleaning and EDA:

```bash
python src/the_super_crew/eda.py
```

Run the full multi-agent CrewAI flow:

```bash
python src/the_super_crew/main.py
```

Outputs are automatically saved in the `outputs/` directory.
The final visualizations will be available as `.png` or `.html` files.

---

## 📊 Visual Outputs

The following charts were generated based on the **Action Advisor’s** recommendations:

* **Chart 1:** Displays **profit margins by product category**, highlighting *Technology* as the most profitable.
* **Chart 2:** Visualizes the **relationship between discounts and profits**, showing a negative correlation (higher discounts reduce profitability).
* **Chart 3:** Illustrates **regional performance**, emphasizing stronger profitability in the *East* and *West* regions.

---

## 🧠 CrewAI Flow Structure

| Crew                      | Description                                                                                              | Key Outputs                                         |
| ------------------------- | -------------------------------------------------------------------------------------------------------- | --------------------------------------------------- |
| 🧩 **Data Analysis Code** |   performes data cleaning and statistical analysis                                                    |  |
| 💡 **Data Analysis Crew**     |  Performs statistical and descriptive data analysis, Selects high-impact business questions, recommends strategic actions, and identifies visualization needs | `data_analysis_findings.md`, `business_insights.md``action_recommendations.md`                         |
| 📈 **Visualization Crew** | Generates charts and exports clean visualization scripts                                                 | `.png` / `.html` charts                             |

---

## 🧰 Tech Stack

* **Python 3.11**
* **CrewAI Framework**
* **Pandas**, **Matplotlib**, **Seaborn**
* **python-dotenv**, **Serper**, **OpenAI API**

---

## 👥 Team

| Name                 | Role                               |
| -------------------- | ---------------------------------- |
| **Michal Fischbein** | AI Developer |
| **Eldad Abadi**      | AI Developer            |
| **Bat El Klein**     | AI Developer                 |
| **Yehuda Frish**     | AI Developer             |

---

## 🧩 Summary

This project demonstrates how multi-agent collaboration can streamline and enhance data analysis workflows.
By leveraging **CrewAI Flow**, each agent contributes a specific role — from data exploration, to strategic recommendations, to visualization delivery —
creating a reproducible and scalable analytics pipeline for business intelligence.

---

> 💡 *The Super Crew* is part of an academic data science portfolio project exploring automation in insight generation using AI agents.

```


