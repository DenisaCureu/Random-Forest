# Random-Forest
Python

The full description of the project is presented in the document "Random Forest.pdf"

Random forest is a machine learning technique that is used to solve regression and classification problems.
For classification tasks, the result of radom forest is the class selected by most trees. For regression tasks, the mean or mean prediction of the individual trees is returned.
![Image](https://github.com/user-attachments/assets/5e5432f0-196e-486d-9c5e-f62c035d9708)

General characteristics:

✓ It is based on the vote of m random trees, where m is a
Input parameter

✓ Generate m drive sets

✓ A random tree is trained for each set

✓ For a test instance, each tree gives a class membership
vote

✓ The class with the most votes is the answer to Random
Forest

#Database -women

![Image](https://github.com/user-attachments/assets/13a45307-280f-4372-84c1-f5f853f36a29)

Creating the model: 3 trees and 3 levels:
![Image](https://github.com/user-attachments/assets/80bda2d7-8cf2-469c-a0f1-4e976db6af04)

#Experimental results

Comparison of predicted labels with real labels:
![Image](https://github.com/user-attachments/assets/4236a72b-ffa2-488a-bc39-68bcdf0505dd)

- Tree 1
  ![Image](https://github.com/user-attachments/assets/faf21b7b-64ac-4fa8-8515-8f0846a3a023)
- Tree 2
  ![Image](https://github.com/user-attachments/assets/182df4c9-c362-4da2-9743-5a4361acb3f9)
- Tree 3
  ![Image](https://github.com/user-attachments/assets/36000225-ba08-453a-b937-8c

  Relationship between recall and accuracy for all three classes in individually is captured in the score F1, which is the harmonic mean between recall and accuracy - the model does well for class 0, quite bad for class 1 and decent for class 2.
 Looking at the confusion matrix, we can see that most mistakes are when we classify 52 records of medium risk as low risk, which provides additional insight into low class 1 recalls.

![Image](https://github.com/user-attachments/assets/7372a2af-17b4-47cc-baf6-7f8bc4233d9d)

The classifier mostly takes into account blood glucose, then a little bit of diastolic pressure, body temperature and just a little age to make a decision, this could also be related to Class 1 low recall, perhaps the medium-risk data relates to characteristics that are largely not considered by the model.

![Image](https://github.com/user-attachments/assets/f259ad80-d5c0-40cc-b090-b1ac9252a665)

The advantage of this algorithm is that it is very stable. Even if a new data feature is introduced into the dataset, the overall algorithm is not affected too much because the new data may have a impact on a tree, but it is very difficult for it to have a impact on all trees.
A disadvantage of this algorithm would be its complexity.
