# 컴퓨터 비젼 분류 미니 프로젝트

## 주제: 역대 화가 50인 자동 분류 프로젝트

* 주제 선정 이유: AI가 그린 예술 작품의 저작권 침해 문제가 심각

* 프로젝트 목표
  1. Data Augmentation (데이터 증강)
  2. Class Weighted ( 클래스 가중치 적용)
  3. Vision Transformer (트랜스포머 기반 모델 적용)
 
* 데이터 소개
  * 이름:  Best Artworks of All Time (역대 가장 영향력 있는 50명의 화가들의 작품)
  ![image](https://github.com/user-attachments/assets/4b8e3fb9-b767-46a8-8a1c-b0c204f420ea)

* 데이터 증강
  * Trivial Augmentation Wide 방식
  * Custom Data Augmentation 적용
    1. Gaussian Blur
    2. Random Perpective
    3. Random Horizontal Flip
    4. Random Rotation
    5. Color Jitter
* 데이터 불균형
  * 학습 데이터 분포
< img src="https://github.com/user-attachments/assets/2c5ec3d7-0f41-4f03-b19c-2e56feefe201" height =300px width= 400px>
  * Data imbalance를 해소하기 위한 방안 => 미니 배치에 class를 균형적으로 load
  * 적은 class에 더 큰 가중치를 부여하여 weight 업데이트

* 주요 모델 설명
  * ResNet (CNN의 대표)
    ![image](https://github.com/user-attachments/assets/8965f03c-45c1-417f-af7a-cc8161825e91)

    
  * Vision Transformer (Transformer의 대표)
  
  ![image](https://github.com/user-attachments/assets/14af79cd-5adc-4838-98d2-c723c067a42c)

 


