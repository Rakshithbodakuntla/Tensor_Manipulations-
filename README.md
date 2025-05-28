700772672
Rakshith Bodakuntla



1.	What patterns do you observe in the training and validation accuracy curves?
   
Training accuracy typically increases steadily over epochs as the model learns the training data.
Validation accuracy usually also increases initially, showing that the model is generalizing well to unseen data.
If both curves rise and then plateau at similar levels, it suggests good model fit.
If training accuracy keeps improving but validation accuracy stalls or decreases, it may indicate overfitting.
Sometimes, validation accuracy fluctuates more because of less data or noise in the validation set

2.	How can you use TensorBoard to detect overfitting?
Overfitting happens when the model learns training data too well but fails to generalize.
In TensorBoard, overfitting shows as:
Training accuracy continuing to improve while
Validation accuracy stops improving or starts to decline
Training loss decreasing steadily but
Validation loss plateauing or increasing
Such divergence between training and validation curves is a red flag.

3.	What happens when you increase the number of epochs?
Initially, both training and validation accuracy improve, and losses decrease.
If you train for too many epochs without regularization:
Training accuracy may approach 100%
Validation accuracy may plateau or degrade (overfitting)
Validation loss may start to increase after some point
To combat this, techniques like early stopping, dropout, or regularization are used.
More epochs give the model more time to learn, but without controls, it can overfit.
