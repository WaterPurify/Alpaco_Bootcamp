
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
    ![image](https://github.com/user-attachments/assets/c3ff8fa5-e1b4-44d0-b4bf-3669b4253db2)

### 4. 이미지 전처리
  * Green,NIR,RedEdge로 merge한 데이터 적용
    ![image](https://github.com/user-attachments/assets/5650ee39-a875-4655-be12-bae753b9ed46)

### 5. 모델 설명
  * Segformer 설명
   * 간단하고 효율적이고 간편한 모델
     1. Multi-scale feature
     2. MLP로만 이루어진 MLP decoder 
 <img src="https://github.com/user-attachments/assets/e73de531-14e1-4e4b-b4d5-064cda8f8bc6" height =400px width=600 px>



