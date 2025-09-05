# Session 1 Datasets - Product Analytics Foundations

This directory contains curated datasets for practicing product analytics concepts covered in Session 1.

## Dataset Overview

### 1. `skillboost_user_data.csv`
**User-level behavioral and transactional data for SkillBoost platform**

**Use Cases**: AARRR analysis, user segmentation, retention analysis
- **Rows**: 50 users (sample from 15,000 total users)
- **Columns**: 10 features
- **Key Metrics**: Registration patterns, purchase behavior, completion rates, churn analysis

**Column Descriptions**:
- `user_id`: Unique user identifier
- `registration_date`: When user signed up
- `first_course_purchased`: Date of first purchase (NULL if never purchased)
- `last_activity_date`: Most recent platform activity
- `total_courses_purchased`: Lifetime course purchases
- `total_revenue_eur`: Lifetime revenue from user
- `referral_source`: How user discovered platform
- `completion_rate`: Average course completion rate (0-1)
- `trial_completed`: Whether user completed trial period
- `churned`: Whether user has churned (binary)

---

### 2. `skillboost_course_analytics.csv`
**Course-level performance and business metrics**

**Use Cases**: Product performance analysis, revenue optimization, content strategy
- **Rows**: 20 courses
- **Columns**: 11 features  
- **Key Metrics**: Enrollment trends, completion rates, revenue analysis

**Column Descriptions**:
- `course_id`: Unique course identifier
- `course_name`: Course title
- `course_category`: Subject area classification
- `price_eur`: Course price in euros
- `launch_date`: When course was made available
- `total_enrollments`: Total student enrollments
- `completion_rate`: % of enrolled students who finish
- `avg_rating`: Student satisfaction score (1-5)
- `revenue_eur`: Total revenue generated
- `instructor_rating`: Instructor quality score (1-5)
- `difficulty_level`: Course complexity (Beginner/Intermediate/Advanced)

---

### 3. `skillboost_funnel_data.csv`
**Conversion funnel analysis across customer journey**

**Use Cases**: AARRR funnel optimization, conversion rate analysis, UX improvement
- **Rows**: 10 funnel stages
- **Columns**: 6 features
- **Key Metrics**: Stage-by-stage conversion analysis, drop-off identification

**Column Descriptions**:
- `funnel_stage`: Sequential stage number (1-10)
- `stage_description`: What happens at this stage
- `users_entering`: Number of users reaching this stage
- `users_converting`: Number advancing to next stage
- `conversion_rate`: Stage conversion rate (0-1)
- `avg_time_in_stage_hours`: Time spent in this stage
- `drop_off_reasons`: Primary reasons for stage exit

---

### 4. `skillboost_cohort_analysis.csv`
**Monthly cohort retention and revenue patterns**

**Use Cases**: HEART retention metrics, cohort analysis, LTV calculation
- **Rows**: 8 monthly cohorts
- **Columns**: 10 features
- **Key Metrics**: Time-based retention curves, revenue per cohort

**Column Descriptions**:
- `cohort_month`: Month when cohort first signed up
- `cohort_size`: Number of users in cohort
- `month_X_retention`: % still active after X months
- `avg_revenue_per_user`: Average revenue per cohort member
- `churn_month_X`: Churn rate in month X

---

## Usage Instructions

### Loading Data in Python
```python
import pandas as pd

# Load datasets
users_df = pd.read_csv('datasets/session_01/skillboost_user_data.csv')
courses_df = pd.read_csv('datasets/session_01/skillboost_course_analytics.csv')
funnel_df = pd.read_csv('datasets/session_01/skillboost_funnel_data.csv')
cohorts_df = pd.read_csv('datasets/session_01/skillboost_cohort_analysis.csv')

# Parse dates
users_df['registration_date'] = pd.to_datetime(users_df['registration_date'])
users_df['first_course_purchased'] = pd.to_datetime(users_df['first_course_purchased'])
```

### Key Analysis Opportunities

**AARRR Framework Applications**:
- **Acquisition**: Analyze `referral_source` effectiveness
- **Activation**: Study trial completion vs purchase patterns
- **Retention**: Use cohort data for retention curve analysis
- **Referral**: Calculate viral coefficients from organic traffic
- **Revenue**: Analyze LTV, ARPU, and unit economics

**HEART Framework Applications**:
- **Happiness**: Course ratings and completion satisfaction
- **Engagement**: Activity patterns and session frequency
- **Adoption**: Feature usage and course category preferences
- **Retention**: Multi-timeframe cohort analysis
- **Task Success**: Course completion rates and learning outcomes

**North Star Metrics**:
- Compare potential metrics: MAU vs Learning Hours vs Skills Completed
- Analyze metric correlations with business outcomes
- Design measurement frameworks around chosen North Star

---

## Data Quality Notes

- **Realistic Patterns**: Data includes natural business patterns (seasonality, churn curves, etc.)
- **Missing Values**: Some users have NULL purchase dates (never purchased)
- **Anonymization**: All personally identifiable information has been removed
- **Scale**: Sample datasets represent larger population patterns
- **Time Range**: Data spans March 2024 - September 2024 (6 months)

---

## Integration with Lab Exercises

These datasets directly support all Lab 1 exercises:
- **Part A**: AARRR calculations using user and funnel data
- **Part B**: HEART metrics design with course performance data  
- **Part C**: North Star evaluation using cohort and revenue data
- **Part D**: Integrated analytics using all datasets combined

The data is designed to reveal realistic product analytics challenges and opportunities that mirror real-world scenarios.