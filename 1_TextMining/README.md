
# Group Project

## 주제: 계절별 호텔 리뷰 패턴 분석
  ### 주제 선정 이유
   1. 호텔은 여가,출장,휴가 등 다양한 목적으로 이용
   2. 다양한 호텔 플랫폼에서 가장 사용자들이 사용하고 있는 아고다 선정 (다양한 리뷰들이 존재)
 
  ![image](https://github.com/user-attachments/assets/4962c882-4b94-43e0-b139-eb3309d101db)

  ### 프로젝트 목표
   1. 계절별 Word Cloud, CounterVectorize를 통한 트렌드 분석
   2. 사용자의 리뷰들을 바탕으로 호텔 리뷰의 긍부정 분류 예측 & 리뷰 점수에 대한 중요 요인 분석
   3. 클러스터링 모델들을 적용해 사용자 맞춤 리뷰 추천
  ### 데이터 수집
   * 아고다 사이트에서 9 곳의 호텔 리뷰 1900개의 리뷰 크롤링
     ![image](https://github.com/user-attachments/assets/fdc9df8e-c39d-4068-867d-9a1373ee715b)


     ![image](https://github.com/user-attachments/assets/1d4fa610-6df4-4fa4-ab93-08bde96f3e48)

   * 크롤링 과정에서의 문제로 중복된 리뷰가 다수 존재-> 최대한 다양한 호텔을 크롤링,시간이 많이 소요
 
  ### 리뷰 토큰화
   * 영어 추출, NLTK 토큰화, Gensim 불용어
  ### EDA
   * 호텔 리뷰 트렌드 분석 => 2023년도 부터 아고다 사용 증가=> 리뷰수 증가, 평균 리뷰 점수 감소
     ![image](https://github.com/user-attachments/assets/46d6393c-903e-4bc5-b6a8-388a4f79bfd4)

   * 리뷰 점수 분포 & 리뷰 길이 분포
     ![image](https://github.com/user-attachments/assets/737d9f91-95f1-4f24-a5e3-07f87d061e60)

   * 여행 유형 빈도 & 리뷰자 국적 Top 20
     ![image](https://github.com/user-attachments/assets/60dca76c-c711-4aa6-a479-484ea8a319ee)


   * 정규성 검정: 샤피로-월크 검정을 통해 정규성 검정
    * 표본의 크기가 2000이하이기 때문에 샤피로-월크 검정을 실시
     * 모든 변수가 정규성을 만족하지 않음 -> 비모수 검정 실시하기로 판단
   
   * Spearman 방식

     ![image](https://github.com/user-attachments/assets/2392396b-a9b7-41d8-b0b4-ab5aead62e3e)

      
      * 숙박 일수와 리뷰길이은 양의 상관관계
      * 리뷰 평점과 다른 컬럼은 뚜렷한 상관관계 X
  
  ### 모델링

  * K-Means clustering, GMM clustering, DBSCAN
    * 성능이 GMM clustering이 가장 좋음
      * BIC 와 AIC 기반으로 clustering 결과 -> 3이 최적의 clustering 종류
        ![image](https://github.com/user-attachments/assets/dbf44010-6821-470c-8383-e84eff22a3b9)
      * 3일 경우 분포 시각화
        ![image](https://github.com/user-attachments/assets/ad36ed0c-1a62-4ff7-855b-4e7aa46cec0d)
        
      * 리뷰수수는 label1의 숫자가 가장 많고 평균적으로 label2의 평점이 높았지만 차이 X
        ![image](https://github.com/user-attachments/assets/10dafb7a-c65f-4e53-bb25-ab5e36fbdc61)
  * 클러스터링 결과
    * 호텔 주변 Outdoor활동이나 호텔 내에 있는 gym에 관심이 많은 사람에게 적합 -> Label 0 (자주 나오는 단어들 하위 80%)
    ![image](https://github.com/user-attachments/assets/7e608b12-6491-4def-adb0-57d161f8a73c)

    * 자쿠지와 같은 욕조나 스파에 대한 리뷰가 궁금한 사람에게 적합 -> Label 1 (자주 나오는 단어들 하위 80%)

    ![image](https://github.com/user-attachments/assets/a85c352b-0f60-4427-bce5-faf9911deb44)

    * 가족 구성원들끼리 가는 여행을 준비 중인 사람이나 바다 주변 부산 호텔을 찾아보는 사람에게 적합-> Label 1 (자주 나오는 단어들 하위 80%)

    ![image](https://github.com/user-attachments/assets/65957b99-c7b3-42ae-b176-d5c30c8a0714)



# Mini Project

* 개인 프로젝트


