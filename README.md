# Hybrid BERT-Based Sentiment Analysis with Knowledge Graph

## 📌 Overview
This study analyzes public sentiment toward agricultural digitalization by combining transformer-based NLP and graph-based modeling. The approach integrates BERT with multiple machine learning classifiers and extends the analysis using Knowledge Graph to capture relationships between entities in news data.

## 📊 Dataset
News articles collected from:
- BBC
- The Guardian
- The Independent
- Reuters

## ⚙️ Methodology

### 1. Sentiment Analysis (Hybrid Models)
BERT is used as a feature extractor, followed by multiple classifiers:
- BERT + SVM  
- BERT + Random Forest  
- BERT + XGBoost  

Each model is evaluated using cross-validation to compare performance across different classifiers.

### 2. Model Selection
Although multiple hybrid models are explored, BERT + Random Forest is selected as the final model due to:
- Stable and high performance
- Faster inference
- Better suitability for downstream Knowledge Graph integration :contentReference[oaicite:0]{index=0}

### 3. Knowledge Graph Construction
Sentiment outputs are integrated into a Knowledge Graph through:
- Named Entity Recognition (NER)
- Relation extraction (subject–relation–object triples)

Each relationship is enriched with sentiment probabilities from the model. :contentReference[oaicite:1]{index=1}

### 4. Graph-Based Analysis
Further analysis is performed using:
- Graph Convolutional Network (GCN)
- Community detection
- Centrality analysis

This allows identification of topic clusters and sentiment patterns across entities.

## 🚀 Contribution
- Hybrid comparison: BERT + SVM, RF, and XGBoost  
- Integration of sentiment analysis with Knowledge Graph  
- Graph-based insight extraction beyond traditional text analysis  

This approach addresses limitations of prior studies that rely solely on text-based sentiment analysis. :contentReference[oaicite:2]{index=2}

## 📈 Insights
The model enables:
- Sentiment classification of news articles
- Entity-level relationship mapping
- Topic and community detection within news discourse

## 🛠️ Tech Stack
- Python
- BERT (Transformer)
- Scikit-learn (SVM, Random Forest)
- XGBoost
- spaCy (NER & relation extraction)
- NetworkX / Graph Processing
- Graph Convolutional Network (GCN)

## 📖 Notes
This project is part of a master’s thesis focusing on hybrid NLP and graph-based sentiment analysis for understanding media narratives in agricultural digitalization.
