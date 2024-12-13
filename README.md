# Hybrid Feature Analysis for COVID-19 Mortality Prediction

A hybrid approach to COVID-19 mortality prediction combining Random Forest and BlueBERT models. Analyzes both clinical metrics and medical text from 10,000 patient records, achieving 94.4% accuracy.

## Project Overview
### What Makes This Project Unique

- Dual Analysis Approach: Combines traditional machine learning (Random Forest) for clinical metrics with healthcare-specific natural language processing (BlueBERT) for medical text
- Comprehensive Data Integration: Analyzes both structured data (vital signs, demographics) and unstructured medical text in a single predictive model
- High Accuracy: 94.4% prediction accuracy through combined analysis methods

### Key Findings
Our analysis identified three critical mortality risk factors:

- Patient age (18.7% importance)
- Viral sepsis (12.0% importance)
- Acute respiratory distress (7.0% importance)

### Technical Implementation

- Built using Python ecosystem (Pandas, Scikit-learn)
- Random Forest for clinical metrics analysis
- HuggingFace Transformers for BlueBERT implementation
- Plotly for data visualization
- Feature importance analysis across both structured and unstructured data

### Dataset
Analysis based on Synthea's COVID-19 dataset including:

- Patient demographics and vital signs
- Medical conditions and diagnoses
- Medications and treatments
- Clinical procedures
- Comprehensive medical notes

## Project Structure

├── README.md
└── src
    ├── data
    │   └── final_df.csv          # Preprocessed dataset
    ├── documents
    │   ├── COVER_PAGE.pdf
    │   └── Hybrid Feature Analysis for COVID-19 Mortality Prediction.[docx/pdf]
    ├── notebooks
    │   ├── COVID_Project.ipynb   # Data preprocessing notebook
    │   ├── COVID_NN.ipynb        # Numerical analysis notebook
    │   └── Covid_LLM.ipynb       # Text-based analysis notebook
    └── presentation
        ├── HYBRID FEATURE ANALYSIS FOR COVID-19 MORTALITY PREDICTION.[pptx/pdf]
        └── hybrid_feature_analysis_final_project.mp4


## Getting Started

### Prerequisites
- Python 3.x
- Jupyter Notebook
- Required Python packages (listed in each notebook)

### Data Setup
1. Download the COVID-19 dataset from [Synthea](https://synthea.mitre.org/downloads)
2. Place the downloaded CSV files in your working directory
3. Run `COVID_Project.ipynb` to preprocess the data and generate `final_df.csv`

### Running the Analysis
1. **Data Preprocessing**: Run `COVID_Project.ipynb` to join and preprocess all data tables
2. **Numerical Analysis**: Use `COVID_NN.ipynb` for Random Forest classification
3. **Text Analysis**: Use `Covid_LLM.ipynb` for BlueBERT text processing

## Project Components

- `COVID_Project.ipynb`: Initial data preprocessing and table joining
- `COVID_NN.ipynb`: Numerical-based analysis using Random Forest
- `Covid_LLM.ipynb`: Text-based analysis using BlueBERT
- `final_df.csv`: Preprocessed dataset ready for analysis
- Project presentation and report available in PDF/PPTX format
- Full project presentation video available in `src/presentation`

## Authors
- Mykel Boachie
- Alejandro Mignucci

The University of Texas at Austin

## License
This project is licensed under the MIT License - see the LICENSE file for details.