# 기상청 자외선 지수 예측 모델 개발 (2022.07~2022.08)

## 맡은 역할
### EDA 및 데이터 전처리, 데이터 모델링, 모델 최적화, 보고서 작성

## 상세 활동
### EDA 및 데이터 전처리 과정에서 실제 기상 관측 값이 -999일 경우, 실제 관측이 되지 않은 기상 데이터이기 때문에 보간법을 사용해 전후 데이터의 평균값 적용
### 가시채널과 근적외채널의 경우 정상적인 측정값은 0 이상의 값을 가진다는 것을 멘토링을 통해 확인 후, 태양천정각을 기준으로 90 이상일 경우 야간으로 판단해 음수값을 0으로 대체
### 데이터 모델링 과정에서 Boosting 기반의 트리 모델인 LightGBM 모델과 가중치를 0까지 만들어 회귀 예측을 진행하는 Lasso를 사용해 자외선 지수 예측을 진행
### 각 모델별 MSE와 R^2값을 비교해 모델 선정

## 성과
### 모델 순위 7위, 종합 순위 7위로 공모전 입선

## 배운점 및 느낀점
### 데이터를 처음 받았을 때, 태양천정각, 각종 밴드 등 낯선 변수들이 많이 보였으며, 각 밴드별 이상치가 존재해 이걸 어떻게 처리해야하나 고민을 많이 했습니다.
### 감사하게도 기상청에서 멘토링을 통해 물음에 대한 대답을 들을 수 있었고, 팀원들과 변수들에 대해 찾아보면서 과제에 적합한 데이터 처리 방식을 고민하면서
### 데이터 분석에서 데이터 전처리에 70%의 시간을 쓴다는 것을 몸소 깨달을 수 있었습니다.
### 처음 참여한 대외 공모전임에도 불구하고 7위라는 성적을 거둘 수 있어 팀원들에게 고마움과 동시에 이 공모전을 통해 데이터 탐색/전처리/모델링 등 데이터 분석의 모든 부분에서 많은 것을 배울 수 있었습니다.
