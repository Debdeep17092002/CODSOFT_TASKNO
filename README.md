🎬 Movie Genre Classifier

Predict a movie's genre from its title and plot summary using TF-IDF features and classic linear classifiers (Naive Bayes, Linear SVM, Logistic Regression).

The best model, a class-balanced Logistic Regression, reaches ~60% accuracy and 0.42 macro-F1 across 27 genres on a 54,200-movie held-out test set.

Results

Evaluated on test_data_solution.txt (54,200 movies, 27 genres):

Model	Accuracy	Macro-F1	Weighted-F1
Complement Naive Bayes	0.572	0.280	0.517
Linear SVM (balanced)	0.576	0.401	0.581
Logistic Regression (balanced)	0.597	0.422	0.597

The final model is chosen by macro-F1, because plain accuracy rewards a model that ignores rare genres.

Best-performing genres (F1): western 0.87 · documentary 0.76 · game-show 0.72 · horror 0.65 · drama 0.64

Hardest genres (F1): biography 0.05 · history 0.09 · mystery 0.15 · fantasy 0.20
