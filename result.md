# Training Results & Analysis

## Model Performance
| Metric | Value |
|--------|-------|
| Training Accuracy | 87.32% |
| Validation Accuracy | 87.97% |
| Training Loss | 0.3923 |
| Validation Loss | 0.3661 |
| Total Parameters | 2,624,742 |
| Trainable Parameters | 366,246 |

## Training Curves
![Training History](training_history.png)

## Key Observations
- Model converges well by epoch 5
- Validation accuracy peaks at epoch 10
- No significant overfitting observed
- Early stopping patience set to 5 epochs

## Disease Classes (38 total)
- Apple Scab, Apple Black Rot, Apple Rust, etc.
