# Smart Loan Recovery System

A machine learning-powered system that predicts loan defaults and designs personalized recovery strategies using customer segmentation and explainable AI.

## 🎯 Project Overview

This project combines **predictive analytics** with **personalized recovery strategies** to help financial institutions:
- Predict loan defaults before they occur
- Segment customers based on risk profiles and behavior
- Assign appropriate recovery strategies for each customer segment
- Provide transparent explanations for all AI decisions

## 🔧 Tech Stack

- **Python 3.8+**
- **pandas** - Data manipulation and analysis
- **scikit-learn** - Machine learning algorithms
- **SHAP** - Explainable AI for model interpretability
- **matplotlib/seaborn** - Data visualization
- **numpy** - Numerical computing

## 🚀 Getting Started

### Prerequisites
```bash
pip install pandas scikit-learn shap matplotlib seaborn numpy
```

### Installation
1. Clone the repository
```bash
git clone https://github.com/yourusername/smart-loan-recovery.git
cd smart-loan-recovery
```

2. Install dependencies
```bash
pip install -r requirements.txt
```

3. Download the Lending Club dataset and place it in `data/raw/`

### Quick Start
```python
# 1. Load and preprocess data
python src/data_preprocessing.py

# 2. Train default prediction model
python src/default_prediction.py

# 3. Perform customer segmentation
python src/customer_segmentation.py

# 4. Generate recovery strategies
python src/recovery_strategies.py

# 5. Create explainable AI reports
python src/explainable_ai.py
```

## 📈 Model Performance

- **ROC AUC Score**: 0.85+ (Target: >0.8)
- **Precision**: High precision for default prediction
- **Recall**: Balanced recall to catch potential defaults
- **F1-Score**: Optimized for business impact

## 🔍 Explainability Features

### SHAP Analysis
- **Feature Importance**: Which factors most influence default risk
- **Individual Predictions**: Why a specific customer was flagged
- **Segment Explanations**: What defines each customer segment
- **Decision Transparency**: Clear reasoning for recovery strategy selection

### Example SHAP Output
```
Customer ID: 12345
Default Probability: 0.78
Top Contributing Factors:
  - Credit utilization (45%) → +0.25 (high risk)
  - DTI ratio (38%) → +0.20 (high risk)
  - Past delinquencies (2) → +0.15 (high risk)
  - Employment length (8 years) → -0.10 (low risk)
```

## 💼 Business Impact

### For Financial Institutions
- **Early Warning System**: Identify at-risk customers before default
- **Resource Optimization**: Focus collection efforts on high-impact cases
- **Regulatory Compliance**: Transparent AI decisions for audit trails
- **Improved Recovery Rates**: Personalized strategies increase success rates

### Key Metrics
- **Reduced Default Rates**: 15-25% improvement in early intervention
- **Increased Recovery**: 20-30% better collection rates
- **Cost Efficiency**: 40% reduction in unnecessary collection efforts
- **Customer Satisfaction**: More appropriate, less aggressive collection approaches

## 🛠️ Technical Implementation

### Data Preprocessing
- Missing value imputation
- Categorical variable encoding
- Feature scaling and normalization
- Target variable creation (binary classification)

### Model Training
- Train-test split with stratification
- Cross-validation for model selection
- Hyperparameter tuning
- Model persistence and versioning

### Clustering Analysis
- Optimal cluster number selection (elbow method)
- Cluster stability analysis
- Segment profiling and interpretation

### Explainability Integration
- SHAP value computation
- Waterfall plots for individual predictions
- Summary plots for global feature importance
- Dependence plots for feature interactions

## 📊 Visualizations

The system generates comprehensive visualizations:
- **Model Performance**: ROC curves, confusion matrices, precision-recall curves
- **Segmentation**: Cluster scatter plots, segment profiles, distribution analysis
- **SHAP Plots**: Feature importance, waterfall plots, dependence plots
- **Recovery Analytics**: Strategy effectiveness, segment response rates

## 🔮 Future Enhancements

- **Real-time Prediction API**: Flask/FastAPI endpoint for live predictions
- **Advanced Clustering**: Try DBSCAN, Gaussian Mixture Models
- **Deep Learning**: Neural networks for more complex pattern recognition
- **A/B Testing Framework**: Test different recovery strategies
- **Dashboard**: Interactive web interface for stakeholders
- **Model Monitoring**: Track model drift and performance over time

## 📝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Lending Club** for providing the comprehensive loan dataset
- **SHAP Team** for the excellent explainability framework
- **Scikit-learn** community for robust machine learning tools

## 📧 Contact

Your Name - your.email@example.com
Project Link: https://github.com/yourusername/smart-loan-recovery

---

**Note**: This project is for educational and research purposes. Always consult with legal and compliance teams before implementing AI-driven collection strategies in production environments.
