<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=180&section=header&text=Manikanth%20Nampally&fontSize=42&fontColor=fff&animation=twinkling&fontAlignY=32&desc=Data%20Engineer%20%7C%20ML%20Infrastructure%20%7C%20Cloud%20Data%20Platforms&descAlignY=53&descAlign=50" width="100%"/>

<div align="center">

[![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=700&size=20&pause=1000&color=00D4FF&center=true&vCenter=true&width=750&lines=Building+real-time+pipelines+processing+10%2B+TB%2Fday;Streaming+708M%2B+events+across+AWS+%7C+Azure+%7C+GCP;AI+agents+scoring+500%2B+equities+daily+with+LangGraph;Fine-tuning+FinBERT+%7C+PyTorch+%7C+TensorFlow+in+production;MLOps+engineer+shipping+0.992+F1+phishing+detectors)](https://git.io/typing-svg)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/manikanthn)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/maninampally)
[![Email](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:manikanthnampally94@gmail.com)
[![Profile Views](https://komarev.com/ghpvc/?username=maninampally&label=Profile%20Views&color=0e75b6&style=for-the-badge)](https://github.com/maninampally)

🟢 **Open to Data Engineer · ML Engineer · MLOps roles · Remote friendly**

</div>

---

## ☕ Barista Pipeline

```python
# ── BARISTA PIPELINE ─────────────────────────────────────────
# (yes this is a real ETL. yes i wrote it between orders.)

from datetime import datetime

def extract(beans: str) -> dict:
    """Pull raw ingredients from the bar"""
    return {"beans": beans, "source": "FAU Starbucks", "barista": "Mani"}

def transform(order: dict) -> dict:
    """Craft the drink. no oat milk. ever."""
    hour = datetime.now().hour
    if 5 <= hour < 15:
        order["drink"]  = "Brown Sugar Shaken Espresso sub VSC"
        order["mood"]   = "focused ⚡"
    else:
        order["drink"]  = "Trenta Vanilla Sweet Cream Cold Brew"
        order["mood"]   = "in the zone 🧊"
    order["made_by"]    = "Mani (the barista who also deploys to prod)"
    order["quality"]    = "10/10 — obviously"
    return order

def load(order: dict) -> str:
    """Serve drink. get back to writing dbt models."""
    return (
        f"\n ☕ DRINK READY  : {order['drink']}\n"
        f"  🎯 Mood         : {order['mood']}\n"
        f"  👨‍🍳 Made by      : {order['made_by']}\n"
        f"  ⭐ Quality      : {order['quality']}\n"
        f"  📝 Next action  : finish this Airflow DAG before next customer\n"
    )

# E → T → L
raw     = extract("espresso beans + vanilla sweet cream")
crafted = transform(raw)
print(load(crafted))
print("  💬 'I debug pipelines and make cold brews. simultaneously.'\n")
```

---

## 🧠 About Me

```python
# ============================================================
#   mani.py — run at your own risk. side effects include:
#   jaw dropping, immediate hiring, and pipeline envy.
# ============================================================

import random
import time

# ── FUEL SYSTEM ─────────────────────────────────────────────
FUEL = {
    "morning"    : "☕ Double Espresso",
    "debugging"  : "🧊 Cold Brew (large)",
    "production" : "⚡ Red Bull",
    "bored"      : "🧋 Brown Sugar Boba",
    "victory"    : "🍺 Craft IPA",
    "2am_deploy" : "☕☕☕ Triple Shot Everything",
}

FOOD = {
    "focused"    : "🍜 Ramen (extra spicy)",
    "monday"     : "🍕 Pizza (mandatory)",
    "data_win"   : "🌮 Tacos (celebration mode)",
    "tired"      : "🍫 Dark Chocolate + Cold Brew",
    "weekend"    : "🥞 Pancakes while reading docs",
    "big_deploy" : "🍣 Sushi (earned it)",
}

def refuel(mood):
    drink = FUEL.get(mood, FUEL["debugging"])
    snack = FOOD.get(mood, FOOD["focused"])
    print(f"  🔋 Refueling → {drink} + {snack}")
    time.sleep(0.4)


# ── BOOT SEQUENCE ────────────────────────────────────────────
def boot():
    steps = [
        ("Waking up Mani",              "morning"),
        ("Ingesting 10+ TB/day",        "focused"),
        ("Connecting AWS + GCP + Azure","production"),
        ("Spawning LangGraph agents",   "victory"),
        ("Checking pipeline SLAs",      "debugging"),
        ("Deploying to ECR + EC2",      "2am_deploy"),
    ]
    print("🚀 Booting mani.py...\n")
    for step, mood in steps:
        print(f"  ⚙️  {step}...", end=" ", flush=True)
        time.sleep(0.3)
        print("✅")
        if random.random() > 0.6:       # randomly needs fuel
            refuel(mood)
    print()

boot()


# ── IDENTITY ─────────────────────────────────────────────────
print("""
╔═══════════════════════════════════════════════════════════╗
║          MANIKANTH NAMPALLY  —  DATA ENGINEER             ║
╠═══════════════════════════════════════════════════════════╣
║  📍 Location    Boca Raton, FL (remote-friendly)          ║
║  🎓 Education   M.S. ITM — FAU (2026)  |  GPA 3.9         ║
║  💼 Currently   Data Engineer @ Opsylux LLC               ║
║  ⚡ Scale       10+ TB/day · 708M+ events · 3 clouds      ║
║  🤖 Building    Artha AI · FinSentinel                    ║
╚═══════════════════════════════════════════════════════════╝
""")


# ── SKILLS ───────────────────────────────────────────────────
stack = {
    "🔥 Strengths"   : ["Real-time pipelines", "Lakehouse design", "MLOps", "AI agents"],
    "☁️  Clouds"     : ["AWS", "GCP", "Azure"],
    "🛠️  Core Stack"  : ["PySpark", "Kafka", "Airflow", "dbt Core", "Delta Lake"],
    "🤖 AI / ML"     : ["LangGraph", "PyTorch", "TensorFlow", "MLflow", "FinBERT"],
    "🚢 DevOps"      : ["Docker", "Kubernetes", "Terraform", "GitHub Actions"],
}

print("─" * 55)
for category, items in stack.items():
    print(f"  {category:22} →  {' · '.join(items)}")
print("─" * 55)


# ── FUN FACTS ────────────────────────────────────────────────
print("\n💡 Things Mani does before you finish your coffee:\n")
facts = [
    "processes more data before 9am than most do all week 📦",
    "reduced query runtime 4.2 min → 88 sec, saved $18K 💰",
    "built AI agents that think like Warren Buffett 📈",
    "deploys to 3 clouds at once without breaking a sweat 🌩️",
    "scored 708M+ auth events in real-time at 10K events/sec 🔐",
    "turns raw data into decisions, not just dashboards 🧠",
    "achieves 0.992 F1 then immediately orders sushi 🍣",
]
for i, fact in enumerate(facts, 1):
    print(f"  {i}. {fact}")


# ── CURRENT MOOD ─────────────────────────────────────────────
mood_today = random.choice(list(FUEL.keys()))
print(f"\n🎲 Current mood: {mood_today.upper().replace('_',' ')}")
refuel(mood_today)


# ── STATUS ───────────────────────────────────────────────────
print("""
┌─────────────────────────────────────────────────────┐
│  ✅  Open to:  Data Engineer · ML Engineer · MLOps  │
│  📧  manikanthnampally94@gmail.com                  │
│  🔗  linkedin.com/in/manikanthn                     │
└─────────────────────────────────────────────────────┘
""")

print("# End of mani.py — hire him before someone else does 🚀")
```

---

## 🚀 Featured Projects

| Project | Stack | Scale & Impact |
|---|---|---|
| [**Artha AI**](https://github.com/maninampally/artha-ai) | LangGraph · Airflow · dbt · pgvector · MLflow · FastAPI | 500+ equities daily · 10+ investor models · sub-50ms p99 |
| [**FinSentinel**](https://github.com/maninampally/finsentinel) | PyTorch · FinBERT · GCP · Pub/Sub · Evidently AI · Airflow | 0.95 F1 · 500+ articles/day · live drift monitoring |
| [**AuthPulse**](https://github.com/maninampally/authpulse-analytics) | Kinesis · S3 · Lambda · Terraform · CloudWatch | 708M+ events · 1K–10K/sec · 99.9% SLA |
| [**Network Security MLOps**](https://github.com/maninampally/network-security) | FastAPI · Docker · ECR · EC2 · MLflow · DagsHub | 0.992 F1 · 26 experiments · full CI/CD |

---

## 🛠️ Tech Stack

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)
![Scala](https://img.shields.io/badge/Scala-DC322F?style=for-the-badge&logo=scala&logoColor=white)

**Data Engineering**

![Kafka](https://img.shields.io/badge/Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)
![Airflow](https://img.shields.io/badge/Airflow-017CEE?style=for-the-badge&logo=apacheairflow&logoColor=white)
![dbt](https://img.shields.io/badge/dbt-FF694B?style=for-the-badge&logo=dbt&logoColor=white)
![Spark](https://img.shields.io/badge/Spark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)
![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=for-the-badge&logo=databricks&logoColor=white)
![Delta Lake](https://img.shields.io/badge/Delta_Lake-003366?style=for-the-badge&logoColor=white)

**Cloud**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)
![GCP](https://img.shields.io/badge/GCP-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white)

**ML / AI / MLOps**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=for-the-badge&logo=mlflow&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-00D4FF?style=for-the-badge&logo=python&logoColor=white)

---

## 📊 GitHub Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=maninampally&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" height="165"/>
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=maninampally&layout=compact&theme=tokyonight&hide_border=true" height="165"/>

![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=maninampally&theme=tokyonight&hide_border=true)

</div>

---

## 📈 Contribution Activity

<div align="center">

[![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=maninampally&theme=tokyo-night&hide_border=true)](https://github.com/maninampally)

</div>

---

## 🐍 Contribution Snake

<div align="center">

<img src="https://raw.githubusercontent.com/maninampally/maninampally/output/github-contribution-grid-snake-dark.svg" alt="Snake animation"/>

</div>

---

<div align="center">

*"The stock market is a device for transferring money from the impatient to the patient."*
**— Warren Buffett**

*The best data engineers don't just move data — they move decisions.*

📍 Boca Raton, FL &nbsp;·&nbsp; Open to remote & relocation
&nbsp;
📧 manikanthnampally94@gmail.com

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=100&section=footer" width="100%"/>

</div>