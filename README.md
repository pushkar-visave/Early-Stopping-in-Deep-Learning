# Early Stopping in Deep Learning

A small demo showing how early stopping helps a neural network avoid overfitting, using Keras/TensorFlow.

The notebook trains a basic feedforward network on the `make_circles` dataset, once without early stopping and once with it. Without it, the model trains for the full 3500 epochs, and the validation loss starts climbing well before training ends, a clear sign of overfitting. With Keras' `EarlyStopping` callback watching `val_loss`, training stops once validation performance stalls, usually in a fraction of the epochs, and the resulting model generalizes better.

Loss curves and decision boundary plots are included so you can see the difference directly.

**What's inside:**
- Data generation and a quick visualization
- Baseline training run (no early stopping)
- Training run with `EarlyStopping`
- Side-by-side loss curves and decision boundaries
