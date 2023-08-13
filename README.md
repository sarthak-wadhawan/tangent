# Tangent
The following is a project with the objective to classify digits from 0-9 using MNIST hand-written dataset.
MNIST handdrwan dataset was used to compare techniques and get the best accuracy.
The task was simple; to classify digits from 0-9.
The dataset had 42000 images with 785 columns and in total 33600 samples, to save time 5000 were selected. 4 cases were considered.
1- Gray Scale Images- the orignal gray scale images took 1 minute 14 seconds to fit and 1 minute 4 seconds to score with accuracy of 9.3%.
In the second use case, to improve the accuracy, the images were converted into binary which took the same time to fit and only 16 seconds to score with an improved accuracy of 91%
The third use case contained the gray scale images and PCA (dimensionality reduction technique) was done to reduce computational time. The model was trained in 12 seconds with 92% accuracy and 18 seconds were used to compute the score.
The next use case used the binary images with PCA to check which took 12 seconds to train, had an accuracy of 92% and score was computed in 20 seconds. 
After comparing all the use cases, it was seen that Case 3 and 4 performed the best.
Then to see how increasing the size of the dataset improves the accuracy, the size of the data was increased in every iteration and the accuracy was seen to be increasing after every iteration. The fitting time was also seen to be not increasing as much with every iteration .
Then, hyper parameter tuning was done for SVM with GridSearchCV, we only controlled 2 parameters ("C", "gamma").  Cross Validation was done. Best parameters were selected for C and gamma, and they were assigned to the classification object and then the model was trained again. 

*The csv file is too big for Github therefore it has not been attached. Feel free to contact me if you want the csv file to do the project youreself!
