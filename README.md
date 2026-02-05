# First_TitanicDataParctice

1. 프로젝트 개요 (Overview)
주제: 타이타닉 생존자 예측을 통한 데이터 분석 흐름 익히기

학습 목표: 데이터 로드, 전처리, 시각화, 모델링으로 이어지는 파이프라인 이해

2. 데이터 전처리 및 탐색 (EDA)
가설 설정: "성별과 객실 등급이 생존에 가장 큰 영향을 줄 것이다."

작업 내용: - 결측치 처리 (나이를 성별 평균으로 대체)

특성 공학 (가족 수 합치기, 이름에서 호칭 추출)

시각화 (성별/연령대별 생존율 그래프 삽입) - 코랩에서 만든 그래프를 캡처해서 넣으면 훨씬 좋습니다!

3. 머신러닝 모델링
사용 모델: Decision Tree, Random Forest

성능: 최종 정확도 약 82% 달성

주요 변수: AI가 판단한 중요 지표 (Sex, Title, Pclass 등)

4. 느낀 점 (Self-Reflection)
"6개월 만에 다시 시작하며 방학때 배우고 잊어버린 데이터 분석의 흐름을 다시 복습했다."

"단순히 코드를 복사하는 것에 그치지 않고, 가설을 세워 시각화로 확인하는 과정이 흥미로웠다."

"에러 발생 시 제미나이(AI)를 활용해 해결하며 문제 해결 능력을 길렀다."


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
