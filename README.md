# Analyzing World Unemployment Rates from 1991-2021
**A Course Requirement for the Subject Data Science and Artificial Intelligence**

Submitted by: Group 6

Group Members:
Bautista, Lotes Kaye S.
Loyola, Dave Jarold T.
Marquez, Djullance M.
Salandanan, Jericho M.

Submitted to: Engr. Aisa M. Labastilla, PCpE

Date: January 23, 2024

![image](https://github.com/LotesKaye/ECEData/assets/155596606/9c9abaa5-4ff4-4575-a26f-103afa66bb72)



# Introduction / Problem Statement

Unemployment is considered as a key measure of economic health. It becomes an indicator of the economic struggle of workers to obtain work and contribute to the economy of a country. It simply implies that the higher the unemployment rate, the less total economic production. The measure of unemployment excludes people who leave the labor force due to reasons like disability, pursuit of higher education, and retirement. Additionally, the unemployment rate is usually used as its key indicator, which is determined by dividing the number of unemployed individuals by the total labor force [1]. 

The project is about the analysis of world unemployment rates from 1991 to 2021. The aim of analyzing this problem is to gain insight into global employment trends over the last three decades and understand how various economic, social, and political issues influence employment rates. The Sustainable Development Goal (SDG) addressed by this project is SDG 8: "Decent Work and Economic Growth." This goal aims to foster long-term, inclusive, and sustained economic development, full and productive employment, and decent jobs for all [2].

Through the analysis of global unemployment rates, an in-depth analysis of the global employment landscape is provided as it correlates with this objective. It is also vital in promoting economic growth and ensuring that all individuals will have access to job opportunities.


# Review of Related Literature

**What Is Unemployment**

    Unemployment serves as a crucial economic indicator, reflecting the capacity of workers to secure gainful employment and contribute to overall economic productivity. A higher number of unemployed individuals corresponds to a reduction in total economic production. Conversely, a low unemployment rate indicates that the economy is likely operating close to its full capacity, fostering increased output, wage growth, and elevated living standards. Nevertheless, an excessively low unemployment rate may signal potential challenges, such as an overheated economy, inflationary pressures, and tight labor conditions for businesses seeking additional workers. Balancing unemployment rates is essential for maintaining a healthy economic equilibrium that encourages sustainable growth and prosperity [1].


**Global unemployment rate 2003-2022**

    In 2022, the global unemployment rate exhibited a notable decline, decreasing by 0.4 percentage points (-6.45 percent) compared to the previous year. The unemployment rate represents the proportion of the economically active population actively seeking employment but currently without work. It is important to note that this metric excludes economically inactive groups, including long-term unemployed individuals, children, and retirees. This decrease in the unemployment rate suggests a positive trend in economic conditions, reflecting an increase in employment opportunities for the actively engaged workforce worldwide [4].


**Youth Unemployment Causes and Solutions**

    Globally, the reported figure of 73 million unemployed youth belies the actual extent of the issue, with 620 million identified as not in employment, education, or training (NEET) by the World Bank. The origins of youth unemployment are complex, rooted in various factors. The aftermath of the financial crisis exacerbated pre-existing challenges in labor markets and education systems, leading to precarious job opportunities. Widespread skills mismatch, attributed to inadequate vocational training and curricula misaligned with industry needs, further impedes young people. Additionally, the absence of entrepreneurship and lifeskills education, coupled with challenges in accessing capital for aspiring entrepreneurs, exacerbates the problem. In low-income countries, a digital divide compounds the skills gap, restricting opportunities for those lacking access to technology. Addressing these intertwined challenges is imperative for developing comprehensive global solutions to youth unemployment [5].


**Unemployment and mental health**

    Unemployment, characterized by the absence of employment while actively seeking work, consistently associates with detrimental health outcomes. The negative impact encompasses stress, diminished self-esteem resulting from job loss, financial hardships, insecurity, and reduced future earnings potential. The social security system, involving processes like claims, work capability testing, and job search conditions, can exacerbate mental health challenges. Extended periods of unemployment worsen these consequences, impacting mental health, life satisfaction, and physical well-being. Prolonged pandemic-related restrictions, causing extended periods of reduced income and job loss, amplify concerns regarding the enduring health effects of such circumstances [6].


**Global Unemployment Crisis Continues**

    Within the world's wealthiest nations, encompassing members of the Organization for Economic Cooperation and Development (OECD), approximately 34 million individuals find themselves unemployed. In the European Union, there has been a notable rise in unemployment over the past year, reaching an average of 11.3 percent of the workforce, with significant increases observed in countries such as France, Germany, Italy, and Sweden. In contrast, the United States has experienced intensified job creation, leading to a dip in unemployment below 5 percent. While both the U.S. and the United Kingdom have seen declines in unemployment rates, there is a simultaneous trend of widening income disparities in these countries [7].


**COVID-19 has led to massive job losses, particularly among youth and women**

    In 2020, the global unemployment rate rose to 6.5 percent, marking a 1.1 percentage point increase from the previous year. The number of unemployed individuals worldwide surged by 33 million, reaching a total of 220 million, with an additional 81 million people exiting the labor market entirely. Latin America and the Caribbean, as well as Europe and Northern America, experienced unemployment rate hikes of at least 2 percentage points. Notably, youth and women faced disproportionate impacts, with employment losses of 8.7 percent and 5.0 percent, respectively, compared to 3.7 percent for adults and 3.9 percent for men. Before the pandemic, youth unemployment was already three times higher than that of adults. The crisis prompted more women than men to leave the labor force for childcare responsibilities, exacerbating longstanding gender gaps in labor force participation rates [8].


# Gathered Data / Dataset
    The "New Unemployment dataset" was gathered from the website Kaggle. Originally named "unemployment dataset", it was created by ANJALI PANT to describe the health of the world economy for the past 31 years in terms of its unemployment rate. The dataset contains about 235 countries, some countries in particular are divided based on their cardinal directions, which is why the countries in total are 235 instead of 195. The file contained about 40.7KB and was imported in a CSV format, but was later changed by the proponents to 203KB to better suit the lines of codes that the proponents will use in training and testing. Each country contains data regarding their rate of unemployment dating from 1991 to 2021 with its corresponding value per year. Furthermore, the four columns in the dataset are divided into Country Names, Country Codes, Year, and Value. Overall, the modified dataset contains four columns and 7,286 rows in a CSV format. The original dataset can be accessed through the link below and the modified dataset can be accessed in the link below the original dataset.
    
Original_Dataset: https://www.kaggle.com/datasets/pantanjali/unemployment-dataset/data?fbclid=IwAR2nDIx9V6DhVvrf2i3hHAzlRxo2SLuMyv7kPb_mePkA4fSB-nDpvzp9KNk


Modified_Dataset: https://drive.google.com/file/d/16DuzGWF388gDlliL9a687Xf9Z3KID2Nm/view?usp=drive_link


# Objectives
    The main objective of the project is to comprehensively analyze world unemployment rates from 1991 to 2021, contributing to a better understanding of global employment trends and their implications for Sustainable Development Goal 8: Decent Work and Economic Growth. To achieve the main objective, the project specifically aims to:
·	Import Data for training and testing.
·	Analyze the data and create a graph.
·	Filter the dataset to the chosen country (Philippines)
·	Analyze the data from the chosen country.
·	Write a code for a Linear Regression and Logistic Regression analysis.
·	Train the models with the chosen dataset
·	Display the graphical results of each model.


# Conceptual
    The provided code includes essential Python library imports for data analysis and visualization, with NumPy imported as 'np,' Pandas as 'pd,' Matplotlib for plotting as 'plt,' and Seaborn as 'sns.' Additionally, the code brings in the Linear Regression model from scikit-learn. Warnings are imported to manage warning messages, and the statement 'warnings.filterwarnings("ignore")' is employed to suppress these warnings. Finally, '%matplotlib inline' is a Jupyter Notebook magic command that ensures Matplotlib plots are displayed directly in the notebook. Together, these imports and configurations establish a comprehensive environment for conducting data analysis and creating visualizations.
    
    To import a dataset in CSV format for analysis, the code snippet utilizes the Pandas library in Python. By specifying the path to the CSV file and using the pd.read_csv() function, the dataset is read and loaded into a Pandas DataFrame named 'df.' This DataFrame serves as a tabular representation of the data, providing a versatile structure for subsequent analysis and exploration. Adjust the file path within the code to match the location of the specific CSV file being used. Once the dataset has been imported, the checking for any null values is performed to ensure that there are no null values in the dataset. If there were any null values, adjustments would be needed to handle them appropriately.
    
    Next, plotting the dataset initially results in a graph with several lines, making it crowded. To focus on the Philippines, the code filters the dataset using the statement 'country = df[df[‘Country Code’] == ‘PHL’].'

    A Linear Regression model is instantiated using scikit-learn's LinearRegression class. The model is then trained on the training data using the fit method, where 'X_train' represents the independent variable (features) and 'y_train' represents the dependent variable (target). This process involves adjusting the parameters of the linear regression model to minimize the difference between the predicted values and the actual values in the training set. After the execution of these lines, the 'model' variable holds a trained linear regression model ready for making predictions on new or unseen data based on the learned patterns from the training set.
    
    Predictions on the test set are generated using the trained Linear Regression model. The model.predict(X_test) function applies the learned patterns from the training set to the independent variable 'X_test,' resulting in the predicted values stored in the 'y_pred' variable. The subsequent lines, where 'test_predict' is assigned the predicted values, represent an identical prediction procedure. The 'test_predict' variable now contains the model's predictions for the test set, which can be further evaluated and compared against the actual target values ('y_test') to assess the model's performance.
    
    Scikit-learn's metrics modules are utilized to compute and evaluate the performance of the Linear Regression model on the test set. The mean absolute error (MAE) and mean squared error (MSE) are calculated using the mean_absolute_error and mean_squared_error functions, respectively. These metrics provide quantitative measures of the model's accuracy by comparing the predicted values ('y_pred') with the actual target values ('y_test'). The computed MAE and MSE values are then printed, offering insights into the average magnitude and squared differences between the predicted and actual values. Lower values for both metrics generally indicate better predictive performance.
    
    For Logistic Regression, a binary classification task is initiated by setting a threshold value of 2. The 'Values' column is created in the Pandas DataFrame 'df' to represent binary classifications (1 for values greater than the threshold, and 0 otherwise) based on whether the 'Value' column exceeds the specified threshold. The independent variable 'X' is assigned the 'Year' column, and the dependent variable 'y' is set to the newly created 'Values' column. The dataset is then split into training and testing sets using the train_test_split function, following the same principles as before. This sets the stage for training and evaluating a machine learning model for binary classification based on the selected features.
    
    A Logistic Regression model is instantiated using scikit-learn's LogisticRegression class. The model is then trained on the training data using the fit method, where 'X_train' represents the independent variable (features) and 'y_train' represents the binary target variable (0 or 1). Logistic Regression is suitable for binary classification tasks, and the fit process involves learning the parameters that best fit the logistic regression equation to the training data. After this step, the 'model' variable holds a trained logistic regression model ready for making predictions on new or unseen data.
    
    The Logistic Regression model is evaluated on the test set using key classification metrics. The predict method is employed to obtain model predictions, and scikit-learn's metrics modules are utilized to compute accuracy, precision, recall, and F1 score. Accuracy measures the overall correctness of predictions, precision assesses the accuracy of positive predictions, recall evaluates the ability to capture positive instances, and F1 score provides a balanced metric between precision and recall. The resulting scores are printed, offering insights into the model's effectiveness in binary classification.
    
    A new data point is represented by the value '2.7' for the 'Year' feature. The Logistic Regression model is then used to predict the corresponding binary classification, indicating whether the 'Value' (unemployment rate) is above the threshold set earlier. The prediction is obtained using the prediction method with the new data point, and the result is printed to the console. This allows for the model's application to unseen data, providing a binary classification prediction for the given 'Year' value.


# Data and Results (Visualization)
![image](https://github.com/LotesKaye/ECEData/assets/155596606/a3899412-687d-4a18-89df-dd3a3ba998f6)
    The visual complexity observed in the graph is due to the inclusion of data for every country in the dataset. Each line on the plot represents the unemployment rates of different countries, resulting in a dense and cluttered appearance. This makes it challenging to discern distinct trends or patterns, as the numerous overlapping lines create a graph that appears chaotic and lacks clear organization.

![image](https://github.com/LotesKaye/ECEData/assets/155596606/e434b5eb-47d0-4987-bf73-1f09effc1d5b)
    The analysis will specifically concentrate on the Philippines. To enhance the clarity and interpretability of the graph, the code snippet 'country = df[df[‘Country Code’] == ‘PHL’]' is employed. This filters the dataset to isolate data pertaining solely to the Philippines. Consequently, the resulting graph will be more organized and easier to understand, exclusively representing the unemployment rates of the selected country.

![image](https://github.com/LotesKaye/ECEData/assets/155596606/4e89c484-3c49-4e01-a592-26aea9c6ab59)
    For Linear Regression, Matplotlib is used for data visualization. A scatter plot is created using the 'Year' and 'Value' columns from the Pandas DataFrame 'df' to display the actual data points. Additionally, a red regression line is overlaid on the scatter plot using the 'X_test' values and corresponding predictions ('y_pred') from the trained Linear Regression model. The resulting visualization provides a visual representation of the model's fit to the data, helping to assess how well the linear regression captures the underlying patterns. The title, xlabel, and ylabel functions are used to label the plot appropriately, enhancing its interpretability. The plt.show() function is then called to display the plot.

![image](https://github.com/LotesKaye/ECEData/assets/155596606/d7d35b6a-266f-47dd-8b23-46e0dcd1004a)
    For Logistic Regression, a logistic regression curve is visualized alongside the scatter plot of the original data points using Matplotlib and NumPy. The x_values array is generated to cover a range of years (1990 to 2021), and the logistic function is applied using the model coefficients (model.coef_ and model.intercept_) to calculate corresponding y_values. The scatter plot displays the original data points in blue, and the logistic regression curve is overlaid in red. This visualization provides an illustration of how the logistic regression model fits the binary classification task based on the 'Year' feature. The x-axis represents the years, the y-axis represents the binary values (0 or 1), and the logistic curve depicts the model's probability estimates across the specified range of years. Labels and a legend are included to enhance interpretability.


# Conclusion
    In conclusion, the proponents were able to import the dataset and create an initial graph depicting global unemployment rates for every country in the dataset. However, the graph appears visually complex and cluttered due to the multitude of overlapping lines, making it challenging to discern specific trends or patterns. To address this issue, the analysis focuses specifically on the Philippines, utilizing a code snippet to isolate and present the country's unemployment rates in a more organized and interpretable manner.
    
    The proponents trained the models using the filtered dataset. The subsequent visualizations employ Linear Regression and Logistic Regression techniques using Matplotlib, Pandas, and NumPy. The Linear Regression plot showcases the model's fit to the data, aiding in assessing its ability to capture underlying patterns. Similarly, the Logistic Regression visualization features a logistic regression curve alongside the scatter plot of original data points, providing a clear representation of the model's application to the dataset.
    
    These refined visualizations enhance the interpretability of the data and facilitate a more insightful analysis of unemployment trends in the Philippines. The capstone project proves highly beneficial by addressing the visual complexity of the initial global unemployment graph through a focused analysis on the Philippines. This approach enhances interpretability and showcases practical data manipulation skills.
    
    The subsequent visualizations, employing Linear and Logistic Regression techniques, not only provide insights into the underlying patterns of unemployment data but also demonstrate the practical application of machine learning models. The integration of Matplotlib, Pandas, and NumPy in these visualizations adds real-world relevance, contributing to a comprehensive learning experience.
    
  Overall, the capstone project serves as a valuable opportunity to apply and solidify data science skills, fostering a deeper understanding of data analysis and modeling techniques.


# Program Codes / MATLAB/ Google collab / Jupyter notebook or spyder IDE 


# References

References

[1] 	A. Hayes, "What Is Unemployment?," Investopedia, 9 August 2023. [Online]. Available: https://www.investopedia.com/terms/u/unemployment.asp#:~:text=What%20Is%20Unemployment?. [Accessed 13 January 2024].
[2] 	"The Global Goals," [Online]. Available: https://www.globalgoals.org/goals/8-decent-work-and-economic-growth/. [Accessed 13 January 2024].
[3] 	A. O'Neill, "Global unemployment rate from 2003 to 2022," statista, 12 December 2023. [Online]. Available: https://www.statista.com/statistics/279777/global-unemployment-rate/. [Accessed 20 January 2024].
[4] 	peace, "Youth Unemployment Causes and Solutions," Peace Child International, 9 September 2015. [Online]. Available: https://peacechild.org/youth-unemployment-causes-and-solutions/. [Accessed 20 January 2024].
[5] 	H. Wilson and D. Finch, "Unemployment and mental health," The Health Foundation, 16 April 2021. [Online]. Available: https://www.health.org.uk/publications/long-reads/unemployment-and-mental-health. [Accessed 19 January 2024].
[6] 	International Labour Organization, "Global Unemployment Crisis Continues; Wage Inequalities Rising, Says ILO Renewed International Commitment to Full Employment is Needed," International Labour Organization, 2024. [Online]. Available: https://www.ilo.org/global/about-the-ilo/newsroom/news/WCMS_008083/lang--en/index.htm. [Accessed 19 January 2024].
[7] 	United Nations, "COVID-19 has led to massive job losses, particularly among youth and women," United Nations, 2020. [Online]. Available: https://unstats.un.org/sdgs/report/2021/goal-08/. [Accessed 19 January 2024].


