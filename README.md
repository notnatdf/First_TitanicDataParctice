# First_TitanicDataParctice

방학 때 배웠던 빅데이터 분석의 흐름을 다시 복습하고 실습해본 기록입니다. 
데이터 로드부터 전처리, 시각화, 그리고 간단한 머신러닝 모델링까지의 전체 파이프라인을 익히는 데 집중했습니다.

## 🛠 실습 과정 (Workflow)

1. **데이터 로드 및 탐색**: Pandas를 활용해 Kaggle의 Titanic 데이터를 불러오고 기초 통계를 확인했습니다.
2. **데이터 전처리 (Pre-processing)**:
   - `Age` 결측치를 성별 평균값으로 대체
   - `Sex`, `Embarked` 등 범주형 데이터를 수치형으로 변환
   - `FamilySize` (가족 수 합치기), `Title` (호칭 추출) 등 새로운 특성(Feature) 생성
3. **데이터 시각화 (EDA)**:
   - 성별, 객실 등급, 연령대별 생존율을 Seaborn과 Matplotlib으로 시각화하여 데이터의 패턴 분석
4. **머신러닝 모델링**:
   - `Decision Tree`와 `Random Forest` 모델을 사용하여 생존자 예측
   - 데이터 전처리 후 모델의 정확도가 향상되는 과정을 확인

## 💡 느낀 점 (Self-Reflection)

- 6개월 만에 다시 데이터를 다루면서 분석의 전체적인 흐름(데이터로드-전처리-시각화-모델링)을 체계적으로 정리할 수 있었습니다.
- 에러가 발생했을 때 Google Colab의 Gemini를 활용하여 해결하는 과정을 거쳤습니다.
- 단순히 코드를 복사하는 것이 아니라, 가설을 세우고 이를 시각화로 직접 검증해보는 과정의 중요성을 배웠습니다.
- 1학년 1학기 여름방학때 배운 빅데이터 교육에서 사용했던 타이타닉 시나리오를 다시금 스스로 해보면서 2학기에 파이썬을 배웠던걸 토대로 다시금 기억을 떠올리면서 해봤습니다.
- 기존에 웹 개발 풀스택 공부를 하다가 빅데이터에 흥미를 느껴서 방학때 수강을 해보고 이후로 빅데이터에도 관심이 생겨서 배웠던걸 좀 더 업그레이드 해본다는 생각으로 했습니다.


객실 등급(Pclass)별 생존자 수 시각화
<img width="571" height="455" alt="image" src="https://github.com/user-attachments/assets/1640b118-5989-45b5-a2b7-ff79989cb968" />

가족 수에 따른 생존율 시각화
<img width="691" height="470" alt="image" src="https://github.com/user-attachments/assets/592fe0a1-19d3-4d56-962d-3b2bf2cd0718" />

호칭별 생존율 시각화
<img width="846" height="470" alt="image" src="https://github.com/user-attachments/assets/00bc8992-942e-45e7-8b01-c5acaf017b32" />

연령대별 생존율 평균 시각화
<img width="846" height="549" alt="image" src="https://github.com/user-attachments/assets/6a3838bc-b618-4083-a4a2-079059ff4bb5" />

연령대별로 나누고, 그 안에서 성별(Sex)로 한 번 더 분리한 생존율 시각화
<img width="1001" height="547" alt="image" src="https://github.com/user-attachments/assets/8b7f0722-494e-4897-9043-52e1ef7bba8b" />

히트맵
<img width="776" height="682" alt="image" src="https://github.com/user-attachments/assets/0b2bd525-6f44-47ec-a8b7-01ff3d96c955" />

중요도 추출
<img width="614" height="435" alt="image" src="https://github.com/user-attachments/assets/aba240e5-9234-44bd-939c-acc55e76ded8" />

랜덤포레스트 모델링 결과값
변수를 추가한 최종 모델 정확도: 83.24%
