# Placement Predictor

Predict whether a candidate receives a **Yes / No** final decision using academic, skill and extracurricular features — built with pandas, seaborn for EDA and XGBoost for classification. This repository includes a reproducible pipeline: EDA (correlation heatmap) → feature selection → XGBClassifier training → evaluation → model prediction.

## Project overview
This project predicts a binary hiring/selection decision (`Target`: `Yes`/`No`) from features such as CGPA, Internships, Projects, Workshops/Certifications, AptitudeTestScore, SoftSkillsRating, SSC_Marks, and HSC_Marks. The recommended workflow:
1. Exploratory analysis with a correlation heatmap.  
2. Decide features to keep/drop using simple correlation thresholds.  
3. Train and evaluate an XGBoost classifier.  
4. Predict if student gets placed or not

---

## Dataset & Features
CSV  columns:
- `CGPA` (float)  
- `Internships` (int) — count or months  
- `Projects` (int) — count of projects  
- `Workshops_Certifications` (int) — count  
- `AptitudeTestScore` (float)  
- `SoftSkillsRating` (float / integer)
- `ExtraCurricularActivites`(`Yes` / `No`)
- `PlacementTraining`(`Yes` / `No`) 
- `SSC_Marks` (float / percentage)  
- `HSC_Marks` (float / percentage)  
- `PlacementStatus` (`Yes` / `No`) — **target column**




