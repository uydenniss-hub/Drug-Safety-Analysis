# Drug Safety Analysis

This project explores a clinical trial dataset comparing **Drug** and **Placebo** groups.  
The main objective is to test whether the treatment is associated with higher adverse effects and whether participant characteristics (e.g., age) differ between groups.

---

## 📊 Project Overview
- **Dataset:** `drug_safety.csv`
- **Goal:** Evaluate drug safety by analyzing adverse effects and participant demographics.
- **Approach:** Applied statistical hypothesis tests and visualizations to examine differences between treatment and control.

---

## 🔬 Key Analyses
1. **Adverse Effects (Binary Outcome)**
   - Converted `adverse_effects` into 0/1 encoding.
   - Compared proportions of adverse effects in Drug vs Placebo groups using a **two-proportion z-test**.

2. **Number of Adverse Effects (Count Outcome)**
   - Tested independence between `num_effects` and treatment group using a **Chi-square test of independence**.

3. **Age Distribution (Continuous Outcome)**
   - Compared ages between Drug and Placebo groups using a **Welch’s t-test**.
   - Visualized age distributions with histograms.

---

## 📈 Results (Example Output)
- **Adverse effects proportion test:** *p = 0.964 → Fail to reject H₀*  
- **Chi-square test (num_effects):** *p ≈ [insert]*  
- **Welch’s t-test (age):** *p ≈ [insert]*  

Interpretation: No statistically significant differences were found in adverse effect rates or participant ages between Drug and Placebo groups.

---

## 🛠️ Tools & Libraries
- Python  
- pandas  
- statsmodels  
- scipy  
- pingouin  
- seaborn / matplotlib  
