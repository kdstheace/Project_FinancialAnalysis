# **Predicting Bankruptcy with Deep Learning Algorithm**
## 1. Description
### Intro
  Predicting Bankruptcy with financial statement.
  Analysis main features of financial statement such as ROA, Turnover rate,
  and even tax rates, it shows whether the company will bankrupt or not, and its
  possibilities.
### Why Predict Bankruptcy?
  1. For managers to deal with financial risk in advance
  2. For investors to make sure whether companies are valuable or not
  3. For Banks to predict the risk for their loan over companies
### Duration
  - 2021-04-12 ~ 2021-05-31
### Team
  - Dongsoo Kim (Daniel)
  - Minyoung Kim (Aphie)
### Powered by
  - Python, Google Colaboratory
  - Numpy, Pandas, Keras, Sklearn
  - Seaborn
### Sources by
  - Kaggle : https://www.kaggle.com/fedesoriano/company-bankruptcy-prediction
### Columns Explanation
  - link : https://docs.google.com/spreadsheets/d/1hKmfA00Vn76y6M_qQpg_ZwRdk32nXVjq5v5pMDa1R7I/edit#gid=0
  - Or <a href = './Column Explanation.xlsx'>click here</a>
  - For Preprocessing, we've deleted several columns because of reasons below:
  1. Columns using certain currency rates(such as Chinese Yen) that lower the compatabilities
  2. Columns showing over-exceptional scatters from boxplot
  3. However, some columns which show critical affects on prediction are remained 
  4. Any unclear columns
## 2. Test Design
### Data Preprocessing
- Data shape : (6819, 71) out of (6819, 96)
- Learning / Test data : 8 / 2
- One-hot Encoding
- Sequence : sklearn's MinMaxScaler
### Modeling
- Activation : Relu, Sigmoid
- Dense layers : 5

## 3. Result & User Interface
We've also provide the service with visualization of result and bankruptcfy prediction of any company that user input the financial index.
User can choose some of columns from whole data sets and predict the accuracies and losses. In addition, they can even customize the visualized plots with selecting two columns.

## Colab Link
- https://colab.research.google.com/github/kdstheace/Project_Financial_Analysis/blob/Daniel/Financial_analysis.ipynb
