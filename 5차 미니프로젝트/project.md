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
##### 1단계
- LogisticRegression              
![image](https://github.com/9eun/aivle3th/assets/113655865/23f512d1-5781-4130-9cc8-5f2be7e5a2cf)
- Sequential                   
![image](https://github.com/9eun/aivle3th/assets/113655865/9d15c215-c8cd-4ba9-8f4d-38ef93269477)
![image](https://github.com/9eun/aivle3th/assets/113655865/fb43c733-f1d6-4002-b987-54654510c668)

##### 2-1단계 : 정적 동작 세부 분류
- 전처리             
![image](https://github.com/9eun/aivle3th/assets/113655865/b6d59354-11c3-487e-8858-426f730b54cd)
- Sequential                         
![image](https://github.com/9eun/aivle3th/assets/113655865/bdd9dd97-0769-425d-9c89-ad3070d77dca)
![image](https://github.com/9eun/aivle3th/assets/113655865/eb94a8c9-3074-4e54-a30a-09f8e507ed00)

##### 2-2단계 : 동적 동작 세부 분류
- 전처리                  
![image](https://github.com/9eun/aivle3th/assets/113655865/4a7d696c-3d5f-4758-bc04-05149bcb1e13)
- Sequential                      
![image](https://github.com/9eun/aivle3th/assets/113655865/a9efdeb5-290f-4e47-925d-7d71e8fe7d3e)
![image](https://github.com/9eun/aivle3th/assets/113655865/587806a9-7556-40ec-b803-45223db34756)

##### 3단계: 예측 결과 합치기
![image](https://github.com/9eun/aivle3th/assets/113655865/e72a0760-5f9e-4986-9c4b-e8973b9bfa68)

</br>


