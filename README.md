# Employee Exit Survey Analysis

Analysis of exit survey data from two Australian public sector organisations (DETE and TAFE) to understand why employees resign and whether dissatisfaction patterns differ by length of service.

---

### **Problem Definition:**
When employees leave an organisation, exit surveys capture their reasons. But raw survey data is messy — inconsistent column names, missing values, free-text responses, and different formats across departments. This project cleans and combines survey data from two separate sources, then analyses the results to answer:

- Are employees who have worked longer more likely to leave due to dissatisfaction?
- Do resignation reasons differ between the two organisations?
- What patterns can inform retention strategies?

### **Approach:**

1. **Data cleaning —** Standardised column names across two differently structured datasets. Handled missing values, cleaned inconsistent categorical responses, and created a unified dissatisfaction indicator from multiple survey questions.
2. **Feature engineering —** Calculated service tenure from employment dates. Created tenure categories (new, experienced, established, veteran) and a binary "dissatisfied" flag combining several resignation-related columns.
3. **Analysis —** Grouped results by tenure category and organisation. Compared dissatisfaction rates across groups using aggregation and visualisation.

#### **Key Findings:**
(Actual findings from the notebook, for example:)

(Example: "Employees with 7+ years of service were significantly more likely to cite dissatisfaction as their reason for leaving.")
(Example: "DETE employees showed higher dissatisfaction rates than TAFE across all tenure categories.")

### Tools Used
 
- **Data cleaning and analysis:** Python, Pandas, NumPy
- **Visualisation:** Matplotlib, Seaborn

### How to Run
 
```bash
git clone https://github.com/kmtaiwo/employee-exit-survey-analysis.git
cd employee-exit-survey-analysis
pip install pandas numpy matplotlib seaborn jupyter
jupyter notebook
```


**Licence**
MIT
