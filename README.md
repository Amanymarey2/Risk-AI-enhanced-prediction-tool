# Risk AI enhanced prediction tool


Portfolio project for **HTH 111: Project Management in the Health Sector** (McMaster University Health Informatics Diploma).  
Demonstrates how data analysis and AI can strengthen traditional project risk management in a healthcare context.

## Project Goal

This project extends the HTH 111 final assignment by transforming a standard risk registry into an **AI-enhanced, data-driven tool** for the proposed **ReadmitPredict** system — a cloud-based predictive analytics solution to reduce preventable 30-day hospital readmissions.

It showcases:

- Structured risk collection (Google Forms)
- Synthetic historical data generation
- Machine learning for risk escalation prediction
- Generative AI for automatic mitigation suggestions
- Interactive visualization dashboard (Plotly Dash) 

The main message:  
**Modern data & AI techniques can significantly improve project management tasks** — especially in high-stakes health sector initiatives.

## Project Summary (from Executive Summary)

**ReadmitPredict** is a cloud-based tool that enhances the LACE index with machine learning to provide real-time 30-day readmission risk scores via an EMR-integrated dashboard (green <20%, yellow 20–50%, red >50%).  

**Target:** >30% reduction in preventable readmissions within 2 years post-pilot (Cardiology & Internal Medicine).  
**Triple constraints:**

| Constraint | Target          | Assurance                                      |
|------------|-----------------|------------------------------------------------|
| Schedule   | 10–12 months    | Phased pilot with clear milestones             |
| Budget     | ~$550,000       | Cloud-based + existing EMR integration         |
| Scope      | Two departments | Excludes full rollout & new hardware           |

## Repository Structure

├── data/
│   ├── historical_healthtech_project_risks.csv      # Synthetic training data
│   ├── Responses.xlsx                               # Raw Google Form responses
│   └── Responses_with_AI_Mitigations.xlsx  # Enriched with AI predictions & mitigations
│   └── Final_ReadmitPredict_Risk_Predictions.xlsx  # Model predictions
├── risk_registry_ReadmitPredict.ipynb              #Jupyter notebook
├── models/
│   └── risk_predictor_model.pkl                    # Trained Random Forest model
└── README.md


## Key Features & Demonstrated Skills

1. **Risk Collection**  
   - Anonymous Google Form: https://forms.gle/ZSdRNrdyVaJMbfLF9  
   - Grok AI-assisted creation of 20 realistic sample risks

2. **Historical Data Simulation**  
   - 500 synthetic health tech projects with realistic correlations

3. **ML Risk Escalation Prediction**  
   - Random Forest Classifier  
   - Threshold tuned to 0.65 for conservative, healthcare-appropriate risk flagging

4. **Generative AI Mitigation Suggestions**  
   - OpenAI GPT-4o-mini via ChatGPT subscription  
   - Context-aware, budget/timeline-aware suggestions

5. **Interactive Dashboard**  
   - Plotly Dash web application  
   - Risk heat map, word cloud of AI mitigations, top words bar chart, KPIs, filtered table

Dashboard can be accessed from: https://c97adaa2-b827-4a32-ac7d-a7faec385ac2.plotly.app/

## Setup & Usage

### Prerequisites

- Python 3.8+
- pip install -r requirements.txt


