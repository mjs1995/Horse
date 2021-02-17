# 경진대회_경마분석
- 코드는 01~06번 순입니다

# 기획의도 
- 경마는 사행성 도박이라는 인식이 강해 대중성이 부족
- 최근 렛츠런파크에서 다양한 활동을 통해서 젊은 층 유입이 많아지고 인식 변화에 성공  
- 경마에 대한 흥미로 데이터 분석 연구를 찾아보았으나, 논문 사례가 많지 않음
- 야구, 축구, 농구 등의 스포츠 산업에서는 빅데이터 기반 통계 및 예측이 활발히 이루어지고 있지만 경마 분석은 미비
- 
# 역할 
- selenium과 beautifulsoup을 이용하여 크롤링
- seaborn countplot과 heatmap을 이용한 데이터 시각화 
- spss 카이제곱 검정 

# 크롤링
![제목 없음](https://user-images.githubusercontent.com/47103479/108218764-53bf6b00-7178-11eb-9391-0e618920798c.png)

- 한국 마사회 서울경마_경주 성적 [[Link](http://race.kra.co.kr/raceScore/ScoretableScoreList.do?Act=04&Sub=1&meet=1)]
- 한국 마사회 말혈통 정보 : [[Link](http://studbook.kra.co.kr/studbook.jsp)]
- 경마 크롤링 코드 실행 결과는 크롤링 결과 파일에서 경마_크롤링_실행결과.ipynb에서 볼 수 있습니다

# 데이터 탐색
- seaborn countplot 과 seaborn heatmap 사용
- SPSS_카이제곱 검정법 사용

![제목 없음1](https://user-images.githubusercontent.com/47103479/108218763-5326d480-7178-11eb-9919-f8e78ebcaa6b.png)

# 데이터 전처리
- Excel 과 Python 사용

# 데이터 분석 
- 데이터 탐색과 기존연구조사를 통해 순위와 연관이 있다고 판단되는 변수들로 학습을 진행 
- 학습 변수 – 순위,마번,연령,중량,마체중,단승,연승,주로습도,거리,코너,S1F,G3F,등급,성별,날씨,기수명
- 데이터 불균형 문제를 해결하기 위해 클래스 빈도에 반비례하는 가중치를 두고 학습
- Logistic Regression 과 Random Forest 사용
 
 # 결론 
- 1등, 2등, 3등까지 들어오는 말을 예측한 결과, RF모델이 LR모델보다 좋은 성능을 보임
- 결측치를 제외한 26828개의 데이터를 이용하여 1등, 2등, 3등까지 들어오는 말 예측

![제목 없음2](https://user-images.githubusercontent.com/47103479/108218755-51f5a780-7178-11eb-987f-06b3593c043c.png)

 # 보완점 
 - 데이터 수집을 조금 더 많이 해서 다시 모델링하면 정확도가 높아질 것 같습니다
 - 유의미한 변수(장구현황, 진료사항, 말의 상태)를 찾아 추가하거나 모델 설정을 다르게 하는 등 다양하고 난이도 높은 분석 가능할 것으로 보임
 - 향후 다른 유의미한 변수를 통해 정확도 향상이 가능하며, 구체적인 순위를 예측하는 모델 설정이 가능할 것으로 보임
 
 # 배운점 
 - 독학으로 배웠던 numpy와 pandas의 기본 지식들을 활용하는 프로젝트가 되었으며 크롤링을 통해서 처음으로 python 코드를 짜는데 흥미를 느끼고 시각화 공부를 하게되는 계기가 되었다.

 # 경진대회 결과
 ![image](https://user-images.githubusercontent.com/47103479/70811345-ca403a80-1e08-11ea-8c47-84a225c71477.png)
