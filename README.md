# Employee Salary Prediction

This is a capstone project for the Edunet Foundation that predicts whether an individual's annual income exceeds 50K based on demographic and employment data. The project uses a Random Forest Classifier and is deployed as an interactive web app using Gradio.

## 1. Problem Statement

[cite_start]The primary goal is to build an accurate classification model to predict if an individual earns more than 50K per year[cite: 15, 17]. [cite_start]This model analyzes features like age, education level, occupation, and hours worked per week[cite: 16]. [cite_start]Such a tool can assist HR departments in workforce planning, salary benchmarking, and budgeting[cite: 18, 20].

## 2. Tech Stack & Libraries

[cite_start]The model was built using the following tools and libraries [cite: 30-34]:

* [cite_start]**Environment:** Google Colab [cite: 29]
* [cite_start]**Data Manipulation:** pandas [cite: 31]
* [cite_start]**Numerical Operations:** numpy [cite: 32]
* [cite_start]**Data Visualization:** matplotlib [cite: 33]
* [cite_start]**ML & Preprocessing:** scikit-learn [cite: 34]
* [cite_start]**Web App/Deployment:** Gradio [cite: 42]

## 3. Methodology

[cite_start]The project followed a standard machine learning workflow [cite: 37-43]:

### Data Preprocessing
1.  [cite_start]**Load Data:** The `adult.csv` dataset was loaded using pandas[cite: 37].
2.  [cite_start]**Feature Selection:** The model uses the following features: `age`, `education-num`, `hours-per-week`, `workclass`, `occupation`, and `gender`[cite: 40].
3.  [cite_start]**Encoding:** Categorical variables (`workclass`, `occupation`, `gender`, and the `income` target) were converted to numerical values using `LabelEncoder` from scikit-learn[cite: 38]. [cite_start]The `education-num` feature was used as the numeric representation for education[cite: 39].

### Model Training
1.  [cite_start]**Data Split:** The dataset was split into training and testing sets[cite: 40].
2.  **Algorithm:** A **Random Forest Classifier** was chosen for the classification task.
3.  [cite_start]**Handling Imbalance:** The `class_weight='balanced'` parameter was used during training to handle the inherent class imbalance in the income data[cite: 41].

### Deployment
[cite_start]A simple web interface was built using **Gradio**[cite: 42]. [cite_start]This UI accepts user-friendly inputs (e.g., dropdowns for 'Occupation' or 'Gender') and passes them to the prediction function, which returns the income class ('>50K' or '<=50K')[cite: 42, 67].

## 4. Results & Demo

[cite_start]The final model is accessible via a shareable Gradio web app[cite: 43]. [cite_start]The interface allows users to input values for age, education, hours per week, and other factors to receive an instant income prediction [cite: 82-88].

``

## 5. How to Run

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/paTRA9090/Employee-Salary-Prediction.git](https://github.com/paTRA9090/Employee-Salary-Prediction.git)
    ```

2.  **Install dependencies:**
    ```bash
    pip install pandas numpy scikit-learn gradio
    ```

3.  **Run the application:**
    [cite_start]Execute the Python script containing the model training and Gradio interface code [cite: 46-95].
    ```bash
    python your_script_name.py
    ```

4.  [cite_start]**Access the App:** The script will launch a local server and provide a URL (and a public, shareable URL if `share=True` is used) to access the web app[cite: 95].
