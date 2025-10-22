# 📊 Demographics Questionnaire & Codebook
## Safe Aperture Micro-Pilot Study

**OSF Project:** [To be added upon registration]  
**GitHub Repository:** https://github.com/riteofrenaissance/safe-aperture-study  
**Pre-registration:** AsPredicted #252740  
**Study Period:** December 2025 - February 2026  
**Document Version:** 1.0  
**Last Updated:** October 22, 2025

---

## 📋 Table of Contents

1. [Purpose](#purpose)
2. [Data Collection Timeline](#data-collection-timeline)
3. [Questionnaire Items](#questionnaire-items)
4. [Variable Codebook](#variable-codebook)
5. [Data Management](#data-management)
6. [Analysis Plan](#analysis-plan)
7. [Ethical Considerations](#ethical-considerations)

---

## 🎯 Purpose

This document serves three functions:

1. **Participant-Facing Questionnaire:** Items as presented to participants during screening/baseline
2. **Data Codebook:** Variable names, coding schemes, and allowed values
3. **Analysis Plan:** How demographic data will be reported and analyzed

All demographic data is collected at **baseline only** (T0) and used for:
- Sample description (Table 1 in publications)
- Checking randomization balance between groups
- Exploratory moderator analyses (age, education, baseline anxiety)

---

## ⏰ Data Collection Timeline

| Assessment Point | Demographics | Notes |
|-----------------|--------------|-------|
| **Screening** | ✅ Collected | Before randomization |
| **Baseline (T0)** | ✅ Confirmed | Used for group assignment |
| **Post-intervention (T1)** | ❌ Not collected | — |
| **Follow-up (T2)** | ❌ Not collected | — |

**Rationale:** Demographics are stable characteristics; repeated collection is unnecessary and increases participant burden.

---

## 📝 Questionnaire Items

### Section 1: Basic Information

**Instructions to Participants:**
> The following questions help us understand who participates in our study. All responses are confidential and will be reported in aggregate form only (e.g., "average age: 28 years"). You may skip any question you're uncomfortable answering.

---

#### Q1: Age
**Question:**  
*What is your age?*

**Response Format:**
- Open text field (numeric only)
- Range validation: 18-99 years

**Variable:** `age`

---

#### Q2: Gender
**Question:**  
*What is your gender?*

**Response Options:**
- [ ] Man
- [ ] Woman
- [ ] Non-binary
- [ ] Prefer to self-describe: [text field]
- [ ] Prefer not to answer

**Variable:** `gender`

---

#### Q3: Country of Residence
**Question:**  
*In which country do you currently live?*

**Response Format:**
- Dropdown menu (ISO country codes)
- Most common: USA, UK, Canada, Australia, Other

**Variable:** `country`

---

#### Q4: Primary Language
**Question:**  
*What is your primary language (the language you're most comfortable using)?*

**Response Options:**
- [ ] English
- [ ] Spanish
- [ ] French
- [ ] Arabic
- [ ] Other: [text field]

**Variable:** `language`

**Note:** Study materials are in English; this assesses language comfort for subgroup analyses.

---

### Section 2: Education & Employment

#### Q5: Education Level
**Question:**  
*What is the highest level of education you have completed?*

**Response Options:**
- [ ] Less than high school
- [ ] High school diploma or equivalent (GED)
- [ ] Some college/university (no degree)
- [ ] Associate degree (2-year)
- [ ] Bachelor's degree (4-year)
- [ ] Master's degree
- [ ] Doctoral degree (PhD, MD, JD, etc.)
- [ ] Prefer not to answer

**Variable:** `education`

---

#### Q6: Current Employment Status
**Question:**  
*What is your current employment status?*

**Response Options:**
- [ ] Employed full-time (35+ hours/week)
- [ ] Employed part-time (<35 hours/week)
- [ ] Self-employed
- [ ] Unemployed (seeking work)
- [ ] Unemployed (not seeking work)
- [ ] Student
- [ ] Retired
- [ ] Unable to work
- [ ] Prefer not to answer

**Variable:** `employment`

---

#### Q7: Student Status
**Question:**  
*Are you currently enrolled as a student?*

**Response Options:**
- [ ] No
- [ ] Yes, part-time
- [ ] Yes, full-time

**Variable:** `student_status`

**Note:** Included separately from employment because students may also work.

---

### Section 3: Mental Health History

**Instructions:**
> The next questions ask about your mental health history. This information helps us understand our sample and ensure participant safety. All responses are confidential.

---

#### Q8: Previous Therapy/Counseling
**Question:**  
*Have you ever received therapy or counseling for mental health concerns?*

**Response Options:**
- [ ] No
- [ ] Yes, in the past (not currently)
- [ ] Yes, currently
- [ ] Prefer not to answer

**Variable:** `therapy_history`

---

#### Q9: Current Psychiatric Medication
**Question:**  
*Are you currently taking any psychiatric medications (e.g., for anxiety, depression, ADHD)?*

**Response Options:**
- [ ] No
- [ ] Yes
- [ ] Prefer not to answer

**Variable:** `psych_meds`

**Note:** We do NOT ask which medications to minimize identifiability.

---

#### Q10: Previous Diagnosis
**Question:**  
*Have you ever been diagnosed with any of the following by a healthcare professional? (Check all that apply)*

**Response Options:**
- [ ] Generalized Anxiety Disorder
- [ ] Social Anxiety Disorder
- [ ] Panic Disorder
- [ ] Major Depressive Disorder
- [ ] Obsessive-Compulsive Disorder
- [ ] PTSD
- [ ] Other anxiety/mood disorder: [text field]
- [ ] None of the above
- [ ] Prefer not to answer

**Variable:** `diagnosis_history` (multiple checkboxes → separate binary variables)

---

### Section 4: Intervention-Specific Questions

#### Q11: Previous Experience with Ambiguity Training
**Question:**  
*Have you ever participated in any training or therapy specifically focused on increasing comfort with uncertainty or ambiguity?*

**Response Options:**
- [ ] No
- [ ] Yes
- [ ] Unsure

**Variable:** `previous_ambiguity_training`

---

#### Q12: Meditation/Mindfulness Practice
**Question:**  
*Do you currently practice meditation or mindfulness?*

**Response Options:**
- [ ] No
- [ ] Yes, occasionally (less than weekly)
- [ ] Yes, regularly (weekly or more)

**Variable:** `meditation_practice`

**Rationale:** Mindfulness may affect baseline ambiguity tolerance; we want to check balance across groups.

---

#### Q13: Technology Comfort
**Question:**  
*How comfortable are you using online platforms and websites?*

**Response Options:**
- [ ] Not at all comfortable
- [ ] Slightly comfortable
- [ ] Moderately comfortable
- [ ] Very comfortable
- [ ] Extremely comfortable

**Variable:** `tech_comfort`

**Rationale:** Our intervention is web-based; low tech comfort may predict dropout.

---

### Section 5: Recruitment Source

#### Q14: How Did You Hear About This Study?
**Question:**  
*How did you learn about this study?*

**Response Options:**
- [ ] Social media (Reddit, Twitter, Facebook, etc.)
- [ ] University/college announcement
- [ ] Friend or colleague
- [ ] Research participation platform (Prolific, MTurk, etc.)
- [ ] Other: [text field]

**Variable:** `recruitment_source`

---

## 📊 Variable Codebook

### Complete Variable List

| Variable Name | Type | Coding | Range/Values | Missing Code |
|--------------|------|--------|--------------|--------------|
| `participant_id` | String | P001-P030 | — | — |
| `group` | Categorical | 0 = Control, 1 = Intervention | 0, 1 | — |
| `age` | Numeric | Years | 18-99 | 999 |
| `gender` | Categorical | 1 = Man, 2 = Woman, 3 = Non-binary, 4 = Self-describe, 5 = Prefer not to answer | 1-5 | 999 |
| `gender_text` | String | Free text if gender = 4 | — | NA |
| `country` | Categorical | ISO 3166-1 alpha-2 codes | US, GB, CA, AU, etc. | 999 |
| `language` | Categorical | 1 = English, 2 = Spanish, 3 = French, 4 = Arabic, 5 = Other | 1-5 | 999 |
| `language_other` | String | Free text if language = 5 | — | NA |
| `education` | Ordinal | 1 = <HS, 2 = HS, 3 = Some college, 4 = Associate, 5 = Bachelor, 6 = Master, 7 = Doctoral, 8 = Prefer not to answer | 1-8 | 999 |
| `employment` | Categorical | 1 = FT, 2 = PT, 3 = Self, 4 = Unemployed-seeking, 5 = Unemployed-not, 6 = Student, 7 = Retired, 8 = Unable, 9 = Prefer not to answer | 1-9 | 999 |
| `student_status` | Categorical | 0 = No, 1 = Part-time, 2 = Full-time | 0-2 | 999 |
| `therapy_history` | Categorical | 0 = No, 1 = Past, 2 = Current, 3 = Prefer not to answer | 0-3 | 999 |
| `psych_meds` | Categorical | 0 = No, 1 = Yes, 2 = Prefer not to answer | 0-2 | 999 |
| `dx_gad` | Binary | 0 = No, 1 = Yes | 0, 1 | 999 |
| `dx_social_anxiety` | Binary | 0 = No, 1 = Yes | 0, 1 | 999 |
| `dx_panic` | Binary | 0 = No, 1 = Yes | 0, 1 | 999 |
| `dx_depression` | Binary | 0 = No, 1 = Yes | 0, 1 | 999 |
| `dx_ocd` | Binary | 0 = No, 1 = Yes | 0, 1 | 999 |
| `dx_ptsd` | Binary | 0 = No, 1 = Yes | 0, 1 | 999 |
| `dx_other` | String | Free text | — | NA |
| `previous_ambiguity_training` | Categorical | 0 = No, 1 = Yes, 2 = Unsure | 0-2 | 999 |
| `meditation_practice` | Ordinal | 0 = No, 1 = Occasionally, 2 = Regularly | 0-2 | 999 |
| `tech_comfort` | Ordinal | 1 = Not at all, 2 = Slightly, 3 = Moderately, 4 = Very, 5 = Extremely | 1-5 | 999 |
| `recruitment_source` | Categorical | 1 = Social media, 2 = University, 3 = Friend, 4 = Platform, 5 = Other | 1-5 | 999 |
| `recruitment_other` | String | Free text if recruitment = 5 | — | NA |

---

## 💾 Data Management

### Data Storage
- **Raw data:** Stored on secure REDCap server (HIPAA compliant)
- **De-identified data:** GitHub repository (private until study completion)
- **OSF archive:** De-identified data + codebook (public after publication)

### Data Quality Checks
```r
# Age validation
if (age < 18 | age > 99) → flag for review

# Gender consistency
if (gender == 4 & is.na(gender_text)) → prompt participant

# Missing data monitoring
if (sum(is.na(demographics)) > 3) → flag participant record
```

### De-identification Protocol
1. Remove all free-text fields before public sharing
2. Recode `participant_id` to random IDs
3. Bin age into categories: 18-24, 25-34, 35-44, 45+
4. Replace country with region: North America, Europe, Asia, Other

---

## 📈 Analysis Plan

### 1. Sample Description (Table 1)

**Reported for:**
- Full sample (N=30)
- Intervention group (n=15)
- Control group (n=15)

**Variables:**
```
Age: M (SD), Range
Gender: n (%)
Education: n (%) per category
Employment: n (%) per category
Therapy history: n (%) Current vs Past vs None
Psychiatric medication: n (%)
Previous diagnosis (any): n (%)
Baseline anxiety (GAD-7): M (SD)
```

**Format:**
```markdown
| Variable | Total (N=30) | Intervention (n=15) | Control (n=15) | p-value* |
|----------|--------------|---------------------|----------------|----------|
| Age, M (SD) | — | — | — | — |
| Gender, n (%) | — | — | — | — |
| ... | — | — | — | — |

*p-values from chi-square tests (categorical) or t-tests (continuous)
```

---

### 2. Randomization Balance Checks

**Statistical Tests:**
- Continuous variables (age, baseline GAD-7): Independent t-tests
- Categorical variables (gender, education, etc.): Chi-square tests or Fisher's exact test
- **Significance threshold:** p < 0.05 (will be reported as potential baseline imbalance, not as exclusion criteria)

**Expected Result:**
No significant differences between groups on demographic variables (confirms successful randomization).

---

### 3. Exploratory Moderator Analyses

**Research Questions:**
- Does intervention effect vary by age? (median split or continuous)
- Does baseline anxiety (GAD-7) moderate treatment response?
- Does previous therapy history predict adherence?

**Statistical Approach:**
```r
# Example: Age as moderator
lm(TAS_change ~ group * age_centered + baseline_TAS)

# Example: Baseline anxiety as moderator
lm(TAS_change ~ group * GAD7_baseline + baseline_TAS)
```

**Reporting:**
All moderator analyses are **exploratory** and will be clearly labeled as such. No corrections for multiple comparisons (but effect sizes and CIs will be reported).

---

### 4. Attrition Analysis

**Research Question:**
Do demographic characteristics predict dropout?

**Variables Examined:**
- Age (younger → higher dropout?)
- Tech comfort (lower → higher dropout?)
- Baseline anxiety (higher → higher dropout?)
- Student status (busier → higher dropout?)

**Statistical Approach:**
Logistic regression:
```r
glm(completed ~ age + tech_comfort + GAD7_baseline + student_status, 
    family = binomial)
```

---

## 🔒 Ethical Considerations

### Privacy Protection
1. **No identifiable information:** Names, emails, IP addresses stored separately from research data
2. **Aggregate reporting:** Cells with n < 3 will be suppressed in tables
3. **De-identification:** All public data will be de-identified per protocol above

### Informed Consent
Participants are informed:
> "You will be asked to provide demographic information (age, gender, education, etc.) and answer questions about your mental health history. This information helps us describe our sample and check that our random assignment worked properly. All responses are optional, and your data will be reported in aggregate form only."

### Sensitive Data
- Mental health history questions include "Prefer not to answer" option
- No diagnostic confirmation required (self-report only)
- Free-text responses reviewed for identifiable information before data sharing

---

## 📎 Appendices

### Appendix A: Inclusion/Exclusion Criteria

Demographics are used to verify eligibility:

**Inclusion Criteria:**
- ✅ Age ≥ 18 years (`age >= 18`)
- ✅ English proficiency (self-reported; `language = 1` or comfortable with English)
- ✅ Internet access (implied by survey completion)
- ✅ GAD-7 < 15 (measured separately, not in demographics)

**Exclusion Criteria:**
- ❌ Age < 18
- ❌ Severe anxiety (GAD-7 ≥ 15)
- ❌ Previous participation in ambiguity tolerance training (`previous_ambiguity_training = 1` → exploratory analysis only, not exclusion)

---

### Appendix B: Data Dictionary File

**Filename:** `demographics_data_dictionary.csv`

Columns:
- `variable_name`
- `variable_label`
- `type` (numeric, categorical, string)
- `values` (coding scheme)
- `missing_code`
- `notes`

Available in repository: `/data/dictionaries/`

---

### Appendix C: Sample Demographics Form (REDCap)

**Instrument Name:** Demographics Questionnaire  
**Event:** Baseline (T0)  
**Estimated Completion Time:** 5 minutes

Available as: `/materials/demographics_form_redcap.xml`

---

## 📞 Contact

**Questions about this document:**  
Email: riteofrenaissance@proton.me

**Data access requests:**  
See OSF project (available after study completion)

---

## ✅ Document Checklist

Before uploading to OSF:

```markdown
□ Questionnaire items finalized
□ Codebook reviewed for accuracy
□ Missing data codes specified
□ Analysis plan matches pre-registration
□ De-identification protocol documented
□ Consent language reviewed
□ Variable names match data files
□ Ready for OSF upload
```

---

## 📝 Version History

| Version | Date | Changes | Author |
|---------|------|---------|--------|
| 1.0 | 2025-10-22 | Initial document for pre-registration | Rite of Renaissance |

---

## 📄 License

This document is part of the Safe Aperture Micro-Pilot Study and is licensed under [CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/).

**Citation:**
```
Rite of Renaissance. (2025). Safe Aperture Micro-Pilot Study: 
Demographics Questionnaire & Codebook (Version 1.0). 
Open Science Framework. https://osf.io/[project_id]
```

---

**Document Status:** ✅ Ready for OSF Upload  
**Next Update:** After data collection begins (any questionnaire modifications will be logged)