# Safe Aperture Micro-Pilot Study

[![Study Status](https://img.shields.io/badge/Status-Pre--registered-blue)](https://github.com/riteofrenaissance/safe-aperture-study)
[![Phase](https://img.shields.io/badge/Phase-IRB_Submission-orange)]()
[![License](https://img.shields.io/badge/License-CC--BY--4.0-green)](LICENSE)
<!-- [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.XXXXXXX.svg)](https://doi.org/10.5281/zenodo.XXXXXXX) -->
<!-- DOI badge will be added after Zenodo release -->

**A pre-registered randomized controlled pilot study testing the efficacy of Safe Aperture training for increasing ambiguity tolerance.**

---

## 📋 Study Summary

| **Element** | **Description** |
|-------------|-----------------|
| **Design** | Randomized Controlled Pilot Trial |
| **Sample** | N = 30 adults (18-65 years) |
| **Groups** | Intervention (n=15) vs. Waitlist Control (n=15) |
| **Duration** | 4 weeks active intervention + 4 weeks follow-up |
| **Primary Outcome** | Tolerance of Ambiguity Scale (TAS) |
| **Timeline** | December 2025 - February 2026 |
| **Budget** | $5,000 (self-funded) |
| **Status** | Pre-registered, IRB submission in progress |

---

## 🎯 Research Question

**Does a 4-week graduated Safe Aperture training program increase tolerance of ambiguity compared to waitlist control?**

---

## 📖 Background

### Rationale
Intolerance of uncertainty (IU) is a transdiagnostic risk factor for:
- Generalized anxiety disorder
- Depression
- Poor decision-making under ambiguity
- Avoidance behaviors

Existing interventions (CBT, mindfulness) address IU indirectly. **Safe Aperture** proposes a direct, graduated exposure approach specifically targeting ambiguity tolerance.

### Theoretical Foundation
- **Exposure therapy principles:** Repeated, graduated exposure reduces anxiety
- **Acceptance and Commitment Therapy (ACT):** Observation without interpretation
- **Mindfulness:** Present-moment awareness without judgment

### Innovation
Unlike general mindfulness training, Safe Aperture:
- ✅ Targets ambiguity specifically
- ✅ Uses structured 5-level progression
- ✅ Includes built-in safety protocols
- ✅ Balances challenge with support

---

## 🧪 Study Design

### Participants
**Inclusion:**
- Age 18-65 years
- Fluent in [study language]
- Daily internet access
- Willing to commit 10-20 min/day for 4 weeks

**Exclusion:**
- Active suicidal ideation
- History of psychotic disorder
- Severe untreated depression (PHQ-9 > 20)
- Current participation in other psychological intervention

### Randomization
- **Method:** Simple 1:1 randomization via random number generator
- **Timing:** After baseline assessment completion
- **Stratification:** None (pilot study)

### Intervention
**Experimental Group:** Safe Aperture Training (Levels 1-3 only)

| **Level** | **Duration** | **Focus** | **Time/Day** |
|-----------|--------------|-----------|--------------|
| **Level 1** | Weeks 1-2 | Everyday ambiguity | 10 min |
| **Level 2** | Week 3 | Interpersonal ambiguity | 15 min |
| **Level 3** | Week 4 | Conceptual ambiguity | 20 min |

**Delivery:** Web-based platform  
**Link:** [Safe Aperture Simulation](https://riteofrenaissance.github.io/riteofrenaissance/safe_aperture_simulation.html)

**Control Group:** Waitlist (no intervention during active period; offered training after Week 8)

---

## 📊 Measures

### Primary Outcome
**Tolerance of Ambiguity Scale (TAS)** - McLain (2009)
- 13 items, 5-point Likert scale
- Higher scores = greater tolerance
- **Timepoints:** Baseline, Week 4 (post), Week 8 (follow-up)

### Secondary Outcomes
1. **Intolerance of Uncertainty Scale - Short Form (IUS-12)**
   - Carleton et al. (2007)
   - 12 items, 5-point Likert
   - Higher = greater intolerance

2. **Generalized Anxiety Disorder Scale (GAD-7)**
   - Spitzer et al. (2006)
   - 7 items, 4-point scale
   - Range 0-21; ≥10 = moderate anxiety

### Process Measures
- **Adherence:** % of exercises completed
- **Satisfaction:** 5-item post-intervention questionnaire
- **Safety:** Adverse events (weekly monitoring)

---

## 🔬 Hypotheses (Pre-registered)

### H1 (Primary)
Intervention group will show **significantly greater increase** in TAS scores (Baseline → Week 4) compared to control.

**Analysis:** Independent samples t-test on change scores  
**Expected effect:** Cohen's d ≥ 0.5 (medium)

### H2 (Persistence)
Intervention effects will **partially persist** at Week 8 follow-up (though possibly attenuated).

### H3 (Secondary outcomes)
Improvements in TAS will be **paralleled** by:
- Decreased IUS-12 scores (lower intolerance)
- Decreased GAD-7 scores (lower anxiety)

### H4 (Exploratory - Moderators)
**Baseline anxiety** will moderate intervention effects:
- Moderate anxiety → largest gains
- High anxiety → smaller gains (ceiling effect)

---

## 📁 Repository Contents

```
safe-aperture-study/
│
├── README.md                       # This file (study overview)
├── PROTOCOL.md                     # Complete detailed protocol
├── PRE-REGISTRATION.md            # Pre-registered analysis plan
├── LICENSE                         # CC-BY-4.0
│
├── measures/                       # Measurement instruments
│   ├── TAS_McLain2009.pdf         # Tolerance of Ambiguity Scale
│   ├── IUS-12_Carleton2007.pdf    # Intolerance of Uncertainty Scale
│   └── GAD-7_Spitzer2006.pdf      # Generalized Anxiety Disorder scale
│
├── materials/                      # Study materials
│   ├── consent_form.md            # Informed consent template
│   ├── recruitment_flyer.pdf      # Participant recruitment poster
│   ├── screening_form.md          # Eligibility questionnaire
│   └── debriefing_script.md       # Post-study debriefing
│
├── analysis/                       # Analysis scripts (added after data collection)
│   ├── analysis_plan.R            # Pre-registered analysis code
│   ├── power_analysis.R           # Sample size justification
│   └── data_cleaning.R            # Data preparation script
│
└── data/                           # Data files (added after collection)
    ├── README_data.md             # Data dictionary
    ├── raw_data_deidentified.csv  # Raw data (anonymized)
    └── processed_data.csv         # Analysis-ready data
```

---

## 🗓️ Timeline

| **Phase** | **Duration** | **Dates (Estimated)** | **Status** |
|-----------|--------------|------------------------|------------|
| **Protocol Development** | 2 weeks | Oct 2025 | ✅ Complete |
| **IRB Submission** | 2-3 weeks | Nov 2025 | 🔄 In Progress |
| **Recruitment** | 2 weeks | Late Nov 2025 | ⏳ Pending |
| **Baseline Assessment** | 1 week | Late Nov 2025 | ⏳ Pending |
| **Active Intervention** | 4 weeks | Dec 2025 | ⏳ Pending |
| **Follow-up Assessment** | 4 weeks | Jan 2026 | ⏳ Pending |
| **Data Analysis** | 2 weeks | Late Jan 2026 | ⏳ Pending |
| **Manuscript Writing** | 3 weeks | Feb 2026 | ⏳ Pending |
| **Preprint Publication** | - | Feb 2026 | ⏳ Pending |

---

## 👥 Research Team

| **Role** | **Name** | **Affiliation** |
|----------|----------|-----------------|
| **Principal Investigator** | [TBD - Seeking partner] | [University TBD] |
| **Project Coordinator / Funder** | Rite of Renaissance | Independent |
| **Research Assistant** | [TBD - To be hired] | [University TBD] |
| **Statistical Consultant** | [TBD] | [TBD] |

**Seeking Academic Partnership:**  
We are actively seeking a PhD-level researcher in psychology/neuroscience to serve as PI for IRB oversight and co-authorship. Minimal time commitment (~5-10 hours total). Fully funded study.

**Contact:** riteofrenaissance@gmail.com

---

## 💰 Budget

**Total:** $5,000 (self-funded by Rite of Renaissance)

| **Item** | **Cost** |
|----------|----------|
| Participant compensation (30 × $50 gift cards) | $1,500 |
| Research Assistant (part-time, 3 months) | $2,500 |
| Survey platform (Qualtrics via university) | $0 |
| Measurement instruments (all public domain) | $0 |
| IRB fees (via university) | $0 |
| Data storage (OSF/Zenodo) | $0 |
| Preprint publication | $0 |
| Contingency | $1,000 |

---

## 🔐 Ethics & Data Protection

### IRB Approval
- **Status:** Application in preparation
- **Institution:** [University name - TBD upon PI partnership]
- **Expected approval:** November 2025

### Informed Consent
- Electronic consent obtained before baseline
- Participants informed of:
  - Study purpose, procedures, timeline
  - Voluntary participation (can withdraw anytime)
  - Risks (possible temporary discomfort)
  - Benefits (improved coping skills; contribution to science)
  - Compensation ($50 for completing all assessments)
  - Confidentiality measures

### Data Protection
- **Deidentification:** All personal identifiers removed
- **Storage:** University-secured servers (password protected)
- **Access:** Research team only during active study
- **Sharing:** Deidentified data publicly shared on OSF after publication

### Safety Monitoring
- **Weekly check-ins** by RA
- **Emergency Exit** available in platform
- **Distress protocol:** Referral to campus counseling if GAD-7 ≥ 15
- **Adverse event tracking:** All reported distress documented

---

## 📊 Statistical Analysis Plan

### Primary Analysis
**Independent samples t-test:**
- DV: TAS change score (Week 4 - Baseline)
- IV: Group (Intervention vs. Control)
- α = 0.05 (two-tailed)
- Effect size: Cohen's d with 95% CI

### Secondary Analyses
1. **Repeated measures ANOVA:** Group × Time interaction (Baseline, Week 4, Week 8)
2. **Correlation:** Adherence × outcome change (intervention group only)
3. **Multiple regression:** Moderator analysis (baseline anxiety × group)

### Missing Data
- **Primary:** Complete case analysis (baseline + Week 4 data)
- **Sensitivity:** Last observation carried forward (LOCF)
- **Reporting:** Attrition rates and completer vs. dropout comparisons

### Software
- R (version 4.3+) or SPSS (version 28+)
- All scripts pre-written and publicly available

---

## 🌐 Open Science Commitment

### Pre-registration
✅ Study protocol, hypotheses, and analysis plan documented **before data collection**

### Open Materials
All study materials publicly available:
- Protocol (PROTOCOL.md)
- Pre-registration (PRE-REGISTRATION.md)
- Measures (measures/ folder)
- Consent forms (materials/ folder)

### Open Data
After publication:
- ✅ Deidentified raw data (CSV)
- ✅ Analysis scripts (R/SPSS)
- ✅ Codebook and data dictionary

### Open Access
- ✅ Preprint on PsyArXiv (regardless of results)
- ✅ Target open-access journals (e.g., PLOS ONE)
- ✅ No paywalls for materials

---

## 📚 Dissemination Plan

### Preprint
**Timeline:** Within 4 weeks of analysis completion (Feb 2026)  
**Platform:** PsyArXiv or MedRxiv  
**Commitment:** Publish regardless of outcome (positive, negative, or null)

### Peer-Reviewed Publication
**Target Journals:**
1. *Mindfulness* (if results positive)
2. *Pilot and Feasibility Studies* (methodological focus)
3. *PLOS ONE* (open-access, accepts negative results)

### Conference Presentations
- Society for Research in Psychopathology (SRP)
- Association for Behavioral and Cognitive Therapies (ABCT)

### Public Communication
- Blog post summarizing findings (lay audience)
- Social media thread (key takeaways)
- Updates to platform users

---

## 📖 How to Cite

### Citing This Protocol (Before Publication)
```
Rite of Renaissance. (2025). Safe Aperture Micro-Pilot Study: 
Pre-registered Protocol (Version v1.0). GitHub. 
https://github.com/riteofrenaissance/safe-aperture-study
```

### Citing After Zenodo DOI
```
Rite of Renaissance. (2025). Safe Aperture Micro-Pilot Study: 
Pre-registered Protocol (Version v1.0). Zenodo. 
https://doi.org/10.5281/zenodo.XXXXXXX
```

### Citing the Intervention Platform
See: [riteofrenaissance/riteofrenaissance](https://github.com/riteofrenaissance/riteofrenaissance) repository

---

## 🤝 Collaboration Opportunities

### For Researchers
**Academic PI Partnership:**
- Minimal time commitment (~5-10 hours)
- Co-authorship on publication
- Preliminary data for future grants
- No financial contribution required

**Contact:** riteofrenaissance@gmail.com

### For Students
**Research Assistant Position:**
- Part-time (10 hours/week, 3 months)
- $2,500 compensation
- Hands-on RCT experience
- Co-authorship consideration

**Requirements:**
- Graduate student in psychology/neuroscience
- Familiarity with Qualtrics/REDCap
- Detail-oriented, reliable

**To Apply:** Send CV to riteofrenaissance@gmail.com

---

## 🚧 Limitations (Acknowledged)

This is a **pilot/feasibility study** with recognized limitations:

1. **Small sample (N=30):** Underpowered for subgroup analyses
2. **No active control:** Can't separate specific vs. non-specific effects
3. **Self-selected sample:** Generalizability limited
4. **Short follow-up (8 weeks):** Long-term effects unknown
5. **Online delivery:** Adherence harder to ensure than in-person

These limitations are **acceptable for preliminary work** and will inform future larger trials.

---

## 🔗 Links

- **Study Protocol:** [PROTOCOL.md](PROTOCOL.md)
- **Pre-registration:** [PRE-REGISTRATION.md](PRE-REGISTRATION.md)
- **Intervention Platform:** [Safe Aperture Simulation](https://riteofrenaissance.github.io/riteofrenaissance/safe_aperture_simulation.html)
- **Product Repository:** [riteofrenaissance/riteofrenaissance](https://github.com/riteofrenaissance/riteofrenaissance)
- **DOI (after release):** [To be added]
- **Contact:** riteofrenaissance@gmail.com

---

## 📜 License

**Protocol & Materials:** CC-BY-4.0  
**Data (after publication):** CC-BY-4.0  

You are free to:
- Use in your own research (with citation)
- Adapt and modify
- Distribute
- Use commercially

**Attribution required.**

---

## 📞 Contact & Questions

**General Inquiries:** riteofrenaissance@gmail.com  
**PI Partnership:** riteofrenaissance@gmail.com  
**RA Application:** riteofrenaissance@gmail.com  
**Study Participation:** [Link will be added after IRB approval]

---

## 🙏 Acknowledgments

This study is made possible by:
- Self-funding from Rite of Renaissance project
- Open-source measurement instruments (McLain, Carleton, Spitzer)
- Future academic partnership (TBD)
- Open science community (OSF, Zenodo, PsyArXiv)

---

**Last Updated:** October 20, 2025  
**Protocol Version:** 1.0  
**Study Status:** Pre-registered, IRB submission in progress
