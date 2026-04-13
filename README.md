# 📺 YouTube Video Analysis — India Trending Data

An exploratory data analysis (EDA) project that digs into India's YouTube trending videos dataset to uncover patterns in views, likes, dislikes, comments, and channel performance.

---

## 📌 Project Overview

This project analyses the `India_youtube_trending_data.csv` dataset to answer questions like:

- Which YouTube channels trend the most in India?
- What categories dominate the trending page?
- Is there a relationship between views, likes, and dislikes?
- How many trending videos have comments or ratings disabled?

---

## 📂 Project Structure

```
Youtube_video_Analysis/
├── Youtube_video_Analysis.ipynb   # Main analysis notebook
├── India_youtube_trending_data.csv  # Dataset (not included — see below)
└── README.md
```

---

## 🛠️ Technologies Used

| Tool | Purpose |
|---|---|
| Python | Core language |
| Pandas | Data loading, cleaning, manipulation |
| NumPy | Numerical operations |
| Matplotlib | Plotting and visualisation |
| Seaborn | Statistical data visualisation |

---

## 📊 Analysis Performed

### 🔍 Data Cleaning
- Checked dataset shape and structure
- Identified and calculated percentage of missing values
- Filled missing `channelTitle` values with `"Unknown"`
- Dropped irrelevant columns: `channelId`, `thumbnail_link`, `description`, `tags`

### 📈 Exploratory Analysis
- Counted unique video IDs and channel titles
- Aggregated views, likes, dislikes, and comment counts per channel
- Identified top 25 channels by total view count

### 📉 Visualisations
- **Top Trending YouTube Categories in India** — horizontal bar chart by category ID
- **Views vs. Likes** — scatter plot on log scale to show engagement correlation
- **Likes vs. Dislikes** — scatter plot on log scale
- **Comments Disabled Distribution** — bar chart (enabled vs. disabled)
- **Top 10 Most Trending Channels** — bar chart by number of trending videos
- **Ratings Disabled** — pie chart showing percentage breakdown

---

## 🚀 Getting Started

### Prerequisites

Make sure you have Python 3.x installed, then install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn
```

### Running the Notebook

1. Clone or download this repository.
2. Place the `India_youtube_trending_data.csv` file in the same directory as the notebook.
3. Launch Jupyter Notebook:

```bash
jupyter notebook Youtube_video_Analysis.ipynb
```

4. Run all cells from top to bottom (`Cell > Run All`).

---

## 📁 Dataset

The dataset used is **India YouTube Trending Data**, which can be found on [Kaggle](https://www.kaggle.com/datasets/datasnaek/youtube-new).

Key columns include:

| Column | Description |
|---|---|
| `video_id` | Unique identifier for each video |
| `channelTitle` | Name of the YouTube channel |
| `categoryId` | Numeric category of the video |
| `view_count` | Total views |
| `likes` | Total likes |
| `dislikes` | Total dislikes |
| `comment_count` | Total comments |
| `comments_disabled` | Whether comments are turned off |
| `ratings_disabled` | Whether ratings are turned off |

---

## 💡 Key Insights

- A small number of channels dominate the trending page repeatedly.
- Views and likes show a strong positive correlation.
- The majority of trending videos have comments and ratings enabled.
- Certain category IDs appear far more frequently in trending than others.

---

## 🙋 Author

Made as a data analysis learning project.  
Feel free to fork, extend, or build on it!
