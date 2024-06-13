# Yelp Pulse: Yelp Review Summarizer: Topic Modeling and Sentiment Analysis Using BERT

## Problem Statement & Context
Enhance business owner and customer interactions on Yelp by implementing a "review tags" feature based on sentiment analysis. This feature categorizes reviews into positive, neutral, and negative sentiments and highlights common themes to facilitate better decision-making and improve user engagement.

## Stakeholders
- **Business Owners**: Can leverage insights to improve services and address customer concerns more effectively.
- **Customers**: Benefit from a clearer understanding of business strengths and weaknesses, aiding their decision-making.
- **Yelp Platform**: Enhanced user engagement and satisfaction contribute to Yelp’s operational success and reputation.

## Actions Based on Deliverables
- **Business Owners**: Utilize "review tags" and "sentiment insights" to prioritize improvements and promotional strategies.
- **Customers**: Use sentiment-based tags to make informed choices, enhancing satisfaction and trust in the Yelp platform.

## Criteria for Success
- **Accuracy**: Achieve at least 70% accuracy in sentiment classification.
- **Recall**: Prioritize a recall of 75% to ensure that negative sentiments are not overlooked, crucial for maintaining service quality and customer trust.

## Scope
- **Sentiment Classification**: Categorize reviews into positive, negative, and neutral; assess how sentiments have progressed recently.
- **Sentiment Insights**: Develop a dashboard to visualize sentiment trends over time for different businesses.
- **Review Tags**: Generate and display keywords or phrases commonly mentioned in positive and negative reviews.

## Possible Constraints
- **Time Constraints**: Limited to 4 weeks for project completion.
- **Data Bias**: Review data may be skewed towards positive reviews; insufficient negative data could bias the model.
- **Recent Performance Trends**: Incorporate analysis to highlight recent changes in sentiment, reflecting the current performance rather than historical averages.

## Possible Data Sources
- **Yelp Open Dataset**: Utilize the extensive review and business data provided by Yelp, which includes user-generated reviews and business information.

## Possible Methodology
1. **Data Wrangling & Cleaning**:
   - Assess and clean the Yelp dataset, addressing missing values, duplicates, and potential skewness in the distribution of sentiments.
2. **Exploratory Data Analysis (EDA)**:
   - Analyze how sentiments are distributed among different business categories and identify any variables that are strongly associated with specific sentiments.
   - Visualize sentiment distribution to understand prevailing trends and potential data biases.
3. **Data Preprocessing**:
   - Apply natural language processing (NLP) techniques to extract keywords and phrases from reviews.
   - Prepare the textual data for modeling, including tokenization and vectorization.
4. **Modeling & Hyperparameter Tuning**:
   - Start with baseline models such as Logistic Regression and Random Forest for initial sentiment classification.
   - Develop and train an LSTM model to capture the sequential nature of text data and enhance the accuracy of sentiment classification.
   - Evaluate model performance using metrics like accuracy, precision, recall, F1-score, and ROC AUC.
   - Adjust model parameters based on performance metrics and retrain as necessary.
5. **Sentiment Insights & Review Tags Generation**:
   - Implement algorithms to generate "review tags" based on extracted keywords and identified sentiments.
   - Develop a "Sentiment Insights" feature that visualizes sentiment trends over specific periods to highlight recent business performance.
6. **Model Deployment**:
   - Create an interactive dashboard using Streamlit, allowing users to select a business and view sentiment analysis results, including overall sentiment trends and review tags.
7. **Performance Evaluation**:
   - Conduct user testing to assess the usefulness and accuracy of the sentiment insights and review tags.
   - Gather feedback to refine the model and interface continuously.

## Creative Interface Ideas
- **Interactive Dashboard**: Enable users to dynamically explore sentiment analysis results, with options to filter by time period, review sentiment, and business category.
- **Streamlit Application**: Develop a user-friendly application where stakeholders can easily interact with the model outputs and gain actionable insights.
