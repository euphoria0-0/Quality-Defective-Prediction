# 제품 불량률 예측
Samsung SDS Brightics AI Academy 공모전

## 1. EDA
- Outlier
  - 상위 0.5% 제거

## 2. Model
- Dimension Reduction
  - kernel PCA를 이용하여 k=5의 주성분 생성
  - GridSearchCV를 이용한 최적 파라미터 선정
- xgb, lgbm으로 예측
  - GridSearchCV를 이용한 최적 파라미터 선정
  - 평균으로 앙상블
- Bi-directed LSTM
  - 시계열 특성 이용을 위한 LSTM 모형
  - CallBack
