# AI-Driven Development of High-Entropy Prussian Blue Cathodes with Exceptional Electrochemical Performance

This repository contains the code, datasets, models and checkpoints accompanying the paper:

**"AI-Driven Development of High-Entropy Prussian Blue Cathodes with Exceptional Electrochemical Performance"**

We integrate high-throughput density functional theory (DFT) calculations, machine learning (ML) models, and experimental validation to design and optimize high-entropy Prussian blue analogues (HE-PBAs) for potassium-ion battery (KIB) cathodes.

## Project Structure
```
PBA_opt/
├─ DFT&MD_scripts
│  ├─ ChangeFourMetals.py
│  ├─ DFT_POSCAR.zip          # DFT-optimized local structure in POSCAR format
│  ├─ GetAvgProperty.py       # Retrieve physicochemical properties from MD simulation structures
│  ├─ GetMetalNumTatio.py     # Extract the composition ratio from MD simulation structures
│  └─ properties.csv
├─ ML
│  ├─ ExpData.csv             # Experimental dataset
│  ├─ GenerateComposition.py  # Enumerate all elemental compositions across the space at 1 % resolution
│  ├─ Model1.py               # ML model that predicts theoretical properties from component ratios
│  ├─ Model1_cpt.h5           # Model1 checkpoint
│  ├─ Model2.py               # ML model to predict experimental property from theoretical properties
│  ├─ Model2_cpt.joblib       # Model2 checkpoint
│  ├─ Prediction_sorted.xlsx  # Full-space experimental-property prediction, ranked from highest to lowest
│  └─ TheorData.csv           # Theoretical dataset from MD simulations
├─ README.md
```
