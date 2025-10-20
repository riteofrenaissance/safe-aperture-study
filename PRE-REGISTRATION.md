# AsPredicted Pre-registration
## Safe Aperture Micro-Pilot Study

**Pre-registration Date:** October 2025  
**Study Start Date:** December 1, 2025 (estimated)  
**AsPredicted ID:** #252740  
**GitHub Repository:** https://github.com/riteofrenaissance/safe-aperture-study

---

### 1. Have any data been collected for this study already?
**No**, this is a pre-registration before any data collection.

---

### 2. What's the main question being asked or hypothesis being tested in this study?

**Research Question:**  
Does a 4-week graduated ambiguity tolerance training program (Safe Aperture) increase tolerance of ambiguity compared to a waitlist control condition?

**Primary Hypothesis (H1):**  
Participants randomly assigned to the Safe Aperture intervention will show significantly greater increases in Tolerance of Ambiguity Scale (TAS) scores from baseline to Week 4 compared to waitlist control participants.

**Secondary Hypotheses:**
- H2: Intervention effects will partially persist at 8-week follow-up
- H3: Parallel improvements will be observed in Intolerance of Uncertainty (IUS-12) and anxiety (GAD-7)
- H4 (Exploratory): Participants with moderate baseline anxiety will show larger gains than those with high anxiety

---

### 3. Describe the key dependent variable(s) specifying how they will be measured.

**Primary Outcome:**
- **Tolerance of Ambiguity Scale (TAS)** - McLain 2009
  - 13 items, 5-point Likert scale
  - Measured at: Baseline, Week 4 (post-intervention), Week 8 (follow-up)
  - Scoring: Sum of items (higher = greater tolerance)
  - Change score calculated: Week 4 - Baseline

**Secondary Outcomes:**
- **Intolerance of Uncertainty Scale - Short Form (IUS-12)**
  - 12 items, 5-point Likert
  - Same timepoints as TAS
  - Higher scores = greater intolerance

- **Generalized Anxiety Disorder-7 (GAD-7)**
  - 7 items, 4-point scale (0-3)
  - Same timepoints
  - Total score 0-21

**Process Outcomes:**
- Adherence rate: % of assigned exercises completed
- Satisfaction: 5-item questionnaire (post-intervention only)
- Adverse events: Open-ended weekly reports

---

### 4. How many and which conditions will participants be assigned to?

**N = 30 total participants**

**Two conditions (randomized 1:1):**

1. **Intervention Group (n=15):**
   - Receives Safe Aperture training for 4 weeks
   - Progressive exposure to ambiguous stimuli (Levels 1-3)
   - Daily exercises (10-20 minutes/day)
   - Web-based delivery
   - Weekly check-ins from research assistant

2. **Waitlist Control Group (n=15):**
   - No intervention during 4-week active period
   - Completes same assessments as intervention group
   - Offered intervention after Week 8 follow-up
   - Weekly check-ins from research assistant (for retention)

**Randomization method:**  
Simple randomization using online random number generator after baseline assessment completion.

---

### 5. Specify exactly which analyses you will conduct to examine the main question/hypothesis.

**Primary Analysis:**
- **Independent samples t-test** comparing TAS change scores (Week 4 - Baseline) between intervention and control groups
- **Effect size:** Cohen's d with 95% confidence interval
- **Significance level:** α = 0.05 (two-tailed)
- **Software:** R

**Secondary Analyses:**
1. **Repeated measures ANOVA:**
   - 2 (Group: Intervention vs. Control) × 3 (Time: Baseline, Week 4, Week 8)
   - Separate models for TAS, IUS-12, and GAD-7

2. **Adherence-outcome correlation:**
   - Pearson correlation between % exercises completed and TAS change (intervention group only)

3. **Moderator analysis (Exploratory):**
   - Multiple regression: TAS change ~ Group + Baseline GAD-7 + Group×GAD-7

**Missing Data Handling:**
- Primary analysis: Complete case (participants with baseline AND Week 4 data)
- Sensitivity analysis: Last observation carried forward (LOCF)

**Outliers:**
- Defined as scores >3 SD from group mean
- Analyses reported with and without outliers

---

### 6. Describe exactly how outliers will be defined and handled, and your precise rule(s) for excluding observations.

**Outlier Definition:**
- Statistical outliers: Scores >3 standard deviations from group mean on any outcome variable

**Exclusion Criteria:**

**Pre-randomization exclusions:**
- Age outside 18-65 range
- Non-fluency in English
- Active suicidal ideation
- History of psychotic disorder
- Severe depression (PHQ-9 >20)

**Post-randomization exclusions:**
- None (intention-to-treat principle)

**Data Quality Checks:**
- Incomplete baseline assessment (>20% missing items)
- Straight-lining detection
- Duplicate entries

---

### 7. How many observations will be collected or what will determine sample size?

**Target N = 30** (15 per group)

**Determination:**
Fixed budget ($5,000) allows compensation for 30 participants plus research assistant support.

**Stopping Rule:**
- Recruitment stops when 30 participants complete baseline assessment and are randomized

---

### 8. Anything else you would like to pre-register?

**Secondary Exploratory Analyses:**

1. **Meditation Experience as Moderator**
2. **Gender Differences** in intervention response
3. **Level-Specific Adherence** patterns
4. **Trajectory Analysis** of individual change
5. **Safety Monitoring** metrics

**Variables Collected for Exploratory Purposes:**
- Demographics
- Previous therapy experience
- Open-ended feedback

**Deviations from Plan:**
Any deviations will be clearly labeled as "post-hoc" in publications.

**Data Sharing:**
All deidentified data and materials will be made publicly available on GitHub and Zenodo.

---

**Declaration:**
This pre-registration represents our analysis plan before any data collection begins. We commit to reporting results transparently, including null or unexpected findings.

**Submitted by:** Rite of Renaissance  
**Date:** October 2025  
**AsPredicted ID:** #252740

