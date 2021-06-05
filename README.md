# 날씨 빅데이터 콘테스트 - 공공협력형
4월 26일 ~ 6월 28일까지 진행되는 기상청 주최하는 [날씨 빅데이터 콘테스트](https://bd.kma.go.kr/contest/main.do)

멋쟁이사자처럼 K-Digital Training의 마지막 프로젝트로 4인 1조로 참여

Collaborated with [Bill Kim](https://github.com/billkim418), [Heewon Kwon](https://github.com/HeewonKwak), [Titus Choi](https://github.com/TitusChoi)

기상에 따른 산림재해 예측 및 산사태 예측기술 개발, 개선 프로젝트

## 활용 데이터
* 산사태 발생 이력
  + 2011년 7월부터 2019년 10월까지의 경상북도, 경상남도 내 산사태 발생 이력
* 산림 공간 정보
  + 경상북도, 경상남도 임상도 및 토양도
* 행정 구역 경계
  + 경상북도, 경상남도 읍, 면, 동 지역 구분
* [기상청 날씨 데이터](https://data.kma.go.kr)
  + 기상 자료 개방 포털의 날씨 데이터 API


## 데이터 설명
- data_submission: 분석과 모델링을 위해 쓰이는 전처리된 정제 데이터
  * ASOS_final: 기상청 날씨 데이터를 크롤링하고 읍면동 단위로 정리한 종관기상관측장비 **ASOS** 데이터 (csv)
  * AWS_final: 기상청 날씨 데이터를 크롤링하고 읍면동 단위로 정리한 방재기상관측장비 **AWS** 데이터 (csv)
  * landslide_asos_merged: 산사태 발생이력과 ASOS 데이터를 병합한 데이터 (csv)
  * landslide_final: 산사태 발생 이력 정리 데이터 (csv)
- data_raw: 날씨 빅데이터 콘테스트에서 제공되는 기존 데이터 및 크롤링을 통해 구한 원본 데이터
  * district: 행정 구역 경계 (csv)
  * landslide_history: 산사태 발생이력 (csv)
  * forest_47_1_gsbd: 임상도 47_1 경상북도 (csv)
  * forest_47_2_gsbd: 임상도 47_2 경상북도 (csv)
  * forest_48_1_gsnd: 임상도 48 경상남도 (csv)
  * soil_47_1_gsbd: 토양도 47_1 경상북도 (csv)
  * soil_47_2_gsbd: 토양도 47_2 경상북도 (csv)
  * soil_48_gsnd: 토양도 48 경상남도 (csv)
  * META_관측지점정보_ASOS: ASOS 관측 지점의 위치 정보 (csv)
  * META_관측지점정보_AWS: AWS 관측 지점의 위치 정보 (csv)
