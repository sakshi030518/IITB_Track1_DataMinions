[README.md](https://github.com/user-attachments/files/22545572/README.1.md)
# Effect of Feedback on Cognitive & Affective Measures
**Group:** Data Minions  

---

## A. Problem Statement  
The aim of this project is to analyze the **effect of feedback** on both **cognitive** (accuracy, response time) and **affective** (EEG engagement, GSR arousal) measures.  
We studied whether students perform and engage differently under **Feedback** vs **No-Feedback** conditions.  

---

## B. Dataset Description  
We used the **Multisensor Dataset of South Asian Postgraduate Students working on Mental Rotation Tasks**.  
The dataset consists of:  
- **PSY.csv** → Accuracy, Response Time, Difficulty, Feedback condition  
- **EEG.csv** → Brain activity data (Theta, Alpha, Beta, Delta bands)  
- **GSR.csv** → Galvanic skin response (Arousal/Stress)  
- **Survey.csv** → Demographic and background information  

---

## C. Methodology (Proposed Model / Framework)  
Our analysis followed this **model pipeline**:  
1. **Preprocessing:** Cleaning PSY, EEG, and GSR data, handling missing values  
2. **Merging:** Creating a trial-level dataset linking PSY, EEG, and GSR  
3. **Feature Extraction:**  
   - Accuracy & Response Time (from PSY)  
   - EEG Theta/Alpha power (from EEG)  
   - GSR conductance values (from GSR)  
4. **Statistical Analysis:** Used **ANOVA** to compare Feedback vs No-Feedback  
5. **Visualization:** Plots for accuracy, RT, EEG, and GSR across conditions  

---

## D. Results  
- **Cognitive Results:**  
  - Accuracy higher with feedback  
  - Response time faster with feedback  
- **Affective Results:**  
  - EEG Theta/Alpha increased with feedback (greater engagement)  
  - GSR increased with feedback (higher arousal)  
- **ANOVA Findings:**  
  - Accuracy → Significant effect of feedback (F ≈ 7.4, p < 0.05)  
  - Response Time → Significant effect of feedback (F ≈ 6.2, p < 0.05)  
  - EEG Theta → Trend toward significance (p < 0.1)  

---

## E. Conclusion  
Feedback **positively influences** learning:  
- Improves accuracy and speed (cognitive)  
- Increases engagement and arousal (affective)  
- ANOVA confirms these effects are statistically significant  

---

## F. Project Organization  
```
project/
├── data/
│   ├── PSY.csv
│   ├── EEG.csv
│   ├── GSR.csv
│   └── Survey.csv
├── notebooks/
│   └── Project_Notebook.ipynb
├── report/
│   └── Data_Minions_Final_Report_With_All_Screenshots.docx
├── presentation/
│   └── Data_Minions_Creative_Final_Presentation.pptx
└── README.md
```

---

## G. Tools & Technologies  
- **Google Colab** – Python coding and analysis  
- **Python Libraries** – pandas, matplotlib, seaborn, statsmodels  
- **MS Word** – Report writing  
- **MS PowerPoint** – Presentation  

---

## H. How to Run  
1. Upload dataset files (`PSY.csv`, `EEG.csv`, `GSR.csv`, `Survey.csv`) to Google Drive  
2. Open `Project_Notebook.ipynb` in **Google Colab**  
   - Run preprocessing, feature extraction, ANOVA, and visualization steps  
3. Results (graphs + tables) will be saved in `/results/` folder  
4. Report (`.docx`) and Presentation (`.pptx`) contain the final analysis  

---

## I. Deliverables  
- Processed trial-level dataset  
- Graphs & Visualizations  
- Word Report with ANOVA results  
- PowerPoint Presentation with tools & framework  
- GitHub Repository for IITB submission  

---
