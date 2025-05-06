# Olympics-History-EDA-Project

## Project Overview

This project performs **Exploratory Data Analysis (EDA)** on 120 years of Olympic history from Athen 1896 to Rio 2016 data to uncover trends and patterns in history of Olympics. We use libraries like **Pandas, Numpy, Matplotlib, Seaborn** for cleaning, visualization, and analysis. 


![pexels-pixabay-236937](https://github.com/user-attachments/assets/b399dedc-87c5-49ce-8baa-80a90113dadd)

---

## 🎯 Objective

This Exploratory Data Analysis (EDA) on Olympic history from 1896 to 2016 provided valuable insights into the evolution of the Games over more than a century. Here are the key takeaways:
### Participation Trends
- The Olympics have grown massively in scale, with significant increases in the number of participating athletes, countries, and events.
- Major dips in participation align with historical events like World Wars.

### Gender-Based Analysis
- Female participation has increased significantly, especially from the 1980s onward.
- The gender gap is closing, but some sports still show disparity.

### Country-wise Performance
- The USA has consistently been a top-performing nation, along with Russia, Germany, and China in recent years.
- Medal distribution highlights global power shifts and the influence of hosting.

### Sports and Events Evolution
- The number of sports and events has grown steadily, reflecting the inclusion of new disciplines and increased athlete specialization.
- Some events have been discontinued, while others have gained prominence.
- 
---

## 📁 Dataset

The dataset contains **271116** rows and **17** columns , including:
1. athlete_events.csv
This dataset contains athlete-level event data for every Olympic game from 1896 to 2016.

- **ID**	Unique identifier for each athlete
- **Name**	Athlete's full name
- **Sex**	Gender: 'M' (Male), 'F' (Female)
- **Age**	Age of the athlete during the event
- **Height**	Height in centimeters
- **Weight**	Weight in kilograms
- **Team**	Country or team name
- **NOC**	National Olympic Committee code (e.g., USA, GBR)
- **Games**	Year + Season (e.g., "2016 Summer")
- **Year**	Year of the Olympics
- **Season**	Summer or Winter
- **City**	Host city
- **Sport**	The sport category (e.g., Athletics, Swimming)
- **Event**	Specific event name (e.g., 100m Men)
- **Medal**	Medal won: Gold, Silver, Bronze, or blank if none

2. noc_regions.csv
   
This file maps NOC codes to country names and regions. It helps normalize and aggregate data by region.
- **NOC**	National Olympic Committee code
- **region**	Country or region name (e.g., "United States", "Germany")
- **notes**	Additional information (sometimes empty)

---

## Steps and Workflow

### 1. Define Objectives
**Identify what you want to explore.**
- Trends in participation, top countries, gender distribution, sport evolution, etc.

### 2. Load the Data
- Import required libraries: pandas, numpy, matplotlib, seaborn.
- Load athlete_events.csv and noc_regions.csv using pd.read_csv().

### 3. Understand the Data
- Use .head(), .info(), .describe() to inspect structure, data types, and summary stats.
- Check missing values: df.isnull().sum().
- Explore unique values in key columns (e.g., Sport, Year, Medal).

### 4. Data Cleaning & Preparation
- Handle missing values (e.g., Age, Height, Medal).
- Merge datasets on NOC to enrich country info.
- Remove or manage duplicates (especially for medal counts and team events).


### 5. EDA (Exploratory Data Analysis)
📈 a. Participation Trends
- Track how number of athletes, countries, and events changed over time.

🏅 b. Country-wise Performance
- Total medals by country.
- Top 10 medal-winning countries.
- Group medals by Gold, Silver, Bronze.

🚻 c. Gender Analysis
- Participation of male vs. female athletes across years.
- Medal distribution by gender.

🏋️ d. Sport & Event Evolution
- Track how many unique sports and events appeared over time.
- Highlight new or discontinued sports.

### 6. Data Visualization
Used Matplotlib and Seaborn for:
- **Lineplot**: To see correlations among `price`, `availability`, and `number of reviews`.
- **Heatmap**: Showing correlations among numerical features.
- **Histograms and Boxplots**: To detect outliers in `price`.
- **Bar Charts**: Displaying room types and neighborhood group distributions.

---

## Key Findings and Insights

1. **Bar Plot** – Shows the top 10 countries with the highest athlete participation.

2. **Histogram** – Depicts the age distribution of Olympic athletes.

3. **Pie Chart** – Illustrates the gender (male vs. female) distribution among participants.

4. **Bar Chart** – Visualizes the gap in male-female participation ratios across different years.

5. **Seaborn Plots** – Several visualizations utilize Seaborn for enhanced styling and statistical representations.

---

## Future Work

1. Time-Series Analysis:
- Deeper trends in participation, medals, and gender distribution over the decades.
- Analyzing the impact of global events (e.g., World Wars, pandemics) on Olympic data.

2. Geographical Analysis:
- Mapping medal distributions or athlete participation geographically using tools like Plotly or Folium.
- Identifying regional dominance in specific sports.

3. Medal Prediction Models:
- Building machine learning models to predict medal outcomes based on factors like age, country, sport, and past performance.

4. Sport-Specific Insights:
- Analyzing trends and participation in individual sports to identify rising or declining popularity.

5. Athlete Career Tracking:
- Investigating athlete longevity, multiple participations, and performance improvements over time.

6. Equity and Inclusion Analysis:
- Further breakdowns by gender, country income level, and continent to assess diversity and inclusion in the Olympics. 

---

## Conclusion

Olympic EDA reveals dominant countries, peak athlete ages (20–30), rising gender equality, and growing global participation over time.

---
