
#  객체 인식 및 segmentation 프로젝트

## 주제: 벼 이상 검출 AI 시스템

### 1. 서비스 Flow
<img src="https://github.com/user-attachments/assets/612bd50b-5eeb-4d1f-9996-f91e32aebd8e" height  =400px width =1000 px>


### 2. 데이터셋
  * 농업 정밀 데이터


 
   <img src ="https://github.com/user-attachments/assets/e4049484-b818-4536-a818-df43fa681c27" height =400px width = 600 px>

  * 저조도 환경 데이터


 
  <img src="https://github.com/user-attachments/assets/79c6d26c-9421-498a-b512-a4ec71c34627" height =400px width=600 px>

  * 벼 생식 이상
    
    <img src="https://github.com/user-attachments/assets/698db541-3b83-4ce4-9ceb-dca1e9350158" height =400px width=600 px>

### 3. Data Augmentation
  * Albumentation 적용
    
    <img src="https://github.com/user-attachments/assets/c3ff8fa5-e1b4-44d0-b4bf-3669b4253db2" height =400px width=1200 px>
    

### 4. 이미지 전처리
  * Green,NIR,RedEdge로 merge한 데이터 적용

    
     <img src="https://github.com/user-attachments/assets/5650ee39-a875-4655-be12-bae753b9ed46" height =400px width=600 px>

### 5. 모델 설명
  * Segformer 설명
   * 간단하고 효율적이고 간편한 모델
     1. Multi-scale feature
     2. MLP로만 이루어진 MLP decoder 
 <img src="https://github.com/user-attachments/assets/e73de531-14e1-4e4b-b4d5-064cda8f8bc6" height =400px width=600 px>

### 6. 결과
  * Mean IOU & Validation Loss

    ![image](https://github.com/user-attachments/assets/df30af0e-7601-464f-b2a1-bfafb3afc07f)

    ![image](https://github.com/user-attachments/assets/c412faad-7097-41f9-91e2-3eddd15feb3c)

   * Result
     1. 정밀 농업 데이터 학습

     ![image](https://github.com/user-attachments/assets/456fae77-a9fc-4e8c-bb47-fa2b9a9205a5)

     2. 정밀 농업 + 저조도 + 악천후
     
    
    ![image](https://github.com/user-attachments/assets/a901aab3-ca0c-4204-b936-758371307f81)


### 7. 결론
  * Segformer를 이용한 벼 이상 검출 segmentation 시스템 개발
   * 드론을 통해 벼 이상 영역 검출
   * 트랙털르 통해 자율주행 및 수확
### 8. 한계점
  * 모델 복잡도
   * 실제 자율주행에 적용하기 위해서 inference 속도 개선 필요
  * Real-world 적용 한계점
   * Domain range가 다르기 때문에 원하는 segmentation불가
     ![image](https://github.com/user-attachments/assets/be540b9e-c138-4bf3-8b2e-630803b45595)


