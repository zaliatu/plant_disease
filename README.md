Automated Plant Disease Detection Using CNN

Course: Artificial Intelligence - UEB
Domain: Computer Vision & Smart Agriculture
Model: Custom Multi-Layer CNN

Team Members
1. DJAN KONAMAH ADELAIDE - UEB3517623
2. MUMUNI ZALIATU - UEB3511923
3. OWUSUAA CHARLOTTE - UEB3506223

Problem Statement
Traditional disease detection relies on agricultural experts, which is costly and not accessible to smallholder farmers. This project uses deep learning to automatically detect tomato leaf diseases.

Classes Detected
We classified 4 tomato leaf classes:
• Tomato Early Blight - Fungal disease with concentric brown spots
• Tomato Late Blight - Water-soaked dark lesions
• Tomato Leaf Mold - Pale green/yellow spots
• Tomato Healthy - No disease

Dataset
Kaggle Plant Village Dataset - Tomato leaves
• Image size: 128 x 128 x 3
• Data Augmentation: Rotation 20 deg, shift, shear, zoom 0.2, horizontal flip

Methodology
• Model: CNN with Conv2D, Max Pooling, Dropout, Dense layers
• Training: 20 epochs, Adam optimizer, lr=0.001, batch size=32
• Loss Function: Categorical crossentory
Results
• Training Accuracy: 96.4%
• Validation Accuracy: 93.8%
• Macro Average: Precision 0.94, Recall 0.94, F1-Score 0.94

Best performance:
• Healthy: 97% precision, 98% recall
• Leaf Mould: 95% precision

How to Run
1. pip install tensor flow NumPy matplotlib
2. python train.py
3. python app.py

Conclusion
The model successfully classifies tomato diseases and can help farmers with early detection to reduce crop damage.
