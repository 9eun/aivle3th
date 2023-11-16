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
![image](https://github.com/9eun/aivle3th/assets/113655865/23e74090-bc98-41d4-a73e-c9b7348c1a93)
![image](https://github.com/9eun/aivle3th/assets/113655865/dc06d461-6a47-4630-b794-6f94a41ce6b7)

### 4.2. 모델 학습 및 결과
#### 4.2.1. 데이터 전처리
- LabelEncoder로 스케일링 진행
#### 4.2.2. 기본 모델링
- LogisticRegression         
![image](https://github.com/9eun/aivle3th/assets/113655865/a9fd58e5-2dbe-4d32-a1a5-621b84063ecf)
- Sequential     
![image](https://github.com/9eun/aivle3th/assets/113655865/3bc29db2-12de-4f75-a7a2-310ecf3cf909)
![image](https://github.com/9eun/aivle3th/assets/113655865/43090b66-f1b4-4927-8afd-86b3b9f6f617)

#### 4.2.3 데이터 전처리
- Label 추가 : data 에 Activity_0 를 추가
![image](https://github.com/9eun/aivle3th/assets/113655865/52a83bdb-654e-495b-a202-ffe24d34d6a8)
![image](https://github.com/9eun/aivle3th/assets/113655865/53037fdb-1887-481e-81ba-5cdd5b34ce6c)

#### 4.2.4 단계별 모델링
![image](https://github.com/9eun/aivle3th/assets/113655865/72b67874-11f0-4e6e-9903-593bf36b4672)

##### 1단계
- LogisticRegression              
![image](https://github.com/9eun/aivle3th/assets/113655865/b0c96a92-de3e-4459-88ca-4f1e72dbe69f)

- Sequential                   
![image](https://github.com/9eun/aivle3th/assets/113655865/a09a7b36-0df6-4bb8-a0db-8991912cdb38)
![image](https://github.com/9eun/aivle3th/assets/113655865/9d390d7b-24f9-44fb-a1f6-6dbaeebdc4fc)

##### 2-1단계 : 정적 동작 세부 분류
- 전처리             
![image](https://github.com/9eun/aivle3th/assets/113655865/c60cf1e0-717c-4894-b2bd-41fefe812e40)

- Sequential                         
![image](https://github.com/9eun/aivle3th/assets/113655865/1e170b65-c34d-4ffc-babb-5f03125c6419)
![image](https://github.com/9eun/aivle3th/assets/113655865/d3ebcc26-c681-437d-aa01-e9663c009960)

##### 2-2단계 : 동적 동작 세부 분류
- 전처리                  
![image](https://github.com/9eun/aivle3th/assets/113655865/c1b4bf85-e168-4e26-82e9-7d63edcf7eed)

- Sequential                      
![image](https://github.com/9eun/aivle3th/assets/113655865/da267367-f139-4ce8-a1ae-33330a4b6083)
![image](https://github.com/9eun/aivle3th/assets/113655865/006765a8-0fed-4c7d-a62e-9f22d847ed8a)

##### 3단계: 예측 결과 합치기
![image](https://github.com/9eun/aivle3th/assets/113655865/29275e51-6577-4010-8ea4-451dc43e0b9c)

</br>


