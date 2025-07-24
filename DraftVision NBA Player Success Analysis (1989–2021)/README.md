### **"DraftVision: NBA Player Success Analysis (1989–2021)"**

````markdown
# 🏀 DraftVision: NBA Player Success Analysis (1989–2021)

## 📌 Overview
**DraftVision** is a data visualization and statistical analysis project that explores NBA Draft data from 1989 to 2021. It uncovers trends in player performance based on their draft pick position, career longevity, and overall contribution to the league.

The dataset, included in this repository, has been cleaned and visualized using Python libraries like Pandas, Plotly, and Seaborn. The goal is to answer questions like:  
- Do higher picks always perform better?  
- Where were the greatest NBA scorers drafted?  
- Which draft positions provide the most value over time?

---

## 🧰 Libraries Used

```python
import numpy as np 
import pandas as pd
import seaborn as sns
from matplotlib import pyplot as plt
from mpl_toolkits.basemap import Basemap
import warnings
%matplotlib inline
sns.set(style="white", context="talk")
warnings.simplefilter(action='ignore', category=FutureWarning)
warnings.filterwarnings("ignore", category=plt.cbook.mplDeprecation)
````

---

## 🗂️ Dataset Preview

```python
data.head()
```

![Dataset Head](https://user-images.githubusercontent.com/77057546/187243516-e9df2faa-0e0f-4e21-90f0-9c7a2d437a4b.png)

---

## 📊 Key Visualizations & Analysis

### 🔢 Total Points Scored by Overall Pick and Year

A 3D scatter plot shows how draft year and pick position relate to total career points for players with over 250 games played.

![3D Scatter](https://user-images.githubusercontent.com/77057546/187245172-71f25c92-b821-4162-97d1-8be97dc8c7ec.png)

---

### 📉 Performance Breakdown for Picks 1-60

Bar charts summarize total minutes, games, years active, points, win shares, and value over replacement for each pick position.

![Bar Charts](https://user-images.githubusercontent.com/77057546/187245743-549339f5-cdaf-4dc4-bd63-0cd8091a2dea.png)

---

### 🧮 Points Per Game by Year and Pick

Analyzes how points per game vary across draft picks and years, showing standout performers in lower or higher picks.

![Scatter](https://user-images.githubusercontent.com/77057546/187245914-d3133d5e-5ad2-4977-afde-a0252536a07c.png)

---

### 🔥 Top 100 NBA Draft Scorers

Identifies the top 100 draft picks by total points, revealing where some of the greatest scorers came from.

![Top Scorers](https://user-images.githubusercontent.com/77057546/187246124-962d5396-3d5e-407c-aac9-9b4cccd9f862.png)

---

### 🎯 Average Points for Top 3 Picks

Violin plots compare the average points per game of picks 1, 2, and 3 to see which spot delivers the most offensive impact.

![Violin Plot](https://user-images.githubusercontent.com/77057546/187246303-4f9b3f28-f37a-4d4e-a984-1c02c00686d8.png)

---

### 📦 Box Plus Minus by Overall Pick

Evaluates player impact using Box Plus Minus and how it correlates with draft position.

![BPM Chart](https://user-images.githubusercontent.com/77057546/187246541-28f16348-75a2-4bff-a056-7b094ddbad5e.png)

---

### 📈 Value Over Replacement

Ranks players by their Value Over Replacement (VORP), a metric of overall contribution compared to a league-average replacement.

![VORP Chart](https://user-images.githubusercontent.com/77057546/187246729-35f21301-471b-4571-86a6-00824d8e25e6.png)

---

### 🎥 Animated 3D Scatter: Pick 1-60 by Year

Watch how the scoring performance of picks evolves over time using an animated 3D scatter plot.

[https://user-images.githubusercontent.com/77057546/187247740-7a3bdc9d-4233-406c-a385-37bf602073be.mp4](https://user-images.githubusercontent.com/77057546/187247740-7a3bdc9d-4233-406c-a385-37bf602073be.mp4)

---

## 💡 Conclusion

**DraftVision** highlights that draft position doesn't always predict career success. While top picks often perform well, many lower picks have become all-time greats. Through interactive visualizations, this project sheds light on value, efficiency, and scoring power across decades of NBA drafts.

---

### 👨‍💻 Created by Surya Prakash

