# ID2223 LAB1

The "titanic_source_code" folder contains the scouce codes to implement the data preprocessing, feature creating, training and Gradio Application creating of the titanic dataset.

The "iris_source_code"folder contains the scouce codes to implement the feature creating, training and Gradio Application creating of the iris dataset.

The "titanic_uis" folder contains the URLs of an interactive UI and a dashboard UI of titanic prediction task.

The "iris_uis" folder contains the URLs of an interactive UI and a dashboard UI of iris flower classfication task.

# # Data preprocessing
We only pick seven features to train the model. They are "Title", "Sex", "Pclass", "Embarked", "Fare", "Age" and "IsAlone", where "IsAlone" is a feature created by combining the "SibSp", "Parch" and "Family Size" features. So we drop the "Ticket", "Cabin", "Name" and "Passenger ID" features
1. Filling the blanks in the "Embarked" column.
2. Mapping the categorical features such as "embarked", "title" and "sex" in the original titanic dataset to the numbers.
3. Classifying the "fare" and "age" features to different bands and using one distinct number to encode one band.
4. Substituting the "SibSp", "Parch" and "Family Size" features to one feature which is a combination of them called "IsAlone" and use 0 and 1 to encode this new feature.

