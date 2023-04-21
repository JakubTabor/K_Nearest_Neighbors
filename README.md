# K_Nearest_Neighbors
# I have my "X" and "y" prepared, so I can import "train_test_split" and get "train" and "test" set
# Then from "preprocessing" I get "StandardScaler" to make "feature scaling" 
# Prepare my "X_train" ""X_train = sc.fit_transform(X_train)""" and "X_test" """X_test = sc.transform(X_test)"""
# Then from "sklearn.neighbors" I import "KNeighborsClassifier" and set parameters in my "classifier"
# I set "n_neighbors" on (5), so my classifier is gonna take five closest points
# And default "metric" "minkowski" which results are the standard "Euclidean" distance, in this case I need to set also "precision" at (2)
# And save all as "classifier" """classifier = KNeighborsClassifier(n_neighbors = 5, metric = 'minkowski', p = 2)"""
# Then I train my data """classifier.fit(X_train, y_train)"""
# I also check some predictions """classifier.predict(sc.transform([[30,87000]]))"""
# And prepare "y_pred" on my "X_test" """y_pred = classifier.predict(X_test)"""
# Finally I get "confusion_matrix" and put into my "y_test" and "y_pred" """confusion_matrix(y_test, y_pred)"""
