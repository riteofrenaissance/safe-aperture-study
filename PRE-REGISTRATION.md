# 📋 Pre-registration Information
## Safe Aperture Micro-Pilot Study

**Lead Investigator:** Samir Baladi  
**Affiliation:** Rite of Renaissance  
**Registration Date:** October 22, 2025  
**Status:** ✅ Complete - Registered before data collection

---

## 🔗 Registration Links

This study is pre-registered across multiple platforms to ensure maximum transparency and reproducibility:

| Platform | DOI/Link | Status | Purpose |
|----------|----------|--------|---------|
| **OSF Preregistration** | [10.17605/OSF.IO/UTQFC](https://doi.org/10.17605/OSF.IO/UTQFC) | ✅ Complete | Official pre-registration |
| **AsPredicted** | [#252740](https://aspredicted.org/blind.php?x=252740) | ✅ Complete | Alternative pre-registration |
| **Zenodo Archive** | [10.5281/zenodo.17396753](https://doi.org/10.5281/zenodo.17396753) | ✅ Complete | Protocol archive |
| **GitHub Repository** | [safe-aperture-study](https://github.com/riteofrenaissance/safe-aperture-study) | ✅ Active | Living documentation |
| **GitHub Pages** | [Live Platform](https://riteofrenaissance.github.io/safe-aperture-study/) | ✅ Active | Intervention platform |

---

## 📅 Timeline

| Event | Date | Status |
|-------|------|--------|
| Protocol Development | Sep-Oct 2025 | ✅ Complete |
| **Pre-registration (OSF)** | **Oct 22, 2025** | **✅ Complete** |
| **Pre-registration (AsPredicted)** | **Oct 2025** | **✅ Complete** |
| **Zenodo Archiving** | **Oct 2025** | **✅ Complete** |
| IRB Submission | Nov 2025 | ⏳ Pending |
| IRB Approval | Nov 2025 | ⏳ Awaiting |
| **Data Collection Begins** | **Dec 2025** | ⏳ Scheduled |
| Intervention Period | Jan 2026 (4 weeks) | ⏳ Scheduled |
| Follow-up Assessment | Feb 2026 | ⏳ Scheduled |
| Data Analysis | Mar-Apr 2026 | ⏳ Scheduled |
| Results Dissemination | May 2026 | ⏳ Scheduled |

**⚠️ IMPORTANT:** All registrations completed BEFORE data collection begins.

---

## 📊 What's Pre-registered

### **1. Study Design**
- **Type:** Randomized Controlled Trial (RCT)
- **Sample Size:** N = 30 (15 intervention, 15 control)
- **Design:** Parallel-group, 1:1 allocation
- **Duration:** 4 weeks intervention + 4 weeks follow-up
- **Blinding:** Outcome assessors blinded to group assignment

### **2. Hypotheses**

**Primary Hypothesis:**
> Participants in the Safe Aperture intervention group will show significantly greater increases in ambiguity tolerance (TAS scores) from baseline to post-intervention compared to waitlist controls (minimum detectable effect: d = 0.5).

**Secondary Hypotheses:**
1. Intervention effects will be maintained at 4-week follow-up (T2)
2. Intervention group will show reductions in intolerance of uncertainty (IUS-12)
3. Changes in ambiguity tolerance will correlate negatively with anxiety symptoms (GAD-7)

### **3. Outcome Measures**

**Primary Outcome:**
- **TAS (Tolerance of Ambiguity Scale):** 13-item scale, range 1-5
- **Timepoints:** Baseline (T0), Post-intervention (T1), Follow-up (T2)

**Secondary Outcomes:**
- **IUS-12 (Intolerance of Uncertainty Scale):** 12-item scale, range 12-60
- **GAD-7 (Generalized Anxiety Disorder Scale):** 7-item scale, range 0-21
- **Timepoints:** Same as primary + Safety check at Week 2

**Covariates:**
- Demographics (age, gender, education)
- Baseline anxiety (GAD-7)
- Therapy history
- Meditation practice

### **4. Statistical Analysis Plan**

**Primary Analysis:**
```
Linear Mixed Model (LMM):
TAS ~ Time + Group + Time×Group + Baseline_TAS + (1|participant_id)

Primary test: Time×Group interaction at T1 (post-intervention)
Effect size: Cohen's d for between-group difference
Software: R (lme4 package)
```

**Significance Level:**
- Alpha = 0.05 (two-tailed)
- No correction for multiple comparisons (secondary outcomes exploratory)

**Missing Data:**
- Intention-to-treat (ITT) analysis
- Multiple imputation (5 imputations, mice package)
- Sensitivity analysis: Per-protocol (completers only)

### **5. Sample Size Justification**

**Power Analysis:**
- Effect size: d = 0.5 (medium effect)
- Power: 80%
- Alpha: 0.05 (two-tailed)
- Required N: 26
- Recruited N: 30 (accounts for 15% attrition)

**Rationale for d = 0.5:**
- Conservative estimate for novel intervention
- Consistent with related CBT/mindfulness interventions (d = 0.30-0.70)
- Meaningful clinical effect for brief (4-week) intervention

### **6. Eligibility Criteria**

**Inclusion:**
- Age ≥ 18 years
- English proficiency (self-reported)
- Regular internet access
- GAD-7 < 15 (minimal to moderate anxiety)

**Exclusion:**
- GAD-7 ≥ 15 (severe anxiety - referred to resources)
- Currently in another psychological intervention study
- Unable to commit to 8-week study period

### **7. Randomization & Blinding**

**Randomization:**
- Computer-generated random sequence (R software)
- Simple randomization (no blocking/stratification)
- 1:1 allocation ratio
- Conducted after baseline assessment
- Allocation concealment maintained

**Blinding:**
- Participants: Not blinded (aware of group assignment)
- Interventionists: Not applicable (self-administered platform)
- Outcome assessors: Blinded (automated data collection)
- Data analysts: Blinded until primary analysis complete

### **8. Data Collection Procedures**

**Recruitment:**
- Social media (Reddit, Twitter, Facebook)
- University announcements (with IRB approval)
- Research platforms (Prolific, MTurk)
- Target: N = 30 in 4 weeks (December 2025)

**Assessment Schedule:**
- **Screening:** Online survey (Qualtrics), ~5 minutes
- **Baseline (T0):** Demographics + TAS + IUS-12 + GAD-7, ~15 minutes
- **Week 2:** Safety check (GAD-7 only, intervention group)
- **Post (T1):** Week 4, TAS + IUS-12 + GAD-7
- **Follow-up (T2):** Week 8, TAS + IUS-12 + GAD-7

**Intervention:**
- Safe Aperture web platform
- 5 progressive levels (everyday → existential ambiguity)
- Self-paced, recommended 2-3 sessions/week
- 20-30 minutes per session
- Automated email reminders

---

## 📂 Registered Materials

All measurement instruments and protocols are publicly archived:

### **On OSF (DOI: 10.17605/OSF.IO/UTQFC):**
- ✅ TAS.pdf (Tolerance of Ambiguity Scale)
- ✅ IUS-12.pdf (Intolerance of Uncertainty Scale)
- ✅ GAD-7.pdf (Generalized Anxiety Disorder Scale)
- ✅ demographics.docx (Demographics questionnaire)
- ✅ riteofrenaissance.docx (Study overview)

### **On GitHub:**
- ✅ Complete protocol (PROTOCOL.md)
- ✅ Measurement references (measures/MEASURES_REFERENCES.md)
- ✅ Demographics codebook (measures/DEMOGRAPHICS.md)
- ✅ Pre-registration checklist (PREREGISTRATION_CHECKLIST.md)
- ✅ Citation file (CITATION.cff)

### **On Zenodo (DOI: 10.5281/zenodo.17396753):**
- ✅ Complete study protocol (PDF)
- ✅ Methodology details
- ✅ Budget and timeline

---

## 🔒 Registration Integrity

### **Immutability:**
- ✅ OSF registration is timestamped and locked
- ✅ Cannot be edited after archiving
- ✅ Any deviations will be documented transparently
- ✅ Multiple platforms ensure redundancy

### **Transparency Commitment:**

**We commit to:**
1. Report all pre-registered analyses (even if non-significant)
2. Clearly distinguish confirmatory vs. exploratory analyses
3. Document any protocol deviations with justification
4. Share de-identified data and analysis code after publication
5. Report results regardless of outcome

**Deviations Policy:**
- Any changes to protocol will be noted as "Deviation from pre-registration"
- Justification will be provided
- Original pre-registered plan will remain visible
- Exploratory analyses will be clearly labeled

---

## 📖 How to Cite This Pre-registration

### **APA Format:**
```
Baladi, S. (2025). Safe Aperture Micro-Pilot Study: Pre-registered Protocol 
(OSF Registration). Open Science Framework. 
https://doi.org/10.17605/OSF.IO/UTQFC
```

### **BibTeX:**
```bibtex
@misc{baladi2025safeaperture,
  author = {Baladi, Samir},
  title = {Safe Aperture Micro-Pilot Study: Pre-registered Protocol},
  year = {2025},
  publisher = {Open Science Framework},
  doi = {10.17605/OSF.IO/UTQFC},
  url = {https://doi.org/10.17605/OSF.IO/UTQFC}
}
```

---

## 🎖️ Open Science Badges

This study qualifies for:

- ✅ **Pre-registered:** Design and analysis registered before data collection
- ✅ **Open Materials:** All instruments and protocols publicly shared
- ✅ **Pre-registered + Analysis Plan:** Comprehensive statistical plan included
- 🔄 **Open Data:** (Will be shared after publication)

---

## 📧 Contact & Access

### **Study Team:**
**Email:** riteofrenaissance@proton.me

### **Access Registration:**
- **OSF:** https://doi.org/10.17605/OSF.IO/UTQFC
- **AsPredicted:** https://aspredicted.org/blind.php?x=252740
- **Zenodo:** https://doi.org/10.5281/zenodo.17396753

### **Study Materials:**
- **GitHub:** https://github.com/riteofrenaissance/safe-aperture-study
- **Platform:** https://riteofrenaissance.github.io/safe-aperture-study/

---

## 📋 Related Documents

- [Complete Protocol](PROTOCOL.md) - Detailed methodology
- [Pre-registration Checklist](PREREGISTRATION_CHECKLIST.md) - Verification
- [Measurement References](measures/MEASURES_REFERENCES.md) - Instrument details
- [Demographics](measures/DEMOGRAPHICS.md) - Questionnaire and codebook
- [Citation File](CITATION.cff) - How to cite this study

---

## 🔄 Version History

| Version | Date | Changes |
|---------|------|---------|
| 1.0 | Oct 22, 2025 | Initial pre-registration (OSF, AsPredicted, Zenodo) |
| 1.1 | Oct 22, 2025 | Updated with all registration links and DOIs |

---

## ✅ Verification

**Registration Status:** ✅ **COMPLETE**

**Verified:**
- [x] Registered before data collection begins
- [x] All hypotheses pre-specified
- [x] Analysis plan complete and detailed
- [x] Materials publicly archived
- [x] Multiple platforms for redundancy
- [x] Timestamped and immutable

**Next Milestone:** IRB approval (November 2025)

---

**Last Updated:** October 22, 2025  
**Study Phase:** Pre-data collection  
**Registration Phase:** Complete

---

*This study is part of the Rite of Renaissance research initiative promoting ambiguity tolerance and uncertainty navigation skills.*