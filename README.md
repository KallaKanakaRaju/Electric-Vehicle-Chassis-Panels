# Lightweighting Framework for Electric Vehicle (EV) Chassis Materials

A reproducible, data-driven framework for **lightweight EV chassis material selection**. This project integrates curated mechanical property data, physics-informed descriptors, and machine learning to identify low-mass, structurally feasible materials for electric vehicle design.

---

Lightweighting of electric vehicle (EV) chassis panels is essential for improving energy efficiency, range, and sustainability. This repository presents a **reproducible materials informatics pipeline** for preliminary screening and optimization of candidate materials using curated mechanical property data.

The framework demonstrates how surrogate modeling and data-driven design can accelerate materials selection while maintaining mechanical reliability.

---
The dataset comprises **1,552 records**, each containing the following mechanical properties:

- Ultimate strength (Sₙ)  
- Yield strength (Sᵧ)  
- Young’s modulus (E)  
- Shear modulus (G)  
- Density (ρ)  
- Poisson’s ratio (μ)

### 🔬 Preprocessing
- Missing value imputation  
- Outlier filtering  
- Categorical simplification  
- Feature scaling and normalization  

Two **physics-informed descriptors** were engineered:
- Specific strength = Sₙ / ρ  
- Specific modulus = E / ρ  

These enable fair, cross-material comparisons for lightweight design.

---
- **Exploratory Data Analysis (EDA)** to verify data consistency  
- **Random Forest regression baseline** for strength prediction  
  - R² = 0.48  
  - RMSE = 225.8 MPa  
  - MAE = 156.7 MPa  
- Framework provides groundwork for:
  - Constrained **Bayesian Optimization**
  - Multi-objective **material–thickness optimization**

---

Nawale, Purushottam & Kanade, Akshay & Nannaware, Bhalchandra & Sagalgile, Abhijeet & Chougule, Nagesh & Patange, Abhishek. (2023). Design automation and CAD customization of an EV chassis. Journal of Physics: Conference Series. 2601. 012014. 10.1088/1742-6596/2601/1/012014.
https://www.kaggle.com/datasets/purushottamnawale/materials
