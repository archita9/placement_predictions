“This project demonstrates placement prediction using both Machine Learning and Deep Learning. Below is a brief overview of the concepts used.”

**What is ML?**

Machine Learning is the study of algorithms that learn patterns from data instead of relying on hard-coded rules.
ML models improve through experience and can make predictions on new, unseen data.

Common ML models include Logistic Regression, Decision Tree, Random Forest, and SVM.

**What is DL?**

Deep Learning is a subfield of ML that uses neural networks with multiple layers.
Each layer learns increasingly meaningful representations from data, allowing models to capture complex relationships.

Q.  **Why do we need DL when we already have ML?**

ML works well for **simple problems and small/structured datasets**, but has limitations:

* Accuracy saturates after a point
* ML requires manual feature engineering
* ML struggles with highly complex patterns
* Increasing iterations does NOT significantly improve ML performance

DL becomes necessary when:

* Dataset is large
* Patterns are complex
* Automated feature learning is required

**Figure:** <img width="609" height="412" alt="image" src="https://github.com/user-attachments/assets/00493afe-597e-4b02-8668-b9f062df6d87" />
 My Project: Placement Prediction (ML vs DL)

To understand the practical difference between ML and DL, I built a **Placement Prediction system** that predicts yearly placement outcomes based on:

* Number of companies visiting
* Students placed
* Highest package
* Job roles offered
* Year-wise trend patterns

*1*. **Placement Prediction using Machine Learning**

In the ML approach, I used **scikit-learn (sklearn)** to build traditional machine learning models for predicting placement outcomes. These models learn from historical data such as number of companies visiting, students placed, job roles offered, and highest package.

**What the ML model does:**

* Fits simple relationships between features
* Learns trends over the years
* Predicts placement count and package values

**Observation (from the graph):**
<img width="1226" height="595" alt="image" src="https://github.com/user-attachments/assets/08a018bd-0b03-4c89-af45-abc0992e044b" />

The ML model performed well in the beginning — the predicted values were close to the actual values.
However, after a point, the model started **lagging behind**. This happens because:

* ML models rely heavily on manually created features
* They struggle when relationships become more complex
* Accuracy saturates even if we increase iterations

So ML works well as a **baseline model**, but it does not capture deeper, non-linear patterns.

 2. **Placement Prediction using Deep Learning**

To improve and understand the difference, I built a Deep Learning model using **Keras**, part of TensorFlow.
Unlike ML, DL learns features automatically through multiple layers.

**What the DL model does:**

* Uses more layers to learn complex patterns
* Captures non-linear relationships in historical data
* Can theoretically improve with more data

**Observation (from the graph):**
<img width="925" height="573" alt="image" src="https://github.com/user-attachments/assets/c8d19d87-3c1b-436f-bc1b-e580960c928a" />

In the DL results:

* The starting values were lagging
* The last predicted values were also not perfect

This happened because **Deep Learning requires a very large dataset** to learn properly.
Since our dataset has only a few rows (year-wise data), the model doesn’t get enough examples to generalize.

“Overall, this project highlights how traditional ML models perform strongly on smaller datasets, while DL models require much larger data to achieve meaningful improvements.”

**Key takeaway:**

* ML works well for small datasets
* DL performs better only when the dataset is large enough
* With limited data, DL cannot reach its full potential

How to View the Notebooks

Open placement_data(ml).ipynb to review the Machine Learning model and its predictions.

Open placement_data(dl).ipynb to review the Deep Learning model built using Keras.

Both notebooks can be viewed directly on GitHub without downloading.

Each notebook contains its own workflow, visualizations, and final outputs.


Just tell me.
