 # 📊 Layoffs Data Cleaning & Analysis Project (SQL | Databricks)

## 📖 The Story Behind This Project

Imagine getting a raw dataset about global layoffs; messy, inconsistent, full of duplicates, missing values, and wrong formats.

That’s exactly what I started with.

No structure. No clean dates. Duplicate records everywhere. Some values missing. Some completely unusable.

So I treated it like I would treat a real-world analytics problem.

My goal wasn’t just to analyse the data; it was to understand it first, then clean it second, extract meaningful insights to support better decision-making across different organisations for future strategies. 



## 🧹 Step 1: Cleaning the data

Before any analysis, I had to clean the dataset:

- Removed duplicate records using window functions 
- Standardized inconsistent values like industry and country names
- Fixed messy text 
- Handled missing and incorrect values 
- Converted everything into proper data types

At this point, the dataset finally became usable.



## 📊 Step 2: Exploring the Data

Once the data was clean, I started asking questions:

- Which companies had the highest layoffs?
- Which industries were most affected?
- Which countries were impacted the most?
- How did layoffs change over time?

I used SQL aggregations and grouping to uncover trends in the data.


## 🔥 Step 3: Finding Deeper Insights

Then I went deeper:

- Ranked companies by layoffs using `DENSE_RANK()`
- Identified the Top 5 companies per year
- Analyzed rolling layoffs over time using window functions
- Tracked how layoffs evolved month by month

This is where the data started telling a story.



## 💡 What I Discovered

- A small number of companies contributed to a large portion of layoffs  
- Certain industries were hit much harder than others  
- Layoffs peaked during specific time periods  
- Economic downturns were clearly reflected in the data  



## 🛠️ Tools I Used
- SQL (Databricks)
- Window Functions
- CTEs
- Data Cleaning Techniques
- Time Series Analysis



## 🚀 Key Take Aways

While some companies appear to have very high total layoffs, the impact must be interpreted in relation to company size.

A large absolute layoff number does not always mean a larger impact  bigger companies naturally have larger workforces, so their layoffs may represent a smaller proportion of their total employees.

This pattern is clearly visible in the dataset:

- Google (2023) and Microsoft (2023) both recorded ~10,000–12,000 layoffs, but their impact is relatively lower due to their large global workforce.
In contrast, Katerra (2021) lost 2,434 employees, which represents 100% of its workforce, indicating complete shutdown.

- Due to the COVID-19 pandemic in 2020, many companies experienced increased layoffs by early 2023.
  
- Industries with the Most Layoffs: Consumers & retail were hit hard, likely due to office closures during the pandemic.
  
- Countries with the Most Layoffs: The United States had the most layoffs, with 256,420.
 
- Locations with the Most Layoffs: The SF Bay Area had the highest number, with 125,551, likely due to higher COVID-19 cases.

## Suggestion Strategy

- Provide specialized assistance programs for industries such as retail, transportation, and real estate, including financial aid packages, retraining programs, and staff retention incentives.
  
- Implement early warning systems and trend tracking to anticipate and address possible layoff surges, allowing for proactive measures to lessen the effects.
