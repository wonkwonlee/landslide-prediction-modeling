# 날씨 빅데이터 콘테스트 - 공공협력형
> 날씨, 임상도, 토양도 데이터를 기반으로 한 경상도 지역의 산사태 예측 

2021년 4월 26일 ~ 8월 25일까지 진행되는 기상청 주최 [날씨 빅데이터 콘테스트](https://bd.kma.go.kr/contest/main.do) 공공협력 분야

멋쟁이사자처럼 K-Digital Training의 마지막 프로젝트로 4인 1조로 참여

Collaborated with [Bill Kim](https://github.com/billkim418), [Heewon Kwak](https://github.com/HeewonKwak), [Titus Choi](https://github.com/TitusChoi)

기상에 따른 산림재해 예측 및 산사태 예측 기술 개발, 개선 프로젝트

129팀 중 최종 6위 수상

[최종 공모안](submission.pdf)
 
## 활용 데이터
* 산사태 발생 이력
  + 2011년 7월부터 2019년 10월까지의 경상북도, 경상남도 내 산사태 발생 이력
* 산림 공간 정보
  + 경상북도, 경상남도 임상도 및 토양도
* 행정 구역 경계
  + 경상북도, 경상남도 읍, 면, 동 단위의 지역 구분
* [기상청 날씨 데이터](https://data.kma.go.kr)
  + 기상 자료 개방 포털의 종관기상관측(ASOS) 날씨 데이터


## Data
- data: 날씨 빅데이터 콘테스트에서 제공되는 기존 데이터 및 크롤링을 통해 구한 날씨 데이터
  * district.csv: 행정 구역 경계
  * landslide_history.csv: 2011년부터 2019년까지의 산사태 발생 이력
  * forest_47_1_gsbd.csv: 경상북도 임상도 데이터 1
  * forest_47_2_gsbd.csv: 경상북도 임상도 데이터 2
  * forest_48_1_gsnd.csv: 경상남도 임상도 데이터
  * soil_47_1_gsbd.csv: 경상북도 토양도 데이터 1
  * soil_47_2_gsbd.csv: 경상북도 토양도 데이터 2
  * soil_48_gsnd.csv: 경상남도 토양도 데이터
  * ASOS_all_2011 ~ 2019.csv: 2011년부터 2019년까지 경상도 ASOS 날씨 데이터
  
## Modeling
* Random Forest
* XGBoost
* Deep Neural Network

