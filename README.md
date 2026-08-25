# Overview

Music emotion recognition aims to automatically predict the emotional response induced by a piece of music, using audio features. The Emotify dataset provides 400 one-minute excerpts across four genres (classical, rock, pop, electronic), each annotated by listeners using the GEMS-9 scale (Geneva Emotional Music Scale, 9-category version): amazement, solemnity, tenderness, nostalgia, calmness, power, joyful activation, tension, and sadness.

Prior work on Emotify has focused almost exclusively on classical machine learning methods — SVM, KNN, MLP, and Naive Bayes — applied to handcrafted audio features. This project fills a gap in that literature by evaluating tree-based ensemble methods, which have seen little to no application on this dataset despite being standard baselines in most other MER benchmarks.

# Objectives
- Extract audio features (e.g., MFCCs, chroma, spectral contrast, tempo) from the Emotify excerpts
- Train and tune Random Forest and Gradient Boosted Trees (e.g., XGBoost/LightGBM) classifiers on the GEMS-9 emotion labels
- Evaluate performance using accuracy, ROC AUC, and per-class metrics, given the dataset's multi-label and class-imbalance characteristics
- Compare results against previously published SVM and KNN baselines on the same dataset

# Dataset
Source: Emotify dataset (Aljanaki, Wiering, Veltkamp)
Size: 400 tracks (100 per genre: classical, rock, pop, electronic), 8,407 total annotations
Labels: GEMS-9 emotion categories, multi-label (up to 3 emotions per listener per track)

