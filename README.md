# **Predicting Bankruptcy with Deep Learning Algorithm**
## Colab Link
- https://colab.research.google.com/drive/1vLJzXIfBHCK2W009ygaQWSlKfuC6vsXT?usp=sharing
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
<br>
<br>
# 기업 부도예측 및 재무건전성 관리 프로그램
## 1. 개요
### Intro
  기업의 각종 재무지표를 이용해 부도를 예측하는 어플리케이션입니다. 주요 예측 요소로는 재무제표, 손익계산서 등의 계정을 통해 계산하는 ROA, 회전율, 유동비율부터 시작해, 법인세율 등의 외부 지표까지 고려했습니다. 
### 왜 부도예측을 하는가?
  1. 기업의 관리자는 여러가지 재무적 리스크를 사전에 대응할 수 있다.
  2. 투자자들은 투자하고자 하는 회사의 가치를 명확하게 평가할 수 있고, 본인 투자에 건전성을 높일 수 있다.
  3. 은행의 경우 시행된, 시행될 대출자금에 대해 리스크를 예측하고 대응할 수 있다.
### 기간
  - 2021-04-12 ~ 2021-05-31
### Team
  - 김동수(Daniel)
  - 김민영 (Aphie)
### 사용기술
  - Python, Google Colaboratory
  - Numpy, Pandas, Keras, Sklearn
  - Seaborn
### 데이터 소스
  - Kaggle : https://www.kaggle.com/fedesoriano/company-bankruptcy-prediction
### 데이터 피쳐 설명
  - link : https://docs.google.com/spreadsheets/d/1hKmfA00Vn76y6M_qQpg_ZwRdk32nXVjq5v5pMDa1R7I/edit#gid=0
  - 혹은 <a href = './Column Explanation.xlsx'>링크로 이동</a>
  - 데이터 전처리를 위해, 몇 개의 컬럼을 아래와 같은 기준에 따라 삭제하였습니다:
  1. 특정 화폐를 사용하고 있어 해당 분석의 국가적 호환성을 낮추는 컬럼을 제거했습니다. (예: 중국의 위안화)
  2. BoxPlot을 시각화해보고 예외치가 너무 많은 경우 삭제하였습니다.
  3. 2번 항목에도 불구하고, 결과에 많은 영향을 미치는 컬럼은 유지했습니다. 
  4. 그 외에 국가별 회계기준(IFRS)이 달라 불분명한 계정 등을 삭제했습니다. 
## 2. 테스트 설계
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


