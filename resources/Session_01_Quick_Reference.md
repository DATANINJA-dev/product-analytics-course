# Session 1 Quick Reference Guide
**Product Analytics Foundations - Key Concepts & Formulas**

---

## AARRR Framework Reference

### Key Metrics & Formulas

**Acquisition**
- `Conversion Rate = New Users / Total Visitors`
- `Cost Per Acquisition (CPA) = Marketing Spend / New Users`
- `Channel Effectiveness = (Users × Quality Score) / Cost`

**Activation**
- `Activation Rate = Activated Users / New Users`
- `Time to Activation = Median Time from Signup to First Value`
- `Activation Quality = % of Activated Users who Complete Key Action`

**Retention** 
- `N-Day Retention = Users Active on Day N / Users from Cohort`
- `Churn Rate = Users Lost / Total Users at Period Start`
- `Cohort Retention = Users Active in Period / Cohort Size`

**Referral**
- `Viral Coefficient (k) = Invites per User × Invite Accept Rate × Conversion Rate`
- `Referral Rate = Referred Users / Total New Users`
- `Net Promoter Score (NPS) = % Promoters - % Detractors`

**Revenue**
- `ARPU = Total Revenue / Number of Users`
- `LTV = ARPU / Churn Rate` (simplified)
- `LTV:CAC Ratio = Customer Lifetime Value / Customer Acquisition Cost`
- `Monthly Recurring Revenue (MRR) = Sum of Monthly Subscriptions`

---

## HEART Framework Reference

### Goals → Signals → Metrics (GSM) Process

| HEART Dimension | Goal Example | Signal Example | Metric Example |
|-----------------|--------------|----------------|----------------|
| **Happiness** | Users love the product | High ratings, positive reviews | NPS, 5-star ratings % |
| **Engagement** | Users actively use product | Sessions, interactions | DAU/MAU, Session duration |
| **Adoption** | Users try new features | Feature usage events | % users using feature |
| **Retention** | Users come back regularly | Return visits | Day-1, Day-7, Day-30 retention |
| **Task Success** | Users accomplish their goals | Successful completions | Task completion rate, Error rate |

### Implementation Framework
1. **Define Goals**: What user behavior indicates success?
2. **Identify Signals**: How does that behavior manifest?
3. **Choose Metrics**: How can we measure those signals?
4. **Set Targets**: What represents good performance?
5. **Track Over Time**: Monitor trends and changes

---

## North Star Metrics Reference

### IMPACT Evaluation Framework

| Dimension | Definition | Key Questions |
|-----------|------------|---------------|
| **Impact** | Captures meaningful customer value | Does this metric represent real user benefit? |
| **Measurable** | Can be tracked accurately | Do we have reliable data sources? |
| **Predictive** | Indicates future business success | Does this predict revenue/growth? |
| **Actionable** | Teams can influence through actions | Can product/marketing teams move this? |
| **Controllable** | Company has direct influence | Is this within our control vs external factors? |
| **Timely** | Provides fast feedback | Can we see changes quickly after actions? |

### Common North Star Patterns by Industry

**SaaS/B2B**: Weekly Active Users, Feature Adoption Rate, Customer Health Score
**E-commerce**: Gross Merchandise Value, Repeat Purchase Rate, Cart Completion Rate  
**Content/Media**: Content Consumption Hours, Engagement Rate, Content Creation Rate
**Social**: Messages Sent, Connections Made, Time Spent in App
**EdTech**: Learning Hours, Skills Mastered, Course Completion Rate

---

## Python Code Snippets

### AARRR Calculations
```python
# Conversion Rate
def calculate_conversion_rate(converted_users, total_visitors):
    return converted_users / total_visitors

# Simple LTV
def calculate_ltv_simple(arpu, churn_rate):
    return arpu / churn_rate

# Cohort Retention
def cohort_retention_rate(active_users_period_n, original_cohort_size):
    return active_users_period_n / original_cohort_size
```

### HEART Metrics Setup
```python
# Engagement Score
def calculate_engagement_score(sessions_per_user, avg_session_duration, feature_usage_rate):
    # Weighted engagement score (customize weights based on business)
    return (sessions_per_user * 0.4) + (avg_session_duration * 0.3) + (feature_usage_rate * 0.3)

# Task Success Rate
def task_success_rate(successful_completions, total_attempts):
    return successful_completions / total_attempts
```

### Data Visualization Templates
```python
import matplotlib.pyplot as plt
import seaborn as sns

# Funnel Visualization
def plot_conversion_funnel(stages, users):
    plt.figure(figsize=(10, 6))
    plt.plot(stages, users, marker='o', linewidth=3)
    plt.xlabel('Funnel Stage')
    plt.ylabel('Users')
    plt.title('Conversion Funnel Analysis')
    
# Cohort Heatmap
def plot_cohort_heatmap(cohort_data):
    plt.figure(figsize=(12, 8))
    sns.heatmap(cohort_data, annot=True, fmt='.0%', cmap='YlOrRd')
    plt.title('Cohort Retention Heatmap')
```

---

## Common Mistakes to Avoid

### AARRR Pitfalls
- ❌ Focusing only on acquisition without activation
- ❌ Measuring vanity metrics instead of actionable metrics  
- ❌ Ignoring the relationship between stages
- ✅ Optimize the biggest constraint in your funnel first

### HEART Pitfalls  
- ❌ Too many metrics without clear priorities
- ❌ Metrics that teams can't influence
- ❌ Focusing on outputs vs outcomes
- ✅ Start with user goals, work backward to metrics

### North Star Pitfalls
- ❌ Choosing metrics that plateau quickly
- ❌ Optimizing metrics that don't drive business value
- ❌ Having different North Stars for different teams
- ✅ Ensure your North Star aligns with customer value AND business outcomes

---

## Industry Benchmarks

### SaaS/EdTech Benchmarks (Approximate)
- **Trial Conversion**: 15-25%
- **Month-1 Retention**: 70-85%  
- **Month-6 Retention**: 30-50%
- **NPS Score**: 30+ (good), 50+ (excellent)
- **LTV:CAC Ratio**: 3:1 (minimum), 5:1+ (healthy)

### Funnel Benchmarks
- **Website to Trial**: 2-5%
- **Trial to Paid**: 15-25%
- **Paid to Active**: 60-80%
- **New User Activation**: 20-40%

*Note: Benchmarks vary significantly by industry, product complexity, and customer segment*

---

## Useful Resources

### Tools & Platforms
- **Analytics**: Amplitude, Mixpanel, PostHog, Google Analytics
- **A/B Testing**: Optimizely, VWO, LaunchDarkly
- **Customer Feedback**: Hotjar, FullStory, Intercom
- **Data Visualization**: Tableau, Looker, Python (matplotlib/seaborn)

### Further Reading
- "Lean Analytics" by Alistair Croll & Benjamin Yoskovitz
- "The Lean Startup" by Eric Ries  
- "Hooked" by Nir Eyal
- Google's HEART Framework Documentation
- Amplitude's Product Analytics Playbook

---

*This guide complements the detailed notebooks and should be used as a quick reference during analysis work.*