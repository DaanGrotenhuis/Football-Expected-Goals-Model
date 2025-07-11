# Football-Expected-Goals-Model
This project explores how temporal tracking data from youth football matches can enhance Expected Goals (xG) predictions using deep learning. Traditional xG models rely on isolated snapshot features like shot angle and distance, but this work incorporates 5 seconds of sequential ball and player movement data prior to each shot. The aim: compare a simple fully connected model to an LSTM architecture that captures contextual play buildup to improve goal probability estimation.

Key Highlights:
- Based on real match data from youth teams
- Features extracted include distance, angle, average opponent pressure, and defenders in trajectory.
- Temporal model: LSTM + FCL; Baseline: FCL-only.
- Data imbalance tackled using SMOTE and class weighting.
- Comparison of validation accuracy, loss curves, and class-wise performance across models.

Why It Matters:
- Shows how smaller clubs and youth programs can use affordable GPS data to build their own analytics pipelines.
- Demonstrates the value of modeling action sequences, not just shot moments, in predicting goal likelihood.
- Offers a cost-effective alternative to video-based xG systems for under-resourced teams.

Visualization of Results:

<img width="790" height="505" alt="image" src="https://github.com/user-attachments/assets/ee2a5cd9-02d8-4103-ad72-47c290da9bd6" />
<img width="568" height="455" alt="image" src="https://github.com/user-attachments/assets/d282bfab-cdc4-419d-9a16-fd6d0b3f66e4" />

