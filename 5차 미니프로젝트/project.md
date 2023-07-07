# :pushpin: 5차 미니 프로젝트
</br>

## 1. 제작 기간 
- 2023년 4월 10일 ~ 4월 14일

</br>

## 2. 사용 기술
- python

</br>

## 3. 개요
- 스마트폰 센서 데이터 기반 모션 분류     

</br>

## 4. 프로젝트 내용

### 4.1 데이터 분석
- 관점1 : 6개 행동 구분                 
관점2 : 동적, 정적 행동 구분              
관점3 : Standing 여부 구분             
관점4 : Sitting 여부 구분             
관점5 : Laying 여부 구분              
관점6 : Walking 여부 구분              
관점7 : Walking_upstairs 여부 구분             
관점8 : Walking_downstairs 여부 구분
각각의 관점별 기본모델(Random forest)생성한 후 변수 중요도 확인 후 변수 저장
- 예시)
![image](https://github.com/9eun/aivle3th/assets/113655865/37c7f5c2-f4a7-487d-b5ce-cb29c0374831)
![image](https://github.com/9eun/aivle3th/assets/113655865/c867c9e6-463d-48ae-b655-1dae4ed57350)

### 4.2. 모델 학습 및 결과
#### 4.2.1. 데이터 전처리
- LabelEncoder로 스케일링 진행
#### 4.2.2. 기본 모델링
- LogisticRegression         
  ![image](https://github.com/9eun/aivle3th/assets/113655865/fefefb39-bed6-4819-a00a-2f399d87f1fb)
- Sequential     
  ![image](https://github.com/9eun/aivle3th/assets/113655865/8b99eef7-e0e7-4adf-9cc8-4fe882384422)
  ![image](https://github.com/9eun/aivle3th/assets/113655865/aabacc02-7eb4-4cee-9297-a7d3fb82bbb5)

#### 4.2.3 데이터 전처리
- Label 추가 : data 에 Activity_0 를 추가
 ![image](https://github.com/9eun/aivle3th/assets/113655865/2d029195-f488-4a6e-b3b2-767eb55931ab)
  ![image](https://github.com/9eun/aivle3th/assets/113655865/c1b8fe32-36a1-4183-80ec-a017ca5541e8)

#### 4.2.4 단계별 모델링
![image](https://github.com/9eun/aivle3th/assets/113655865/7545f7fd-66a4-4c5d-978a-8db0e1218489)



</br>


