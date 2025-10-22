# Digit_Recognition_Part_1
Digit recognition problem using the MNIST (Mixed National Institute of Standards and Technology) database.

| Model                    | Representation | Nonlinearity              | Error              | Lesson                         |
| ------------------------ | -------------- | ------------------------- | ------------------ | ------------------------------ |
| Softmax                  | 784 raw pixels | None                      | ~0.15              | Linear baseline                |
| PCA + Softmax            | 18D/10D PCA    | None                      | ~0.15              | Compression ≠ information loss |
| Cubic Features + Softmax | 10D → 285D     | Manual                    | ~0.1               | Nonlinear mapping helps        |
| Cubic Polynomial SVM     | Kernel trick   | Automatic polynomial      | ~0.07              | Nonlinear kernels work better  |
| RBF SVM                  | Kernel trick   | Infinite-dimensional      | ~0.06              | Most flexible, best accuracy   |

| Model                       | Main Takeaway                                                        |
| --------------------------- | -------------------------------------------------------------------- |
| Linear / Softmax Regression | Built baseline; limitations of linear decision boundaries.           |
| PCA + Softmax               | Reduced dimensionality; kept performance while improving efficiency. |
| Cubic Feature Mapping       | Added hand-crafted nonlinear terms to capture curved patterns.       |
| Kernel SVM (Poly, RBF)      | Used kernel trick for automatic nonlinearity; accuracy gain.         |

# Key Skills:

Implemented gradient descent softmax regression from scratch

Applied PCA for feature reduction

Used scikit-learn SVMs with polynomial / RBF kernels

Compared models via error analysis and hyperparameter tuning

Gained intuition about linear → nonlinear → kernelized learning

# NEXT: Neural Networks on this classification problem.
