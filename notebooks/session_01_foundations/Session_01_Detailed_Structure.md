# Session 1: Product Analytics Foundations - Detailed Structure

## **Learning Objectives**
By the end of this session, student will be able to:
1. Explain key differences between AARRR, HEART, and North Star frameworks
2. Select appropriate framework based on product type and business context
3. Implement basic analytics tracking setup in Python
4. Analyze real-world framework selection decisions

## **Materials Needed**
- Main session notebook: `01_Product_Analytics_Foundations.ipynb`
- Python environment with pandas, matplotlib, seaborn
- Framework comparison chart (visual aid)
- Real company case study materials

## **Detailed Timeline (90 minutes)**

### **🚀 Opening & Context Setting (5 minutes)**
**Time: 0:00 - 0:05**

**Content:**
- Welcome and session overview
- Quick context: "Why do successful products need analytics frameworks?"
- Preview of what we'll cover and how it applies to real work

**Instructor Notes:**
- Start with energy and relevance
- Connect to Diogo's background immediately
- Set expectation for interactive session

---

### **📋 Problem Statement: Why Product Analytics Frameworks? (5 minutes)**
**Time: 0:05 - 0:10**

**Content:**
- **The Problem**: Most companies track everything but measure nothing meaningful
- **Data Overwhelm**: 100+ metrics but no clear north star
- **Decision Paralysis**: Teams arguing over which metrics matter
- **Business Impact**: How wrong metrics lead to wrong product decisions

**Real Examples:**
- Startup that tracked 50 vanity metrics but missed churn warning signs
- Product team that optimized for page views instead of user value

**Key Insight:** *"You can't optimize what you can't measure, but measuring everything optimizes nothing"*

---

### **⚓ AARRR Framework Deep Dive (15 minutes)**
**Time: 0:10 - 0:25**

**Content Structure:**

#### **What is AARRR? (3 minutes)**
- **A**cquisition: How users find you
- **A**ctivation: First meaningful experience  
- **R**etention: Users coming back
- **R**eferral: Users bringing others
- **R**evenue: Monetization and growth

#### **When to Use AARRR (4 minutes)**
- **Best For:**
  - Early-stage startups
  - Growth-focused products
  - Products with clear user journey
  - Teams needing full-funnel visibility

- **Not Ideal For:**
  - Mature products with established user base
  - Complex B2B products with long sales cycles
  - Products where UX quality matters more than growth metrics

#### **Real Company Examples (5 minutes)**
- **Airbnb**: How they used AARRR to scale from startup to global platform
- **Dropbox**: Referral program optimization using AARRR framework
- **Startup Case Study**: How a SaaS company identified activation bottleneck

#### **AARRR Metrics Examples (3 minutes)**
- Acquisition: CAC by channel, organic vs paid traffic
- Activation: Time to first value, onboarding completion rate
- Retention: DAU/MAU, cohort retention curves
- Referral: Viral coefficient, referral conversion rate
- Revenue: LTV, MRR growth, revenue per user

**Interactive Element:** Ask Diogo to think of his product and identify one metric for each AARRR stage

---

### **❤️ HEART Framework Deep Dive (15 minutes)**
**Time: 0:25 - 0:40**

**Content Structure:**

#### **What is HEART? (3 minutes)**
- **H**appiness: User satisfaction and sentiment
- **E**ngagement: Level of user involvement
- **A**doption: New feature/product uptake
- **R**etention: Rate of returning users
- **T**ask Success: Efficiency of user goal completion

#### **When to Use HEART (4 minutes)**
- **Best For:**
  - UX-focused products (Google, design tools)
  - Mature products optimizing experience
  - Products where user satisfaction drives retention
  - Complex products with multiple user flows

- **Not Ideal For:**
  - Early-stage products prioritizing growth
  - Simple products with obvious user paths
  - Products where revenue is primary concern

#### **Real Company Examples (5 minutes)**
- **Google**: How they measure search quality with HEART
- **YouTube**: Balancing engagement metrics with user satisfaction
- **Spotify**: Using HEART to optimize music discovery experience

#### **HEART Metrics Examples (3 minutes)**
- Happiness: NPS score, user satisfaction surveys, app store ratings
- Engagement: Session duration, interactions per visit, feature usage depth
- Adoption: Feature discovery rate, new feature activation
- Retention: Daily/weekly/monthly active users, churn rate
- Task Success: Completion rate, error rate, time on task

**Interactive Element:** Compare AARRR vs HEART for the same product - what different insights would you get?

---

### **🌟 North Star Framework + Decision Tree (5 minutes)**
**Time: 0:40 - 0:45**

**Content Structure:**

#### **What is North Star? (2 minutes)**
- Single metric that captures core product value
- Aligns entire organization around one goal
- Leading indicator of long-term success
- Balances user value with business value

#### **North Star Examples (2 minutes)**
- **Spotify**: Time spent listening
- **WhatsApp**: Messages sent
- **Airbnb**: Nights booked
- **LinkedIn**: Monthly active professionals

#### **Framework Decision Tree (1 minute)**
```
Product Stage?
├── Early Stage → AARRR (growth focus)
├── Growth Stage → North Star + AARRR (alignment + growth)
└── Mature Stage → HEART (experience optimization)

Primary Business Goal?
├── User Acquisition → AARRR
├── User Experience → HEART  
└── Team Alignment → North Star

Product Complexity?
├── Simple User Journey → North Star
├── Complex Multi-Flow → HEART
└── Clear Funnel → AARRR
```

---

### **🛠️ Workshop: Framework Selection Exercise (20 minutes)**
**Time: 0:45 - 1:05**

**Exercise Structure:**

#### **Setup (2 minutes)**
Present 3 different product scenarios:
1. **New fintech app** (6 months old, pre-Series A)
2. **Established B2B SaaS** (3 years, 1000+ customers) 
3. **Consumer social platform** (Series B, engagement challenges)

#### **Individual Analysis (6 minutes)**
Diogo analyzes each product:
- What stage is the product in?
- What's the primary business challenge?
- Which framework would you choose and why?
- What would be your top 3 metrics for each?

#### **Discussion & Guided Analysis (12 minutes)**
- Review Diogo's framework selections
- Discuss reasoning and alternative approaches
- Explore edge cases and framework combinations
- Connect to Diogo's real work experience

**Learning Reinforcement:** Focus on *why* certain frameworks fit certain contexts

---

### **💻 Python: Metrics Tracking Setup (15 minutes)**
**Time: 1:05 - 1:20**

**Practical Implementation:**

#### **Code Walkthrough (8 minutes)**
```python
# Basic analytics tracking simulation
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

# Simulate user behavior data for AARRR analysis
def generate_user_data(n_users=1000):
    # Create sample data representing user journey
    
# Framework-specific metric calculations
def calculate_aarrr_metrics(data):
    # Implementation for each AARRR stage
    
def calculate_heart_metrics(data):
    # Implementation for each HEART dimension
    
def calculate_north_star_candidate(data, metric_type):
    # North star metric calculation
```

#### **Hands-On Exercise (7 minutes)**
- Diogo executes code step-by-step
- Modifies parameters to see impact on metrics
- Discusses how this connects to real analytics implementation
- Q&A on technical implementation challenges

**Focus:** Not on complex coding, but on understanding how frameworks translate to measurable metrics

---

### **💬 Q&A + Discussion (5 minutes)**
**Time: 1:20 - 1:25**

**Discussion Topics:**
- How does this apply to Diogo's current work context?
- What challenges does he foresee in framework implementation?
- Which framework resonates most with his experience?
- Questions about combining frameworks or transitioning between them

**Instructor Role:** Connect theory to Diogo's practical needs and experience

---

### **📊 Case Study: Slack's North Star Decision (5 minutes)**
**Time: 1:25 - 1:30**

**Live Analysis:**

#### **The Context**
- Slack's early growth was driven by team signups
- Initial metrics focused on user acquisition (typical AARRR approach)
- Realized that signup ≠ value creation

#### **The Decision**
- Shifted to North Star: "Messages sent by teams"
- Why this metric captured core value delivery
- How it changed product development priorities
- Impact on business outcomes

#### **The Learning**
- When to evolve your measurement approach
- How North Star metrics influence product roadmap
- Connecting user behavior to business value

**Wrap-up Question:** "Based on today's session, what would be your North Star metric for a product you know well?"

---

## **Session Materials Checklist**

### **For Instructor:**
- [ ] Main session notebook with all code working
- [ ] Framework comparison visual aid
- [ ] 3 product scenarios for workshop
- [ ] Slack case study materials
- [ ] Timer for keeping sessions on track

### **For Student:**
- [ ] Access to session notebook
- [ ] Python environment setup verified
- [ ] Lab 1 assignment details
- [ ] Framework reference materials

## **Transition to Lab Work**

**End-of-Session Preview:**
- "In Lab 1, you'll apply today's frameworks to 3 real product scenarios"
- "You'll implement the metrics tracking for each framework type"  
- "Come to Session 2 with questions about your framework selections"

## **Success Indicators**

Session is successful if:
- [ ] Diogo can articulate key differences between frameworks
- [ ] He selects appropriate framework for given product scenario with reasoning
- [ ] Python code executes without errors
- [ ] He asks relevant questions about real-world application
- [ ] He's motivated to complete Lab 1 assignment