# :telephone: 통신사 고객 이탈 예측 프로젝트

## :busts_in_silhouette: 팀원 소개
### - 팀명: 아이돌이 될 뻔한 무한상사
|<img src="https://github.com/user-attachments/assets/1852fb34-740b-425f-ac4d-43ef3f31cd1b" width="250"  height="180"/>|<img src="https://github.com/user-attachments/assets/d4ba50e8-38e1-45c4-80b9-a029ee882eba" width="250"  height="180"/>|<img src="https://github.com/user-attachments/assets/d03aad58-532c-4bcc-bc4d-4710d73ee484" width="250" height="180"/>|<img src="https://github.com/user-attachments/assets/200b29be-f529-4746-8c07-fc0031a275bb" width="250" height="180"/>| 
|:--------:|:--------:|:--------:|:--------:|
| 이지복 <br> [@Bokfortune](https://github.com/Bokfortune)  | 노명구 <br>[@nmmm9](https://github.com/nmmm9)| 최문영 <br> [@myoung112](https://github.com/myoung112) | 박진양 <br> [@ParkJinyang-hello](https://github.com/ParkJinyang-hello) |
<br>

## 📜 프로젝트 개요
## 📅 개발 기간  
### 2025.04.17 ~ 2025.04.18
## 프로젝트 필요성
### 📌 고객 유지 비용 보다 큰 신규 고객 유치 비용
-  신규 고객 확보 비용은 광고, 프로모션, 제휴 마케팅 등 많은 비용이 드는 반면, 기존 고객을 유지하는 비용은 훨씬 낮음
-  이탈 가능성이 높은 고객을 사전에 파악하고 선제 대응하는 것이 훨씬 효율적임

### 📌 맞춤형 리텐션 마케팅 가능성 확보
-  이탈 가능성이 높은 고객군을 타겟팅하여 개인화된 리텐션 마케팅을 가능하게 함
-  고객 만족도 상승과 브랜드 충성도 증가로 이어짐

### 📌 고객 생애가치(LTV, Lifetime Value) 극대화
-  장기 고객일수록 ARPU(가입자 평균 매출)도 높고, 부가서비스 사용률도 높음
-  고객 이탈을 줄이면 고객 생애 가치가 증가하고, 이는 곧 장기 수익 증가로 이어짐


### 📌 정체된 시장에서의 경쟁력 확보
-  이미 포화 상태인 통신 시장에서 시장 점유율을 지키기 위해 기존 고객의 이탈을 줄이는 것이 가장 적절함
<br>

# 🎯프로젝트 목표
### 통신사 이탈 고위험성 고객 사전 식별, 높은 고객 유지율, 시장 경쟁력 극대화를 위한 고객 이탈 예측 모델 개발 및 시각화

<br>

## 🛠️기술 스택
|    분야    |사용기술|
|:------:|:------:|
|    언어   |![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python&logoColor=white)|
|데이터분석   |![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=Pandas&logoColor=white)  ![Numpy](https://img.shields.io/badge/Numpy-013243?style=for-the-badge&logo=numpy&logoColor=white)|
|시각화   |![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=matplotlib&logoColor=white) ![Seaborn](https://img.shields.io/badge/Seaborn-43B6C7?style=for-the-badge&logo=seaborn&logoColor=white) ![SHAP](https://img.shields.io/badge/SHAP-5A20CB?style=for-the-badge&logoColor=white)
|    모델 설계    |![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white) ![Random Forest](https://img.shields.io/badge/Random%20Forest-228B22?style=for-the-badge&logoColor=white) ![Logistic Regression](https://img.shields.io/badge/Logistic%20Regression-1E90FF?style=for-the-badge&logoColor=white) ![SVM](https://img.shields.io/badge/SVM-800080?style=for-the-badge&logoColor=white) ![LightGBM](https://img.shields.io/badge/LightGBM-9ACD32?style=for-the-badge&logoColor=white) ![Gradient Boosting](https://img.shields.io/badge/Gradient%20Boosting-F5B041?style=for-the-badge&logoColor=white) ![XGBoost](https://img.shields.io/badge/XGBoost-FF6600?style=for-the-badge&logo=xgboost&logoColor=white)|
|화면구현    |![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=Streamlit&logoColor=white)|

<br> 

-------------------
## 데이터셋 소개
IBM이 제공하는 통신사 고객 이탈 데이터셋을 사용  
https://www.kaggle.com/datasets/blastchar/telco-customer-churn
- 데이터 수 : 7043명
  - 컬럼
    -  `customerID`: 고객의 성별 (남성/여성)
    -  `gender`: 고객의 성별 (남성/여성)
    -  `SeniorCitizen`: 고령자 여부 (1 = 예, 0 = 아니오)
    -  `Partner`: 배우자 유무 (예/아니오)
    -  `Dependents`: 부양 가족 유무 (예/아니오)
    -  `tenure`: 고객이 회사에 가입한 개월 수
    -  `PhoneService`: 전화 서비스 이용 여부 (예/아니오)
    -  `MultipleLines`: 다중 회선 이용 여부 (예/아니오/전화 서비스 없음)
    -  `InternetService`: 인터넷 서비스 종류 (DSL/광섬유/인터넷 서비스 없음)
    -  `OnlineSecurity`: 온라인 보안 서비스 이용 여부 (예/아니오)
    -  `OnlineBackup`: 온라인 백업 서비스 이용 여부 (예/아니오)
    -  `DeviceProtection`: 기기 보호 서비스 이용 여부 (예/아니오)
    -  `TechSupport`: 기술 지원 서비스 이용 여부 (예/아니오)
    -  `StreamingTV`: 스트리밍 TV 이용 여부 (예/아니오)
    -  `StreamingMovies`: 영화 스트리밍 서비스 이용 여부 (예/아니오)
    -  `Contract`: 계약 유형 (월별 계약/1년 계약/2년 계약)
    -  `PaperlessBilling`: 종이사용없는 청구서 여부 (예/아니오)
    -  `PaymentMethod`: 결제 방식 (전자 수표/우편 수표/계좌 이체/신용카드)
    -  `MonthlyCharges`: 월별 서비스 요금
    -  `TotalCharges`: 고객이 누적하여 지불한 총 요금
  - target 컬럼
     - `Churn`: 고객 이탈 여부 (예/아니오)
    
## 📊EDA
### 고객 이탈 여부     

<img src="https://github.com/user-attachments/assets/d4f8a461-5fbf-45e6-b9f0-a8f5c3ac3ca3" width="850">   

-  아

### 성별에 따른 이탈 여부     

<img src="https://github.com/user-attachments/assets/ef7ceb86-e563-489f-9de6-71cc7c19046a" width="850" height="450">

-  1

### 고령자 이탈 여부     

<img src="https://github.com/user-attachments/assets/1642eabd-39b8-48e2-96bc-6511f3bcc869" width="850" height="450">  

-  1

### 이용기간 별 이탈 여부   

<img src="https://github.com/user-attachments/assets/5bb420b7-e7d5-40e5-ad86-b3b7dc020961" width="850">   

-  1

### 월별 요금 별 이탈 여부    

<img src="https://github.com/user-attachments/assets/be2f2c78-cf68-41ce-b2ec-fa634cb2a88b" width="850">   

- 1

### 결제 방법 별 이탈 여부    

<img src="https://github.com/user-attachments/assets/e800c8f3-ef5f-4759-af6a-65bcf2691614" width="850" height="450">   

- 1 

### 인터넷 서비스 별 이탈 여부    

<img src="https://github.com/user-attachments/assets/cf116353-4996-4752-bb88-51d800ffa906" width="850" height="450">   

- 1

### 계약 형태 별 이탈 여부    

<img src="https://github.com/user-attachments/assets/56c1a163-5664-4bfb-9697-377e6ccdaab9" width="850">   

- 1

### 지불 방법 별 이탈 여부     

<img src="https://github.com/user-attachments/assets/a3df36e8-34d7-48b0-929d-ecf3d415cff7" width="850">   

- 1

### 부가 서비스 별 이탈 여부    

<img src="https://github.com/user-attachments/assets/c12a0cb0-7a2c-4a73-a49b-b2063ba12af6" width="850" height="350">  

- 1

## 데이터 전처리 
- 결측치 및 중복값 제거
- 사용하지 않는 feature 제거 (`Customer_ID`)
- Churn의 컬럼 값 1 / 0으로 변환
- TotalCharges 컬럼에서 `NaN` 값 제거 및 데이터 타입 변환(float)

## 특성 스케일링 및 데이터 불균형 처리
- StandardScaler를 이용한 특성 스케일링
- SMOTE 적용

## 사용 모델
- 전통 머신러닝 모델
  - Logistic Regression
  - Random Forest
  - LightGBM
  - SVM
  - XGBoost
  - Gradient Boosting
<br>

 - MoonyungStacking : StackingClassifier를 사용하여 앙상블 모델 구성
   - XGBClassifier
     - n_estimators=90
     - max_depth=5
     - learning_rate=0.08
     - subsample=0.9
     - colsample_bytree=0.7
     - eval_metric="logloss"
     - use_label_encoder=False
     - random_state=42  

   - RandomForestClassifier
      - n_estimators=100
      - max_depth=8
      - random_state=42
        
   - LogisticRegression
     - max_iter=1000

   - StackingClassifier(
     - estimators=[("rf", rf), ("xgb", xgb)]
     - final_estimator=lr
     - passthrough=True

## 모델 평가 및 결과
- 모델별 Accuracy, Recall, Precision, f1-score 비교
![image](https://github.com/user-attachments/assets/9643fca8-7916-4b7a-a183-0c41450be2ad)
- ROC-Curve
![newplot (2)](https://github.com/user-attachments/assets/beae7185-77de-4c8a-9791-3e6d1077bd53)
- 모델 종합 비교
![newplot (1)](https://github.com/user-attachments/assets/9706f6ee-4ae7-46a6-987f-991368530622)

성능 결과 분석
RandomForest 모델이 정확도 82.01%, F1 점수 82.18%로 가장 높은 성능을 보였습니다.
트리 기반 모델(RandomForest, LightGBM, XGBoost)이 로지스틱 회귀보다 우수한 성능을 보였습니다.
GridSearchCV를 통한 하이퍼파라미터 최적화가 모델 성능 향상에 크게 기여했습니다.
모든 모델이 77% 이상의 정확도를 보이며 안정적인 성능을 나타냈습니다.


### 특성 중요도(Feature Importance) 분석 (상위 5개)
<명구님 그림>
Last_Login_days (마지막 로그인 이후 경과 일수)
Watch_Time_Hours (시청 시간)
satisfaction_score (만족도 점수)
daily_watch_hours (일일 시청 시간)
Age (나이)


## 결론
- 최종 결론

- 한계점
AutoML을 통해 구현해 봤을때 
- 개선 방안
  
## 기대효과 및 활용방안
-

### 💭 한줄 회고
- 이지복 : 
- 노명구 : 
- 최문영 : 
- 박진양 :



