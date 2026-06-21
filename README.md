# MovieIQ — Predictive Analytics on Film Success

```
███╗   ███╗ ██████╗ ██╗   ██╗██╗███████╗██╗ ██████╗ 
████╗ ████║██╔═══██╗██║   ██║██║██╔════╝██║██╔═══██╗
██╔████╔██║██║   ██║██║   ██║██║█████╗  ██║██║   ██║
██║╚██╔╝██║██║   ██║╚██╗ ██╔╝██║██╔══╝  ██║██║▄▄ ██║
██║ ╚═╝ ██║╚██████╔╝ ╚████╔╝ ██║███████╗██║╚██████╔╝
╚═╝     ╚═╝ ╚═════╝   ╚═══╝  ╚═╝╚══════╝╚═╝ ╚══▀▀═╝ 
```

```
[ PROJECT   ] ──► MovieIQ — Predictive Analytics on Film Success
[ MODEL     ] ──► Random Forest Classifier
[ FRAMEWORK ] ──► Streamlit Interactive Dashboard
[ BACKEND   ] ──► Pandas · NumPy · Scikit-learn · SciPy
[ STATUS    ] ──► LIVE · INTERACTIVE · PREDICTIVE
Python Streamlit RandomForest Pandas Seaborn Scikit-learn
```

---

## ◈ WHAT IS THIS?

MovieIQ is an interactive Streamlit dashboard that analyzes and predicts the success of movies using key performance indicators. Drop in a movies dataset and the app:

- Predicts whether a movie will be successful based on Budget vs Revenue
- Visualizes trends across genres, budgets, popularity, and vote averages
- Runs T-Test and Chi-Square statistical tests automatically
- Uses Random Forest Classifier for ML-based success prediction
- Filters interactively by genre and vote average via sidebar

No manual analysis. Just explore, filter, and predict.

---

## ◈ SYSTEM ARCHITECTURE

```
┌─────────────────────────────────────────────────┐
│              STREAMLIT DASHBOARD                │
│                                                 │
│  ┌───────────┐  ┌───────────┐  ┌───────────┐  │
│  │  FILTER   │  │  VISUAL   │  │  PREDICT  │  │
│  │ SIDEBAR   │  │ INSIGHTS  │  │  ENGINE   │  │
│  │  🎛️       │  │  📊       │  │  🤖       │  │
│  └─────┬─────┘  └─────┬─────┘  └─────┬─────┘  │
│        │              │              │          │
│        └──────────────┼──────────────┘          │
│                       │                         │
│                ┌──────▼──────┐                  │
│                │  DATA LAYER │                  │
│                │  Pandas +   │                  │
│                │  NumPy      │                  │
│                └──────┬──────┘                  │
│                       │                         │
│         ┌─────────────┼─────────────┐           │
│         │             │             │           │
│   ┌─────▼─────┐ ┌─────▼─────┐ ┌───▼───────┐   │
│   │   STATS   │ │   PLOTS   │ │   ML      │   │
│   │  T-Test   │ │  Seaborn  │ │  Random   │   │
│   │  Chi-Sq   │ │  Matplotlib│ │  Forest   │   │
│   │  SciPy    │ │           │ │  Sklearn  │   │
│   └───────────┘ └───────────┘ └───────────┘   │
└─────────────────────────────────────────────────┘
                       │
                       ▼
┌─────────────────────────────────────────────────┐
│                 movies.csv                      │
│  budget · revenue · popularity · runtime        │
│  vote_average · title · genres                  │
└─────────────────────────────────────────────────┘
```

---

## ◈ KEY FEATURES

```
┌─────────────────────────────────────────────────┐
│  FEATURE          │  DESCRIPTION                │
│───────────────────│────────────────────────────│
│  🎯 Prediction    │  Revenue > Budget = Success │
│  📈 Visualization │  Budget vs Revenue trends   │
│  📊 Statistics    │  T-Test + Chi-Square tests  │
│  🤖 ML Model      │  Random Forest Classifier   │
│  🧠 Filtering     │  Genre + Vote Average       │
│  🧼 Clean UI      │  Modular Streamlit layout   │
└─────────────────────────────────────────────────┘
```

---

## ◈ TECH STACK

```
┌─────────────────────────────────────────────────┐
│  Layer          │  Technology                   │
│─────────────────│──────────────────────────────│
│  Dashboard      │  Streamlit                   │
│  Data           │  Pandas, NumPy               │
│  Visualization  │  Seaborn, Matplotlib         │
│  Machine Learning│  Scikit-learn (Random Forest)│
│  Statistics     │  SciPy (T-Test, Chi-Square)  │
│  Language       │  Python 🐍                   │
└─────────────────────────────────────────────────┘
```

---

## ◈ PROJECT STRUCTURE

```
MovieIQ/
├── MovieIQ.py          ← Main Streamlit dashboard
├── movies.csv          ← Dataset (budget, revenue, genres...)
├── requirements.txt    ← Python dependencies
└── assets/             ← Screenshots and images
```

---

## ◈ DATASET

```
movies.csv must include these columns:

┌──────────────┬─────────────────────────────┐
│  Column      │  Description                │
│──────────────│────────────────────────────│
│  budget      │  Production budget          │
│  revenue     │  Box office revenue         │
│  popularity  │  Popularity score           │
│  runtime     │  Movie duration (minutes)   │
│  vote_average│  Average user rating        │
│  title       │  Movie title                │
│  genres      │  Genre categories           │
└──────────────┴─────────────────────────────┘
```

---

## ◈ SETUP AND RUN

### 1. Clone Repository
```bash
git clone https://github.com/dharankumar/MovieIQ.git
cd MovieIQ
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Run the App
```bash
streamlit run MovieIQ.py
```

### 4. Open in Browser
```
http://localhost:8501
```

---

## ◈ LIVE DEMO

```
🚀 Click here to try the live app(https://movieiq-predictive-analytics-on-film-success-hkz386d9xzv5mygjz.streamlit.app/)
```

---

## ◈ AUTHOR

```
┌──────────────────────────────────────────────────┐
│                                                  │
│  Dharankumar                                     │
│  B.Tech — AI and Data Science                    │
│                                                  │
│  Project: MovieIQ — Predictive Analytics         │
│           on Film Success                        │
│  Stack:   Streamlit · Random Forest · Pandas     │
│           Seaborn · Scikit-learn · SciPy         │
│                                                  │
└──────────────────────────────────────────────────┘

┌────────────────────────────────────────────────────┐
│                                                    │
│   APP FLOW                                         │
│                                                    │
│   LOAD ──► FILTER ──► VISUALIZE ──► PREDICT       │
│              ▲              │            │         │
│              │   (sidebar)  │            │         │
│              └──────────────┘            │         │
│                                          ▼         │
│                                   SUCCESS / FAIL ✅ │
│                                                    │
└────────────────────────────────────────────────────┘

```
A dashboard that predicts movie success before release.
Built with Streamlit · Powered by Random Forest · Analyzed by SciPy
```
