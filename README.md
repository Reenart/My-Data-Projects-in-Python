## Can Music Boost Productivity in Physically Demanding Jobs? A Data-Driven Study.

This project investigates whether playing music during overnight housekeeping shifts can help reduce work completion time.
It is a self-initiated, real-world data project based on my personal work experience as an international student.

## Project Summary:
I worked a 10PM–6AM physically demanding job, and one night, I played music and felt less stressed, bumped, and fast. 
That sparked a question: **Does music actually help me complete my work faster, or was it just in my head?**

To find out, I collected data every night, whether music was played, how I felt before my shift, when I started and completed tasks, break durations, 
the building conditions, and more. For a job that I quit so many times in my head, this project made  me look forward to showing up at work every night
just to collect data and see what it says about my new adventure. 


What started as a simple curiosity of let me just see what music does to my time, turned into a full-blown data project that included
1. Data cleaning
2. Exploratory analysis
3. Modeling and forecasting
4. Real-world storytelling with Python

##  Tools Used:

- **Python (Jupyter Notebook)**
- pandas, numpy, seaborn, matplotlib
- scikit-learn – Linear Regression & Random Forest Regressor
- statsmodels – OLS Regression, p-value testing

## Workflow:
### 1. **Data Collection**
- Logged daily entries before and after each shift
- Fields included:
  - Music played (Yes/No)
  - Start & end time
  - Feeling (Neutral, Tired, etc.)
  - Cleaning type
  - Building condition
  - Break duration

### 2. **Data Cleaning & Transformation**
- Converted 12-hour clock to 24-hour PM format (e.g., 10:36 → 22:36)
- Handled datetime rollovers (e.g., end time on the next day)
- Engineered:
  - Duration_Mins
  - StartTime_Mins
  - Dummy variables for categorical features

### 3. **Analysis & Insights**
- Compared average work duration with vs without music
- Explored weekly patterns (e.g., Sundays had the most music, Wednesdays had the earliest completions)
- Used bar charts and line plots to visualize trends

### 4. **Modeling**
- **Linear Regression**: to measure magnitude & direction of features
- **Random Forest**: to rank feature importance
- **OLS + p-values**: to test the significance of music’s impact

### 5. **Forecasting**
- Simulated future work durations (with and without music)
- Used worst-case conditions (Detailed cleaning, Neutral mood)
- Predicted durations:
  - With Music: **348.7 mins**
  - Without Music: **349.9 mins**

## Final Results

| Question                               |   Answer                                            
|----------------------------------------|--------------------------------------------------
| **Did music help?**                    | Slightly (~1.2 mins faster)                          
| **Was it statistically significant?**  | No (p = 0.387) 
| **Most impactful features?**           | Break Duration, Start Time, Cleaning Type 
| **Least impactful?**                   | Music, Feeling 

## Biggest takeaway?**                  
I hoped to find that music significantly boosted performance, but the data told a different story. 
It reminded me that while our emotions may shape our expectations, data brings objectivity and clarity.
Moving forward, I plan to explore this further by collecting data from a broader group, especially those 
in physically demanding jobs, to see if the results hold across a larger and more varied sample.

## Reflections
- I started this project to validate a feeling.  
- I ended up building a full analytics pipeline.
- I didn’t just analyze a CSV, I turned a tough job into a story worth telling.  

## This project helped me grow as a:
- Data thinker
- Cleaner of messy time data
- Builder of models
- Honest interpreter of results
- And most of all, it made me fall in love with asking questions and chasing answers with Python.

Insight Images:

Line Chart with Music Impact:
![line chart](https://github.com/user-attachments/assets/e08859fb-eca5-4d1b-bed1-017a9b8b428d)

Linear Regression
![LR](https://github.com/user-attachments/assets/c36bb3ac-1fc6-4534-9800-91aa13d36657)

Random Forest:
![RF](https://github.com/user-attachments/assets/4087d961-f45d-486a-9f57-546f6372b979)

OSL Regression
![OSLR](https://github.com/user-attachments/assets/85a45108-dc0e-4de2-9ba3-beadfaf068ab)
