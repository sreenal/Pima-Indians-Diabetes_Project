 Pima Indians Diabetes Project 
 Input Dataset 
================= 
https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database 
Dataset details
===================
1: Pregnancies: Number of times pregnant 
2: Glucose: Plasma glucose concentration a 2 hours in an oral glucose tolerance test. 
3: BloodPressure: Diastolic blood pressure (mm Hg) 
4: SkinThickness: Triceps skinfold thickness (mm) 
5: Insulin: 2-Hour serum insulin (mu U/ml) 
6: BMI: Body mass index (weight in kg/(height in m)²) 
7: DiabetesPedigreeFunction: Diabetes pedigree function 
8: Age: Age (years) 
9: Outcome: Class variable (0 or 1) 268 of 768 are 1, the others are 0 
Pima_Indians_Diabetes


This Prtoject is aimed at finding of possibility of an person getting diabetic
here we have taken data set from kaggle namely’diabetes.csv’ 
We used the vscode ide for executing the dataset .
The following process of Feature engineering was initially implimented on the dataset:
info()
describe()
value_counts()
isna().sum()
corr()
pairplot()
heatmap()
The above methods enabled us in filtering the dataset and and removing the dataset null values and convert the categerical values into numerical formats
Now the above dataset is splited using ‘train-test-split ‘ from the sklearn preprocessing module
Then the dataset is scale down using StandardScalar(),which sclales down the dataset w.r.t standard deviation, Now the given data is fitted with various models and their accuracy, error  are calulated based on their prediction and the best model is chosen to make our model .pickel file 

The scale pickel ,model pickel file are saved 
Now we create the app.py for hosting our data where we define our flask api method also the scale,and the model pickel files are used to predict the output  here we call  the template folder consisting of index.html and result .html  which are triggered with the load method the from our app.py file
The results are printed on the result page .
Once these results are sucessful our whole project data are loaded on github and the repository name is directed to heroku app thus we deploy the application
 you can find the application on :
https://pidib.herokuapp.com/


