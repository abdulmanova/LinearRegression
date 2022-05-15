# LinearRegression
<p> The main machine learning’s approach is identifying relationships
between attributes and targets. The simplest functional relationship that can be
found is linear regression. To define parameters of a function squared or
absolute loss functions are used. Both of these concepts are widely used and the
choice of a loss function strongly depends on a problem. The result of a squared
loss function is a number that describes how far the model's outputs are from
targets. The aim is to minimize the error. Taking derivatives of the loss function
with respect to each weight, the minimum point can be found and, therefore,
most suitable parameters of a model will be identified. However, a model may
become a too complex polynomial which has small error on a training set but
huge error on testing set. There are two ways to cope with over-fitting:
cross-validation and regularization. Cross-validation is a technique of splitting
the data into folds where some folds are used as a training set and the rest as a
validation set. Then compute the average loss. Regularization prevents
over-complexity of a model by means of minimizing the regularized loss.
Regularized loss is a sum of squared loss and squared parameter with a
coefficient. Squared parameter represents complexity of a model and coefficient
penalizes over-complexity.</p>
<p> In my opinion linear regression is a powerful tool. A lot of problems do
not imply too complex solutions. For example, a cost for a product depends on
the materials that were used in production, how long it took to produce, how far
the product was transferred etc. So the final cost can be computed as those
parameters multiplied by a coefficient and then summarized. This assumption is
quite credible and fair. The idea behind cross-validation is impressive: splitting
the training set on the actual training set and a validation set. Meaning that a
model gets tested on the training set too. Cross-validation is used to search for
the best hyperparameters. It helps prevent overfitting because when the model is
trained, the validation identifies the loss score and tells us if the hyperparameter
is suitable. Then the testing set will give us realistic estimation of the model
with the hyperparameters we found. Speaking of regularization, it penalizes a
model for a sum of a loss and model complexity (which is expressed in the
greatest degree of a polynomial). So if a loss is big and a model’s complexity is
low, this implies under-fitting and vice versa. If loss is small and a model is too
complex, it identifies over-fitting.</p>
