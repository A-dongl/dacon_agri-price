# dacon priceforcasting agriculture

## 주제
국민생활과 밀접한 10개 농산물 품목의 가격 예측
(배추, 무, 양파, 사과, 배, 건고추, 깐마늘, 감자, 대파, 상추)

## 설명
traindata:  2018년 ~ 2021년 / 순 단위(10일)

추론 시점 T: 비식별화된 2022년의 순 단위(10일)의 데이터

추론은
추론 시점 T 기준: 최대 3개월의 순 단위(10일)의 입력 데이터를 바탕으로
T+1순, T+2순, T+3순의 평균가격을 예측

### 10개의 품목 중 조건
건고추       화건       30kg      상품
사과        홍로, 후지  10개       상품
감자        감자 수미   20키로상자  상
배          신고       10개       상품
깐마늘(국산) 깐마늘(국산) 20kg      상품
무          무         20키로상자  상
상추        청         100g       상품
배추        배추       10키로망대   상
양파        양파       1키로       상
대파        대파(일반)  1키로단     상


# file explanation


- 산지공판장과 전국도매는 건고추 데이터 없이 순무 데이터만 존재
- 몇몇 품종은 품종명이 요구사항과 일치하는 것이 없음.

 - datacheck_v1 : train data preprocessing -> splited data what i need (all & another )
 - datacheck_v2 : call v1 data & check \n
 - datacheck_v3 : 산지공판장 preprocessing -> splited data what i need (all & another )
 - datacheck_v3 : 전국도매 preprocessing -> splited data what i need (all & another )
