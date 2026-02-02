# ✈️ Airline Passenger Satisfaction Analysis
## 🎯 Project Overview

This project analyzes **129,880 airline passenger satisfaction records** to identify key drivers of customer experience and provide actionable business recommendations. Using **SQL Server** for data analysis and **Power BI** for visualization, I uncovered critical insights about service quality, customer segments, and operational performance.

**Project Goals:**
- Identify factors affecting passenger satisfaction
- Analyze satisfaction across different customer segments
- Evaluate service quality across 14 touchpoints
- Provide data-driven recommendations for improvement

---

## 📊 Dataset

**Source:** [Maven Analytics Data Playground]([https://mavenanalytics.io/data-playground](https://mavenanalytics.io/data-playground/airline-passenger-satisfaction))  
**Database:** `db_airline`  
**Table:** `dbo.airline_passenger_satisfaction`  
**Records:** 129,880 passengers  

### Data Dictionary

| Column | Type | Description |
|--------|------|-------------|
| ID | Integer | Unique passenger identifier |
| Gender | String | Male/Female |
| Age | Integer | Passenger age |
| Customer_Type | String | First-time / Returning |
| Type_of_Travel | String | Business / Personal |
| Class | String | Business / Economy Plus / Economy |
| Flight_Distance | Integer | Flight distance in miles |
| Departure_Delay | Integer | Departure delay in minutes |
| Arrival_Delay | Integer | Arrival delay in minutes |
| **14 Service Ratings** | Integer | 0-5 scale (0 = Not Applicable) |
| Satisfaction | String | Satisfied / Neutral or Dissatisfied |

---


## 🧹 Data Cleaning (SQL)

The data cleaning process was performed using SQL Server.

Handling Missing Values
- Arrival_Delay initially contained NULL values.
- Based on business context, NULL values were interpreted as flights without delay.
- These NULL values were replaced with 0 using SQL UPDATE statements.
- Validation was performed to ensure no remaining NULL values in delay columns.

Power BI Dashboard
- Import Data From SQL Server
- Created DAX measures (Total Passengers, Satisfaction Rate, etc.)
- Built visualizations with conditional formatting
- Interactive slicers for exploration

---

## 📊 Dashboard Overview (Power BI)

### Executive Overview

**KPI Cards:**
- Total Passengers: 129,880
- Satisfaction Rate: 43.4%
- Overall Service Rating: 3.24 / 5.0

**Visualizations:**
- Satisfaction Distribution (Donut Chart)
  - 56.5% Neutral/Dissatisfied 🔴
  - 43.5% Satisfied 🟢

- Satisfaction by Class (Bar Chart)
  - Business: 69% ✅
  - Economy Plus: 25% ⚠️
  - Economy: 19% ❌

- Satisfaction by Customer Type (Bar Chart)
  - Returning: 48% 🟢
  - First-time: 24% 🔴

- Average Rating by Service - 14 services (Column Chart)

**Interactive Features:**
- Gender slicer
- Age range slicer
- Dynamic filtering

---

## 🔑 Key Insights


### Overall Performance
- **Satisfaction Rate:** 43.45% 
- **Overall Service Rating:** 3.24 / 5.0
- **Status:** ⚠️ Below industry standard (60-70%)

### Critical Findings

#### 1️⃣ **WiFi Service is the Biggest Problem** ❌
- **Rating:** 2.73 / 5.0 (lowest of all services)
- **Impact:** Critical for business travelers (69% of passengers)
- **Action:** Priority 1 for improvement

#### 2️⃣ **First-Time Customers at High Risk** ⚠️
- **First-time Satisfaction:** 22.6%
- **Returning Satisfaction:** 48.0%
- **Gap:** 25.4 percentage points
- **Risk:** Low first-time satisfaction = poor conversion to loyal customers

#### 3️⃣ **Massive Class Disparity** 📊

| Class | Satisfaction Rate | Performance |
|-------|------------------|-------------|
| Business | 69.0% | ✅ Excellent |
| Economy Plus | 24.0% | ⚠️ Poor |
| Economy | 19.2% | ❌ Critical |

---

## 💡 Business Recommendations

### Priority 1: WiFi Infrastructure Upgrade 🌐
**Problem:** Lowest rating (2.73/5.0)  
**Solution:**
- Partner with premium WiFi providers
- Increase bandwidth for Business class
- Offer free WiFi for premium passengers

---

### Priority 2: First-Time Customer Program 🎯
**Problem:** Only 22.6% satisfaction (vs 48% returning)  
**Solution:**
- Welcome email with flight tips
- 10-15% discount on next booking
- Priority customer service
- Post-flight survey with incentive

---

### Priority 3: Economy Class Enhancement 📦
**Problem:** 19.2% satisfaction  
**Solution:**
- Improve food/beverage quality
- Free entertainment upgrade
- Complimentary snacks
- Better amenity kits

---

## 🎓 Key Learnings

### Technical Skills
✅ **SQL:** Complex aggregations, CASE statements, NULL handling  
✅ **Power BI:** DAX measures, data modeling, conditional formatting  
✅ **Data Analysis:** EDA, segmentation, correlation analysis  
✅ **Problem-solving:** Root cause identification

### Business Skills
✅ Strategic thinking & prioritization  
✅ Data-driven decision making  
✅ Stakeholder communication  
✅ Industry domain knowledge


## 🛠 Tools Used

| Tools | Purpose |
|------------|---------|
| **SQL Server** | Database management and analysis |
| **SQL** | Complex queries	 |
| **Power BI** | Interactive dashboards |
| **DAX** | Custom measures  |
| **Excel** | Initial data exploration |

**Key SQL Techniques:**
- Data cleaning (NULL handling)
- Aggregations and GROUP BY
- CASE statements
- Conditional aggregations
- Statistical analysis

**Power BI Features:**
- Star schema data modeling
- DAX measures
- Interactive visualizations
- Conditional formatting
- KPI cards

---

##📎 Notes

This project is intended as a portfolio demonstration for entry-level data analyst roles and focuses on clarity of analysis, business reasoning, and reproducibility rather than advanced statistical modeling.

## 📞 Contact

**Your Name**
- LinkedIn: https://linkedin.com/in/anugrah-seputra-321169280
- Email: anugrahseputra93@gmail.com

