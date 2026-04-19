🧠 MFScan — Multi-Level Fake News Detection

“Truth has four shades.”

MFScan is a deep learning-based web application that goes beyond binary classification to detect fake news at multiple levels using NLP, CNN + Bi-LSTM, and Explainable AI (LIME).

🚀 Features
🔍 Multi-Level Classification
🔴 Fake
🟠 Misleading
🟡 Partially Real
🟢 Real
🧠 Deep Learning Model
CNN + Bi-LSTM hybrid architecture
Learns both local patterns (n-grams) and contextual dependencies
📊 Explainable AI
Uses LIME / Occlusion
Highlights important words influencing predictions
⚡ Interactive Web Interface
Paste headline/article and analyze instantly
Visual probability bars and classification bands
🗂️ Fact Database Override
Known facts are directly verified without model prediction
🧪 Model Details
Architecture: CNN + Bi-LSTM
Dataset:
WELFake Dataset (~72,000 articles)
Custom dataset (Indian news, health, science)
Accuracy: ~92%
Vocabulary Size: 8,000+ words
⚙️ How It Works
Input
User enters headline or article
Preprocessing
Lowercasing
Stopword removal
Stemming
Noise removal
Fact Check Layer
Matches against predefined fact database
Model Prediction
CNN extracts features
Bi-LSTM captures context
Outputs probability scores
Multi-Level Mapping
Based on probability thresholds:
P(fake) ≥ 0.75 → Fake
0.55 ≤ P(fake) < 0.75 → Misleading
Otherwise → Partially Real / Real
Explainability
Important words highlighted using LIME
🖥️ Tech Stack
Frontend: HTML, CSS, JavaScript
ML Model: TensorFlow / Keras
NLP: Custom preprocessing + tokenization
Explainability: LIME
