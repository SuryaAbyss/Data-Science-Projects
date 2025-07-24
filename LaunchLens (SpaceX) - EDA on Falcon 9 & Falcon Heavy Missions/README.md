# 🚀 LaunchLens: EDA on Falcon 9 & Falcon Heavy Missions

## 📌 Project Overview
**LaunchLens** is an exploratory data analysis (EDA) project focused on the launch history of SpaceX's Falcon 9 and Falcon Heavy rockets. By analyzing multiple datasets, we aim to understand trends in launch frequency, customer profiles, orbit destinations, and booster recovery outcomes.

---

## 📂 Dataset Sources
- [Dataset 1 - Falcon 9 Launches (Kaggle)](https://www.kaggle.com/datasets/sagarvarandekar/spacex-falcon9-launch-data)  
- [Dataset 2 - Falcon 9 & Heavy (Kaggle)](https://www.kaggle.com/datasets/heyrobin/space-x-launches-falcon9-and-falcon-heavy)

---

## 🚀 About the Rockets

### 🛰️ **Falcon 9**  
A partially reusable medium-lift launch vehicle, capable of transporting cargo and crew to low Earth orbit and the International Space Station (ISS).

### 🚀 **Falcon Heavy**  
A heavy-lift vehicle developed from Falcon 9, with more thrust and larger payload capabilities. It's one of the most powerful rockets ever built.

---

## 🧰 Imports & Setup

```python
import matplotlib.pyplot as plt
import seaborn as sns
import plotly.express as px

# Custom color palette
class clr:
    S = '\033[1m' + '\033[96m'
    E = '\033[0m'

my_colors = ["#094074", "#3C6997", "#9900F0", "#FFD124", "#FE9000"]

print(clr.S + "Notebook Color Scheme: " + clr.E)
sns.palplot(sns.color_palette(my_colors))
````

---

## 🗃️ Dataset Exploration

### 🔍 Summary Statistics

```python
df.describe()
```

![describe](https://user-images.githubusercontent.com/63750425/185083629-0fb48238-b48e-476c-b7e2-90a8ef7190bf.png)

### 📄 Sample Data Preview

```python
df.head()
```

![head](https://user-images.githubusercontent.com/63750425/185083786-69004259-5af5-46ac-bcb3-392d748f24cd.png)

---

## 🛰️ Key Exploratory Visuals

### 📍 Launch Site Distribution

```python
launch_site = df['LaunchSite'].value_counts()
launch_site
```

![launch-site](https://user-images.githubusercontent.com/63750425/185083880-17f679cf-0e69-4779-8373-cdd2655af336.png)

---

### 🌐 Orbit Type Frequency

```python
plt.figure(figsize = (15,8))
most_orbit = df['Orbit'].value_counts()
most_orbit.plot(kind = "barh", color = my_colors[1])
plt.show()
```

![orbit](https://user-images.githubusercontent.com/63750425/185083994-80b390f4-7b3b-4c88-be12-d2d9d41fd5fd.png)

---

### 🧑‍💼 Most Frequent Customers

```python
plt.figure(figsize = (15,8))
Most_customers.plot(kind = 'bar', color = my_colors[2])
plt.show()
```

![customers](https://user-images.githubusercontent.com/63750425/185084091-7c13dc51-767a-429f-aa90-77ba2649164b.png)

---

### 🛬 Booster Landing Outcomes

```python
outcomes_of_landing = df1['Booster_landing'].value_counts()
plt.figure(figsize = (15,8))
outcomes_of_landing.plot(kind = 'pie')
plt.show()
```

---

### 🚀 Booster Version vs Landing Outcome

```python
plt.figure(figsize=(40,20))
year_club = df1.groupby(['Booster_landing', 'Version, Booster']).Booster_landing.size().head(20).plot(kind = 'pie')
plt.title('Booster_landing VS Version, Booster')
plt.legend()
plt.show()
```

![booster](https://user-images.githubusercontent.com/63750425/185084232-28a972c1-810b-4366-9747-8b2bad4f4cf5.png)

---

## 💬 Quote

> *"If humanity doesn't land on Mars in my lifetime, I would be very disappointed."*
> — **Elon Musk**

---

### 👨‍💻 Made with 🚀 by **Surya Prakash**
