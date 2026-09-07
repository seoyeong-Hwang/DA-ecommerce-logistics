<div align="center">

# 📦 E-commerce Logistics Strategy Analysis

### 브라질 Olist의 풀필먼트 센터 입지선정 및 수요예측

<img src="https://img.shields.io/badge/Project-Data%20Analysis-4C78A8?style=flat-square"/>
<img src="https://img.shields.io/badge/K--means-Clustering-F2C14E?style=flat-square"/>
<img src="https://img.shields.io/badge/MILP-Optimization-E45756?style=flat-square"/>
<img src="https://img.shields.io/badge/Prophet-Forecasting-72B7B2?style=flat-square"/>

</div>

---

## 📌 Overview

브라질 이커머스 기업 **Olist의 물류 효율성을 개선하기 위해  
풀필먼트 센터의 입지를 선정하고 센터별 상품 수요를 예측한 데이터 분석 연구**입니다.

기존 3PL 물류 데이터를 분석해 지역별 배송시간·배송비 편차를 확인하고  
**입지선정 → 물류센터 최적화 → 수요예측**으로 이어지는 물류 전략을 설계했습니다.

---

## 🔍 Analysis Process

Olist 주문·고객·배송 데이터 전처리  
        ↓  
지역별 매출·배송비·배송시간 EDA   
        ↓    
입지 평가 요인 중요도 산출    
        ↓    
풀필먼트 도입 지역 선정    
        ↓  
DBSCAN 위치 이상치 제거    
        ↓    
K-means 기반 물류 거점 도출    
        ↓    
MILP 기반 고객-센터 최적 할당    
        ↓    
SARIMAX · Prophet 모델 비교    
        ↓    
센터·카테고리별 수요예측    
        ↓  
센터별 운영 및 재고 전략 제안    

## 🧩 Key Methods

### 1. Target Region Selection
- 지역별 `매출 · 평균 배송비 · 평균 배송시간`을 비교 분석
- 비용·물류·시장 요인의 중요도를 반영해 풀필먼트 도입 우선 지역 평가
- 분석 결과 **São Paulo를 초기 도입 지역으로 선정**

### 2. Fulfillment Center Optimization
- DBSCAN으로 고객 위치 이상치 제거
- K-means를 활용해 São Paulo 내 **5개 주요 물류 거점** 도출
- MILP를 통해 물류비용을 최소화하도록 센터 설치 및 고객 할당 최적화

### 3. Demand Forecasting
- 주문량의 추세·계절성·정상성·자기상관 구조 분석
- **SARIMAX와 Prophet 모델 비교**
- Black Friday와 같은 비정기 이벤트와 계절성을 반영하도록 파라미터 조정
- 최종적으로 Prophet을 활용해 센터별·카테고리별 미래 수요 예측

---

## 👤 My Contribution

### Data Preprocessing & EDA
- Olist 주문·고객·배송 데이터 전처리
- 주(State)별 매출, 주문량, 평균 배송비, 평균 배송시간 비교
- 지역별 물류 효율 편차를 확인해 풀필먼트 도입 필요성 구체화

### Target State Selection
- 풀필먼트 입지 평가 기준을 `비용 · 물류 · 시장` 요인으로 구성
- 데이터와 선행연구를 기반으로 요인별 중요도 산출
- 브라질 전체 지역을 비교해 **São Paulo를 우선 도입 지역으로 선정**

### Demand Forecasting
- **SARIMAX와 Prophet 모델 비교 및 최종 모델 선정**
- Black Friday 등 외부 이벤트를 반영하도록 모델 파라미터 튜닝

---

## 📊 Result

- 풀필먼트 서비스 초기 도입 지역으로 **São Paulo 선정**
- K-means를 통해 São Paulo 내 **5개 주요 물류 거점** 도출
- MILP 최적화 결과 **5개 후보지 모두 풀필먼트 센터 설치 대상으로 선정**
- 고객 수요와 물류비용을 반영한 센터별 고객 할당 구조 도출
- Prophet 기반 센터·카테고리별 미래 수요 예측
- `가구 · 가전디지털 · 화장품 · 스포츠`가 전 센터에서 공통적으로 높은 수요를 보임
- 센터별 수요 차이를 바탕으로 **재고·자원 배치 및 운영 전략 차별화 필요성 도출**

---

## 🏆 Achievement

### Journal Publication

**「이커머스 기업의 물류 전략 연구  
— 브라질 Olist의 풀필먼트 센터 입지선정 및 수요예측」**

- 통계기술정보연구소 **Journal of Statistical Information and Technology** **Volume 7, Number 1** **2025.04 학술지 게재**

---

## 💡 Insight

> 물류센터 입지는 단순히 주문량이 많은 지역을 선택하는 문제가 아니라  
> **시장 규모·배송 효율·고객 위치를 기반으로 입지를 최적화하고  
> 지역별 미래 수요까지 연결해야 실제 운영 전략으로 이어질 수 있다.**
