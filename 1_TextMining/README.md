
# Group Project

## 주제: 계절별 호텔 리뷰 패턴 분석
  ### * 주제 선정 이유
   1. 호텔은 여가,출장,휴가 등 다양한 목적으로 이용
   2. 다양한 호텔 플랫폼에서 가장 사용자들이 사용하고 있는 아고다 선정 (다양한 리뷰들이 존재)
 
  ![image](https://github.com/user-attachments/assets/4962c882-4b94-43e0-b139-eb3309d101db)

  ### * 프로젝트 목표
   1. 계절별 Word Cloud, CounterVectorize를 통한 트렌드 분석
   2. 사용자의 리뷰들을 바탕으로 호텔 리뷰의 긍부정 분류 예측 & 리뷰 점수에 대한 중요 요인 분석
   3. 클러스터링 모델들을 적용해 사용자 맞춤 리뷰 추천
  ### * 데이터 수집
   * 아고다 사이트에서 9 곳의 호텔 리뷰 1900개의 리뷰 크롤링
     ![image](https://github.com/user-attachments/assets/fdc9df8e-c39d-4068-867d-9a1373ee715b)


     ![image](https://github.com/user-attachments/assets/1d4fa610-6df4-4fa4-ab93-08bde96f3e48)

   * 크롤링 과정에서의 문제로 중복된 리뷰가 다수 존재-> 최대한 다양한 호텔을 크롤링,시간이 많이 소요
 
  * 리뷰 토큰화
   * 영어 추출, NLTK 토큰화, Gensim 불용어
  * EDA
   * 호텔 리뷰 트렌드 분석 => 2023년도 부터 아고다 사용 증가=> 리뷰수 증가, 평균 리뷰 점수 감소
     ![image](https://github.com/user-attachments/assets/46d6393c-903e-4bc5-b6a8-388a4f79bfd4)


# Mini Project

* 개인 프로젝트


