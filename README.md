#Body Fat Percentage Prediction Using Machine Learning

The project aimed to develop algorithms to predict body fat percentage based on various body measurements, leveraging machine learning techniques to understand the relationships between physical attributes and body fat.

**Technologies Used**
_Programming Language:_
Python
_Libraries:_
Scikit-learn: For implementing machine learning algorithms (K-Nearest Neighbors and Decision Trees).
NumPy: For numerical operations and data manipulation.
Pandas: For data handling and preprocessing.
Matplotlib/Seaborn: For data visualization (scatter plots, etc.).
Data Source: Kaggle (Body Fat Prediction Dataset)

**Methodology**
Dataset Selection:

I chose a dataset from Kaggle containing body fat percentage predictions of 252 men, along with measurements such as weight, height, age, and circumferences of various body parts.
Data Preparation:

Data Cleaning: I analyzed and cleaned the dataset by removing outliers and irrelevant columns. For example, entries with body fat percentages of 0% or 0.7% were discarded, as they were unrealistic.
Normalization: I converted height and weight measurements from inches and pounds to meters and kilograms to maintain consistency in the metric system.
Central Tendency Measures: Calculated mean, median, and mode to understand the data distribution. The mean was found to be 18.91%, and the median was 20.35%, with no mode detected.
Algorithm Implementation:

I implemented two regression algorithms: K-Nearest Neighbors (KNN) and Decision Tree.

**KNN:** I selected this algorithm due to its simplicity and interpretability. After experimenting with various values for k, I found that 𝑘 = 5  provided the best accuracy for my dataset.

**Decision Tree:** Although simpler and more interpretable, it performed slightly worse than KNN. I set the random state to ensure reproducibility.
Model Training and Testing:

I split the dataset into 80% for training and 20% for testing to evaluate the model’s performance.
I assessed the accuracy of both algorithms based on their predictions compared to actual values.

**Findings**
KNN Results:
The KNN algorithm achieved an average accuracy of 69.67%, correctly predicting body fat percentages for approximately 35 out of 50 test instances. This result was encouraging, demonstrating that the algorithm learned effectively from the training data.

Decision Tree Results:
The Decision Tree algorithm yielded a slightly lower accuracy of 61.87%. While it provided insights into the decision-making process, it did not outperform the KNN algorithm in this scenario.

**Lessons Learned:**

I gained valuable experience in data cleaning, algorithm selection, and implementation.
The importance of understanding data relationships was highlighted, as KNN performed better with the dataset's characteristics.
I learned how to handle outliers and redundant features to improve the quality of the data.
Conclusion
Overall, this project enhanced my understanding of machine learning algorithms, particularly KNN and Decision Trees, and their application in predicting continuous variables like body fat percentage. The experience reinforced the significance of data preparation and the selection of appropriate algorithms to achieve accurate predictions.

References
Various online articles, tutorials, and textbooks on machine learning and data cleaning techniques.
Dataset link: Kaggle Body Fat Prediction Dataset.
