
This project demonstrates the fundamental concept of overfitting in machine learning models through a hands-on experiment using a Decision Tree classifier and scikit-learn.

## Project Overview

The primary objective of this code is to monitor how the performance of a decision tree model evolves as the tree depth (`max_depth`) increases from 1 to 20. By synthetically generating a classification dataset using `make_classification` and splitting it into training and testing sets, the experiment highlights a crucial machine learning phenomenon. As the tree becomes overly complex with a high depth, it begins to memorize the training data rather than learning underlying patterns—achieving up to 100% training accuracy—while test performance fluctuates or plateaus, which is a classic indicator of overfitting.

## Technologies Used

The implementation relies on Python alongside the scikit-learn library for data generation, dataset splitting, and model training, all documented within an interactive Jupyter Notebook environment.

## How to Run

To run this experiment locally, ensure you have the necessary data science libraries installed by running `pip install numpy scikit-learn matplotlib`. Once installed, open the Jupyter Notebook and execute the cells sequentially to observe the training and testing accuracy metrics across different tree depths.
