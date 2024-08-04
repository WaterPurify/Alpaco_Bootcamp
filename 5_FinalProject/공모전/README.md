# **공모전** 🏆
---

## 1. 경상남도 빅데이터 분석 공모전

![공모전 이미지](https://github.com/user-attachments/assets/40c389f1-b076-4192-a24d-08ca1a5ea8cc)

- **기간**: 7월 23일까지
- **주제**: 빈집 활용을 위한 관광지 최적 입지 분석
- **목적**: 경상남도 지역 경제 활성화를 위한 빈집 활용 관광지 개발
  - 전국적으로 심각한 빈집 문제(범죄 노출, 폐가구와 생활쓰레기 방치)를 해결하고자 함

### 데이터

1. **관광지 수요 분석 데이터**
   - 시군별 인구 증감율, 빈집 비율, 경상남도 관광업 현황 데이터
2. **입지 분석 데이터**
   - 관광 수요지 데이터, 입지 후보지 데이터
3. **생성형 AI를 위한 데이터**
   - 기존 우주 및 한옥 컨셉 카페, 게스트하우스 데이터

### 진행 내용

1. **경상남도 시/군별 관광지 수요 분석**
   - 전국 시/군별 인구 증감율, 빈집 비율 분석
   - 경상남도 시/군별 관광업 현황 분석

2. **합천군 세부 행정구역별 관광지 수요 분석**
   - 법정동 단위로 관광지 입지 후보지 선정
   - 지역 내 숙박업소, 음식점, 기타 관광지 등 관광 인프라 고려하여 수요량 산정

3. **MCLP 기법을 활용한 입지 선정**
   - 입지 후보지 중 제약 조건에 맞는 수요를 최대한 커버하는 최종 입지 후보지 3곳 선정

### 결과

- 신규 관광지 개발로 인한 관광 수입 증대
- 관광지 주변 상권 발달
- 빈집 감소로 인한 쾌적한 주변 환경 조성
- 추후 빈집 관련 정책 수립 시 근거 자료로 활용

---

## Code 설명

### EDA

- **EDA_0722_final.ipynb**: 경상남도 데이터 시각화 코드
- **수요지점_시각화.ipynb**: 경상남도 수요지점들 (카페, 레스토랑, 숙박시설, 주유소 등) 시각화 코드

### MCLP

- **MCLP_example.ipynb**: MCLP 예제 코드
- **MCLP_최종.ipynb**: MCLP를 사용하여 합천군 리들을 기준으로 최적의 입지 선정 코드

### LoRA-Stable Diffusion

- 참고 코드: [https://github.com/cloneofsimo/lora](https://github.com/cloneofsimo/lora)

---

## 카페 후보지

<p align="center">
   <img src="https://github.com/user-attachments/assets/ec73b6ff-abba-4ed8-a03f-1a66540b775b" align="center" width="45%">
   <img src="https://github.com/user-attachments/assets/6ead664d-a281-4434-8d07-d2f861870e2a" align="center" width="45%">
</p>

## 숙박시설 후보지

<p align="center">  
   <img src="https://github.com/user-attachments/assets/9c3a6db3-c854-41c1-a972-9053e4691aa6" align="center" width="30%"> 
   <img src="https://github.com/user-attachments/assets/21ebdc04-0ff0-47c0-87af-c621b8cc9eac" align="center" width="30%"> 
   <img src="https://github.com/user-attachments/assets/c8056186-090d-4497-bd43-33449d9b604f" align="center" width="30%"> 
</p>


### 숙박시설 후보지

<p align="center">  
   <img src="https://github.com/user-attachments/assets/9c3a6db3-c854-41c1-a972-9053e4691aa6" align="center" width="30%"> 
   <img src="https://github.com/user-attachments/assets/21ebdc04-0ff0-47c0-87af-c621b8cc9eac" align="center" width="30%"> 
   <img src="https://github.com/user-attachments/assets/c8056186-090d-4497-bd43-33449d9b604f" align="center" width="33%">  </p>
