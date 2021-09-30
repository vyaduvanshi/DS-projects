First off, it was obvious from the target feature that this was a binary classification problem.
The first question that came to mind then was how imabalanced it is. It wasn't very imbalanced, so there was no need for resampling.
As there were many classification algorithms to employ, it was known that I would have to scale the features.
There were many features and because of so many zero values, my intuition told me many features could be redundant.



General Approach:

The general approach was to try out various possibilities at each step, computing the cross-val scores to see which fared better. Picked the one with the better
performance, discarded the other. In other words, I treated data transformation as hyperparameters and tried them all. (Eg- Tried 3 methods of feature selection,
picked the one that gave the best scores)

Detailed Approach:

1. Started with basic non-visual exploration of the data (shape, missing values)
2. Explored each variable visually, found that most cells were filled with 0. Interesting.
3. Tried 2 scaling methods, picked the one with better scores. (StandardScaler())
4. Tried 3 feature selection methods, picked the one with the best scores. (RFE)
5. Created pipeline for transformation of validation and test set in the future.
6. Tried several models, picked the best performing ones from them, ran grid search on them to find best hyperparameters.
7. Picked the top performing models, created an ensemble with them and used it to predict on the validation and test set.
8. Results were satisfactory on the validation set, the ensemble model was not overfit on the training set.