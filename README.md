# Neural Network Model Testing and Validation in R

Sample SQL code in the SQL Command.txt file.
Data used in iconicdata.csv.

iconicrcodefinal.Rmd is an r markdown file which includes code to implement some cleaning of the data as well as infer a gender flag based on a rule and then a for loop cross-validating a neural network fitted to a 70/30 training/test split of the data.

In this code I infer gender accross a dataset for male and female items and attempt to predict the resulting gender with a neural network. The initial split is done by a simple if male items > female items for a specific customer then male else female.

The rule is easily learned by the neural network achieving 99% average accuracy over 50 cross validations on a 70/30 training test split. This code is only intended to demonstrate model testing and cross-validation of a neural network in R.
