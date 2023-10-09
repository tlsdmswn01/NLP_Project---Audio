# 중국어 성조 교육을 위한 시각자료 및 운율점수 제시
## 프로젝트 개요
<div align="left">
 <img width="100%" src="https://github.com/tlsdmswn01/NLP_Project---Audio/blob/main/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20PPT/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20%EA%B0%9C%EC%9A%94.png?raw=true"/>
</p>
 
 ## 최종 결과물
 <p align='left'>
 <img width="100%" src="https://github.com/tlsdmswn01/NLP_Project---Audio/blob/main/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20PPT/%EC%B5%9C%EC%A2%85%20%EA%B2%B0%EA%B3%BC%EB%AC%BC.png?raw=true"/>

</div>

</p>


## 🗂️프로젝트 소개
본 프로젝트는 성조 시각화 자료와 성조 운율 점수 제시를 통해,  
* 학습자들이 중국어 선생님 없이 자신의 성조를 스스로 피드백하고,
* 학습자들의 자가학습을 도와주는 보조자료 제작에 목표를 둡니다.

--- 

## 📃아이디어 제안 배경
 
 ### 중국어 교육의 필요성 
   - 한국의 수출입액의 1위 국가는 중국이며,
   - 한국과 중국의 무역 비중은 20%정도를 차지할 정도로 여전히 교류가 활발합니다.
   - 이를 통해 한국에서는 여전히 중국어 교육에 대한 수요를 가지고 있을 것이라 예상합니다.
   
 
 ### 중국어 비대면 교육 활성화
 - 중국어 교육의 현황은 크게 코로나 전후로 나눌 수 있는데, 
 - 코로나 이전에는 방문교육이 활성화 되었다면 코로나 이후부터는 ICT를 접목한 이러닝의 규모가 커짐으로써(KDB 미래전략 연구소에 따르면) 중국어 비대면 교육이 더욱더 활성화 되었습니다.  

## 📃중국어 구조와 성조에 대하여

 ### 중국어란?
 - 글자 하나하나가 의미를 가지는 표의문자입니다.
 - 중국어는 성조 언어로, 같은 음의 발화여도 음높이의 변화에 따라 의미가 구별됩니다.
 
### 중국어 성조 교육
- 총 4개의 성으로 구성됩니다. 한자에 따라 성조가 없는 경성도 존재합니다
- 현재 통용되고 있는 성조교육방식으로 오도제 표기법(성조의 상대적인 음의 고저를 5에서 1로 선으로 그린 도표)가 있습니다. 이는 성조 교육 시 음높이와 방향을 직관적으로 제시해 교육에 도움을 줍니다. 
 
<div align="center">
 <img width="50%" src="https://github.com/tlsdmswn01/NLP_Project---Audio/blob/main/%EC%84%B1%EC%A1%B0%20%EC%98%A4%EB%8F%84%ED%91%9C%EC%8B%9C%EB%B2%95.png?raw=true"
/>
</div>

### 성조가 중요한 이유
- 성조는 의미를 변별해주는 역할을 해줘, 성조가 다르면 어법 어휘까지 달라집니다.
- 유창한 중국어를 구사하는데 성조는 필수적인 요소입니다.
- 직관적인 예로, 같은 발음 'shi'여도 모두 서로 다른 의미를 가집니다. 

### 성조교육이 어려운 점 - 성조변화
- 성조언어에서 흔히 나타나는 현상으로, 두 개 이상의 음절을 이어서 읽을 때 성조가 변화하는 현상을 말합니다.
- 실질적인 성조 표기와 실질적인 성조의 운율이 상이합니다. 

<div align="center">
 <img width="50%" src="https://github.com/tlsdmswn01/NLP_Project---Audio/blob/main/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20PPT/%EC%84%B1%EC%A1%B0%20%EB%B3%80%ED%99%94%20%EC%96%B4%EB%A0%A4%EC%9B%80.png?raw=true"
/>
</div>


 ---
 
 ## 기존 서비스와의 차별점
 
 ### 오색중국어
 - 5가지 색깔로 성조 표현
 - 직접 녹음 및 듣기 가능
 - 하지만 알맞지 않은 성조로 중국어를 구사해도 잘했다고 피드백을 줄 정도로 성조 오류에 대한 피드백이 없습니다.

 ### Hello Chinese
 - 내가 녹음한 것에 대해 전체적인 평가 점수 피드백이 있었고,
 - 틀린부분도 빨간색으로 표시해주었습니다.
 - 하지만, 평가 점수에 반영된 것이 성조가 틀린 건지 발음이 틀린 건지 구분이 없었습니다.
 - 또한 어떤 방향으로 개선해야 되는지에 대한 피드백은 없었습니다.

---
 
## 📈성조 시각자료 제작
- 분석목표: 각 Pitch값 즉 음 높낮이 값으로 중국어 성조 시각화하는 것입니다.
- 데이터 : 총 2명의 발화자 음성 데이터
 1. 중국인의 발화음성 - AI hub (노이즈 X)
  2. 한국인의 발화음성 - 직접 녹음 (노이즈 존재, 따로 전처리 진행)
     (한 문장에 대한 -> 연습 이전, 중국어 고급자 , 연습 이후 총 3개의 한국인 음성)
### 성조 시각화 플로우 차트

<p align='center'>
<div align="left">
 <img width="100%" src="https://github.com/tlsdmswn01/NLP_Project---Audio/blob/main/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20PPT/%EC%84%B1%EC%A1%B0%20%EC%8B%9C%EA%B0%81%ED%99%94%20%ED%94%8C%EB%A1%9C%EC%9A%B0%20%EC%B0%A8%ED%8A%B8.png?raw=true"/>  
 
 - 각 발화자 음성데이터에서 Praat을 통해 Pitch 값 추출  
 - 한국인 음성 데이터 노이즈 제거
 - 각 발화자 음성 데이터 배열을 합쳐 전처리 진행(음성 시작, 끝점 통일/ 음절 길이 통일 등)
 - 성조 시각화
</div>
</p>

### 성조 시각화
<p align='left'>
<div align="left">
 <img width="32.5%" height="250" src="https://github.com/tlsdmswn01/NLP_Project---Audio/blob/main/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20PPT/%EC%84%B1%EC%A1%B0%20%EC%8B%9C%EA%B0%81%ED%99%94%202.png?raw=true"/>  
 <img width="32.5%" height="250" src="https://github.com/tlsdmswn01/NLP_Project---Audio/blob/main/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20PPT/%EC%84%B1%EC%A1%B0%20%EC%8B%9C%EA%B0%81%ED%99%94%201.png?raw=true"/> 
  <img width="32.5%" height="250" src="https://github.com/tlsdmswn01/NLP_Project---Audio/blob/main/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20PPT/%EC%84%B1%EC%A1%B0%20%EC%8B%9C%EA%B0%81%ED%99%94%203.png?raw=true"/>  
 
  - 파랑색 점선 : 중국인 발화자 음성(정답)  
  - 빨간색 점선 : 한국인 발화자 음성
  - 연습 이전 음성은 정반 가량 성조가 틀린 것을 확인할 수 있었습니다. 
  - 중국어 고급자 음성은 정답과 매우 유사하게 성조를 말했음을 확인할 수 있습니다. 
  - 연습(프로젝트 기간 발화문장 연습) 이후 음성 선의 패턴은  연습 이전 음성에 비해 정답 선의 패턴과 조금 더 유사해짐을 확인할 수 있습니다.
</div>
</p>

### 성조 시각화 기대효과  
<p align='left'>
<div align="left">
 <img width="100%" src="https://github.com/tlsdmswn01/NLP_Project---Audio/blob/main/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20PPT/%EC%84%B1%EC%A1%B0%20%EC%8B%9C%EA%B0%81%ED%99%94%20%EA%B8%B0%EB%8C%80%ED%9A%A8%EA%B3%BC.png?raw=true"/>  

 - 한국인들이 가장 어려워하는 성조 : 2성과 3성
 - 연습 이후 음성을 보아도 여전히 3성을 틀린 것을 확인 할 수 있습니다.
 - 실제 발화자 인터뷰 내용 : 시각화 자료를 보기 전까지 어떤 부분에서 성조를 잘 못 말했는지 인지하지 못했는데, 시각화를 통해 정확히 알게 되었다고 합니다.
 - 이렇듯 성조 시각화 자료는 성조를 가시적으로 보여주면서 선생님의 피드백 없이도 스스로 피드백하며 자가학습을 할 수 있게 도와주는 보조역할을 합니다.
 </div>
</p>

## 🖥️ 운율의 유창성 평가 점수  
분석목표: 중국어의 성조 유창성 점수를 예측하는 회귀모델을 만드는 것입니다.
데이터 : 한국인의 중국어 발화 음성 데이터 - AI hub (노이즈 없음)  
타겟 데이터 : 전문 평가자의 성조 평가 점수

### 데이터 분석 및 모델링 플로우 차트  
<p align='left'>
<div align="left">
 <img width="100%" src="https://github.com/tlsdmswn01/NLP_Project---Audio/blob/main/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20PPT/%EB%8D%B0%EC%9D%B4%ED%84%B0%20%EB%B6%84%EC%84%9D%20%EB%B0%8F%20%EB%AA%A8%EB%8D%B8%EB%A7%81%20%ED%94%8C%EB%A1%9C%EC%9A%B0%20%EC%B0%A8%ED%8A%B8.png?raw=true"/>  
 
 - 음성 데이터 전처리 후 음성정보 중 하나인 크로마그램을 추출하였습니다. 
 - 이후 패딩을 진행하면서 최대길이 설정에 따라 모델 성능이 달라질 수 있다고 판단하여
 데이터의 벡터길이를 고려해 600,500,550이라는 3개의 패딩데이터를 저장하였습니다.  
 - 다양한 모델들로 데이터 실험 및 성능평가를 통해 CNN+LSTM과 LSTM+Attention모델을 보다 집중적으로 모델링 하여, 성능 평가 및 테스트를 진행하였습니다. 
  </div>
</p>

 ### 분석 및 모델링 과정 
 #### 음성 데이터 전처리
 
 문제인식 : 음성 데이터 길이가 모두 달랐습니다.

 - 짤게는 3초, 길게는 70초까지 음성 데이터 길이가 다양했습니다.
 - 데이터 패딩시 음성을 자르게 되면 몇몇 음성은 초반 음성에 대한 점수로 모델이 학습할 수 있어 이로 인한 왜곡이 우려되어 10초라는 특정 시간대 이후로의 데이터는 삭제했습니다.
   (10초 이전 : 데이터가 90%이상 분포하고 있는 구간 )

#### 음성 정보 채택 및 추출

**다양한 음성 정보**  

- Mel Spectogram : 사람의 청각인지를 반영하기 위한 스펙초그램에 Mel sclae를 적용한 특징 추출 기법
  (Mel Scale : 실제 주파수 정보를 인간의 청각 구조를 반영하여 수학적으로 변환하기 위한 방법
  예- 돌고래 소리의 주파수가 매우 높아 사람이 듣지 못하는 개념을 스펙토그램에 반영한 것)
- MFCC(Mel-Frequency Cepstral Coefficients) : 사람의 청각 구조와 음색의 차이를 반영한 음성 데이터 특징 추출 기법
  (Ceptral 분석 : 배음의 구조를 파악해 음색의 차이를 구별하는 분석법 - 악기나 성대의 구조 차이에의해 발생)
- 크로마그램 : 인간 청각이 옥타브 차이가 나는 주파수를 가진 두 음을 유사음으로 인지한다는 음악이론에 기반
  (12개의 Bin으로 특징이 추출된다. - 도,도샵,레, 레샵 ~ 시 12개 음계값)

**크로마그램 채택** 

- 중국어 성조는 음절에 해당하는 소리의 높이 변동
- 중국어 성조 중 2성은 미에서 솔까지 올리면 2성이 됩니다. 이와 같이 성조는 12개의 음계와 매우 밀접한 관련이 있다고 판단해 음성데이터에서 크로마그램을 추출해 분석했습니다.

**크로마그램 추출 후 패딩 + 시각화**  

패딩

<p align='left'>
<div align="left">
 <img width="100%" src="https://github.com/tlsdmswn01/NLP_Project---Audio/blob/main/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20PPT/%ED%81%AC%EB%A1%9C%EB%A7%88%EA%B7%B8%EB%9E%A8%20%EC%B6%94%EC%B6%9C%20%ED%9B%84%20%ED%8C%A8%EB%94%A9.png?raw=true"/>  
 </div>
</p>

 시각화  
 <p align='left'>
<div align="left">
 <img width="100%" src="https://github.com/tlsdmswn01/NLP_Project---Audio/blob/main/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20PPT/%ED%81%AC%EB%A1%9C%EB%A7%88%EA%B7%B8%EB%9E%A8%20%EC%8B%9C%EA%B0%81%ED%99%94.png?raw=true"/>  

 - 크로마그램 시각자료를 보면 빨간색이 진한, 즉 크로마그램 특징이 투렷하게 추출된 음성 데이터의 점수가 높음을 확인할 수 있고, 점수가 낮을수록 크로마그램 특징이 뚜렷하지 않음을 확인할 수 있습니다.

 </div>
</p>

#### 모델링 과정 소개 및 결과
**DNN** 
결과 : 오버피팅 발생 - 문제의 복잡도에 비해 모델이 너무 단순하기 때문이라 판단했습니다.

**CNN+BILSTM**
 <p align='left'>
<div align="left">
 <img width="100%" src="https://github.com/tlsdmswn01/NLP_Project---Audio/blob/main/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20PPT/CNN+LSTM.png?raw=true"/>  
  <p align='left'>
<div align="left">
 <img width="100%" src="https://github.com/tlsdmswn01/NLP_Project---Audio/blob/main/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20PPT/CNN+LSTM%20%EA%B5%AC%EC%84%B1%EC%A0%95%EB%B3%B4.png?raw=true"/>  
 
 - 윤상혁 외 2명(2021), CNN-LSTM 모델 기반 음성 감정 인식, ACK 2021 학술발표대회 논문집 (28권 2호) 을 참고해 모델 작성하였습니다.

 <p align='left'>
<div align="left">
 <img width="100%" src="https://github.com/tlsdmswn01/NLP_Project---Audio/blob/main/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20PPT/CNN+LSTM%20%EC%84%B1%EB%8A%A5%EA%B2%B0%EA%B3%BC.png?raw=true"/>  

 - 각기 다른 패딩값을 가진 3개의 데이터로 실험을 해보았지만 큰 차이는 없었습니다.
 - 그 중에 패딩 최대길이가 500일때가 가장 MSE값이 낮아 해당 데이터로 분석을 진행하게 되었습니다.
 - 성능지표 그래프를 통해 Loss값과 MSE값 모두 한 값으로 수렴하면서 매우 낮아짐을 확인할 수 있습니다.
 </div>
</p>
  
**모델 성능 비교**  
 <p align='left'>
<div align="left">
 <img width="100%" src="https://github.com/tlsdmswn01/NLP_Project---Audio/blob/main/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20PPT/%EB%AA%A8%EB%8D%B8%20%ED%85%8C%EC%8A%A4%ED%8A%B8%20%EC%84%B1%EB%8A%A5%20%EB%B9%84%EA%B5%90.png?raw=true"/>  

 - CNN-BILSTM과 LSTM+Attention 모델의 성능지표값이 가장 좋았고, 근소하게 LSTM+ATTention의 Mse값이 더 낮음을 확인할 수 있었습니다.
 - 하지만 저희 서비스의 목적에 조금 더 부합한 모델이 CNN-BILSTM이라고 생각하고 이를 채택해 실제 데이터로 테스트 해보았습니다.
 </div>
</p>

**CNN-BILSM 실제 데이터 예측값**  
<p align='left'>
<div align="left">
 <img width="100%" src="https://github.com/tlsdmswn01/NLP_Project---Audio/blob/main/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20PPT/%EB%AA%A8%EB%8D%B8%20%ED%85%8C%EC%8A%A4%ED%8A%B8%20%EC%84%B1%EB%8A%A5%20%EB%B9%84%EA%B5%90.png?raw=true"/>

**리츠 주가등락 예측모형에 대한 모델 설계 과정은 다음과 같습니다.**
1. 수집 및 전처리 
2. 변수 선정
3. 모델링
4. 평가 검증 및 성능 측정

### 1. 수집 및 전처리
**데이터 수집**

2019년 1월 ~ 2022년 12월을 기준으로 하여 데이터를 수집하였습니다.
- 각 리츠 일별 / 투자자별 거래 데이터를 한국 주식 거래소(KRX)에서 수집하였습니다.
- 각 리츠 분기별 재무상태표 데이터와 일별 / 월별 거시경제 데이터는 FnGuide를 통해 수집하였습니다.
- 일별 / 부동산 유형별 뉴스 데이터는 빅카인즈를 통해 수집하였습니다.

**파생변수 생성**
- 투자자별 리츠 상품 거래데이터를 통해 "정보비대칭 변수"(기관, 외국인별 순매수도 금액, 체결강도)를 파생변수로 추가하였습니다.
- 일별 주식 거래 데이터를 활용하여 "테크니컬 변수"(SMA20, MACD, ATR, TR, RSI, SLOW_K)를 파생변수로 추가하였습니다.
- 부동산 뉴스테이터를 활용하여 부동산 유형별로 감성 분석을 진행하고 개별리츠의 투자 자산 비중에 맞춰 가중평균한 "부동산 뉴스 심리지수 변수"를 파생변수로 추가하였습니다.


### 2. 변수 선정
**변수 유의성 확인**
앞에서 추출한 후보변수를 고전적 회귀모형 가정(CLM)을 기준으로 변수의 유의성을 확인하였습니다.

- 정규성 검정
정규성 검정 결과 대부분 변수가 정규성을 만족하지 않는다는 것을 확인하였습니다. CLM가정을 중 하나인 정규성을 만족시키기 위해서 데이터 분포의 양 끝단 데이터를 0.5%를 끝단 값으로 대치하는 윈저라이징 기법을 통해 정규성을 확보하고자 하였습니다.

<p align='center'>
<br>
<div align="center">
 <img width="70%" src="https://github.com/ssongssong00/ShinhanAI/assets/96776691/f85a0ab5-1b28-400e-8281-6ccb37b53488"/>

</div>
</p>

 - 다중공선성 확인
상관관계를 파악하기 위해 히트맵으로 변수간 상관의 여부를 파악하고 VIF계수로 그 상관의 정도를 확인하였습니다. 다중공선성이 너무 높은 변수들은 제거하고 모델링을 진행하였습니다.

<p align='center'>
<br>
<div align="center">
 <img width="70%" src="https://github.com/ssongssong00/ShinhanAI/assets/96776691/9f8fd758-c54d-4dcd-9115-ea1da9130952"/>

</div>
</p>

이를 통해 모델 학습에 사용 될 최종 변수들을 선정하고 하나의 데이터프레임으로 합쳐 최종 데이터셋을 생성하였습니다. 

<p align='center'>
<br>
<div align="center">
 <img width="70%" src="https://github.com/ssongssong00/ShinhanAI/assets/96776691/8fb22b82-3870-4839-b7ad-74eed17485aa"/>

</div>
</p>

종속변수는 한달 뒤 주가등락 여부를 확인하는 것으로 상승, 보합 및 하락으로 이진변수로 구성하였습니다. 종속 변수 분포를 확인한 결과, 1:1 비율로 데이터가 균형있게 존재함을 파악하였습니다. 

### 3. 모델링
**알고리즘 채택**
종속변수 주가 등락을 예측하기 위해 분류 알고리즘을 사용하였습니다. 로지스틱 회귀모형, 트리계열의 XGBoost, CatBoost, 기타 분류 모델인 SVM, Naive Bayes 분류 모형 등의 알고리즘을 사용하여 모델링을 진행한 결과, 트리 기반의 XGBoost 알고리즘이 가장 좋은 성능을 보여주었기 때문에 XGBoost를 채택하였습니다.

### 4. 평가 검증 및 성능 측정
**성능 평가 지표**
모형을 평가함에 있어 분류 모델에서 주로 사용되는 Confusion Matrix를 기반으로 Accuracy, Precision, Recall, F1 score를 측정하였습니다. 
<p align='center'>
<br>
<div align="center">
 <img width="70%" src="https://github.com/ssongssong00/ShinhanAI/assets/96776691/fced78cf-c4c2-491a-a6a5-a39ff006983c"/>

</div>
</p>

**피쳐 중요도**
트리계열 알고리즘에서 어떤 변수가 가장 큰 영향을 미쳤는지 파악하기 위해 학습시킨 모형에서 피쳐중요도를 확인하였습니다. 1달 뒤의 주가등락을 예측하였기 때문에 중장기 주가 등락을 예측할 때 중요한 변수들임을 파악할 수 있습니다. 
<p align='center'>
<br>
<div align="center">
 <img width="70%" src="https://github.com/ssongssong00/ShinhanAI/assets/96776691/2c40566a-2006-495b-937b-11c0faa81d0a"/>

</div>
</p>

---

## 📔대시보드 설명
### **SAR Dashboard** ###

### 1. Home 대시보드
대시보드를 처음 실행 시, 사용자는 메인화면에 접속하게 됩니다. 

<p align='center'>
<br>
<div align="center">
 <img width="70%" src="https://github.com/ssongssong00/ShinhanAI/assets/100076851/3fd3e08a-669c-4e54-9d85-8015d57ed9ee"/>

</div>
</p>
 
- **주가등락예층모형 기반 기간별 리츠 추천**을 통해 등락 여부, 배당수익률, 기초자산 건전성을 비교하며 안전하고 전망이 좋은 리츠 상품을 한눈에 파악 가능
- **부동산 시장에 주로 영향을 미치는 거시변수**인 주택 매매지수/국고채 3년/종합주가지수/건설업종지수의 추이를 한눈에 확인하여 시장상황에 적합한 투자 가능
- **섹터별 부동산 뉴스기사 감성분석**을 통해 부동산 시장에 대한 의견 및 평가를 요약된 정보로 부동산 섹터별 확인 가능 
- **부동산 뉴스기사 및 키워드 제공**을 통해 부동산 시장에 대한 정보를 키워드로 한눈에 파악 가능


### 2. 개별 리츠 대시보드
메인화면에서 '개별 리츠(ex.신한알파리츠)'를 클릭 시, '개별 리츠' 대시보드로 이동하게 됩니다.

<p align='center'>
<br>
<div align="center">
 <img width="70%" src="https://github.com/ssongssong00/ShinhanAI/assets/100076851/deeb88a7-0609-484a-9728-271bc1310229"/>

</div>
</p>

- 현재 종가, 등락률 등과 같은 보유한 자산의 섹터별 구성 비중 정보인 **리츠의 자산 구성**  제공
- **애널리스트 투자의견**을 통해 전문가의 투자의견과 자신의 투자 의견을 종합한 합리적인 투자 가능
- FFO,P/FFO 등 **회계 요약 정보**를 통해 리츠 투자시 고려할 회계 정보를 투자자들이 이해하기 쉽게 설명과 함께 요약 제공
- 위치 기반, 임대 현황, 추이와 같은 **기초자산정보**를 참고하여 주변 상권에 대한 전망을 파악할 수 있으며 임대 동형 확인 가능

### 3. 리츠 회사 회계 정보 대시보드
'개별 리츠' 대시보드에서 '회계 정보 상세보기'를 클릭 시, '회계 정보' 대시보드로 이동하게 됩니다.

<p align='center'>
<br>
<div align="center">
 <img width="70%" src="https://github.com/ssongssong00/ShinhanAI/assets/100076851/efa74c57-baf7-4ec8-9e32-95400cf06a3c"/>

</div>
</p>

- 리츠가 약속한 배당을 잘 주고 있는지, 추후 배당일정은 어떻게 되는지 등의 **배당내역** 제공
- **투자보고서와 월간보고서**를 링크와 pdf를 통해 제공하여 분산되어 있는 리츠 정보 제공
- 해당 리츠가 현재 얼마나 돈을 많이 벌고 있는지 확인 가능한 **FFO(Funds For Opperation)** 제공
- 현재 발생하는 임대료에서 영업 경비를 제외한 **NOI(Net Opperation Income)** 제공
- 회계정보에서 합계로만 제공되는 **Cap Rate**와 **건물별 Cap Rate**를 제공하여 실질적인 투자 수익률 확인 가능
- **자산, 부채, 자본, 총계** 정보 제공

### 3-1. 회계 용어 설명
낯선 회계 용어를 만나면 지표 옆의 물음표 버튼을 통해 SAR의 쉬운 **회계 용어 설명** 제공

<p align='center'>
<br>
<div align="center">
 <img width="70%" src="https://github.com/ssongssong00/ShinhanAI/assets/100076851/713d21d1-b88f-49f1-a38f-e71eb258b718"/>

</div>
</p>




### 4. 기초자산정보 대시보드
'개별 리츠' 대시보드에서 '기초자산정보 상세보기'를 클릭 시, '기초자산 정보' 대시보드로 이동하게 됩니다.

<p align='center'>
<br>
<div align="center">
 <img width="70%" src="https://github.com/ssongssong00/ShinhanAI/assets/100076851/8c4c8f7b-c942-41b7-a591-2e7e58928c77"/>

</div>
</p>

- 자산의 임차인, 사용 목적, 기업 분류와 같은 **임차인 정보** 제공
- 임대료에 영향을 미치는 요인들을 제공하고 지도에 표시할 선택 가능한 **지표** 제공
- 선택 **지표 상세정보**, 자산과 리츠의 평균 평점 정보를 제공
- **기초자산 위치 정보**를 통해 자산의 위치, 선택 지표 정보를 지도에 제공하며 검색 기능을 통해 리츠의 자산 외의 지역도 검색 및 탐색 가능
- 자산이 속해 있는 **지역 뉴스**를 통해 주변 상권 및 자산의 가치 동향 파악 가능

## 📈프로젝트 기대효과

- 리츠 시장의 정보 비대칭성 해소

일반 투자자들은 분산된 리츠의 정보들을 SAR 대시보드를 통해 한눈에 쉽게 파악 가능합니다. 이를 통해 리츠 시장에 대한 정보 비대칭성을 해소하고, 투자자들은 리츠기업의 재정상태, 기초자산의 건전성등을 쉽게 파악해 안전한 투자가 가능해집니다.   

- 리츠 시장의 진입장벽 완화

SAR 대시보드는 투자자들이 알기 어려운 회계용어 및 리츠추천 기능의 원리 등의 정보들에 대해 이해하기 쉬운 설명과 함께 제공됩니다. 각 용어와 원리에 대한 쉬운 설명으로 일반 투자자들의 리츠 투자에 대한 진입장벽이 낮아지고 더 나아가 고령 투자자의 안전한 리츠 투자가 가능해져 퇴직연금 시장의 리츠 투자가 활성화 될 것으로 기대됩니다.  

- 신한투자증권 HTS시스템과 SAR의 연동

SAR이 활성화 되어 신한투자증권에 개설된 연금계좌가 연동되면 투자자들의 더욱 안전한 리츠투자가 가능할 것으로 기대됩니다. 이는 신한투자증권의 연금 운용 활성화 기능으로써 신한투자증권의 IRP계좌를 계설하는 고객들이 많아지고, 더 나아가 리츠 매매가 활성화 될 것으로 예상됩니다. 

- 신한 AI MWS와의 시너지

SAR이 활성화 되면 앞으로 신한 AI, 마켓워닝시스템 'MWS'와의 연계가 가능할 것으로 기대됩니다. 시장에 영향을 많이 받는 부동산의 특성을 고려해 '마켓워닝시스템'을 활용해 리츠 시장에 유연하게 대처하며 적합한 리츠 상품 추천까지 가능한 시스템으로 확장할 것으로 예상됩니다. 


---
