# :pushpin: 3차 미니 프로젝트
</br>

## 1. 제작 기간 
- 2023년 3월 20일 ~ 3월 24일

</br>

## 2. 사용 기술
- python

</br>

## 3. 개요
- 저시력자를 위한 원화 화폐 분류

</br>

## 4. 프로젝트 내용

### 4.1 데이터 분석
- 다양한 각도에서 촬영된 샘플들이 많아 따로 이미지 증강 하지 않았다.

### 4.2. 데이터 전처리
![image](https://github.com/9eun/aivle3th/assets/113655865/a0bb90b4-6ca2-468f-ad0a-6fad5c8dca5d)      
- 세트를 분할 시킬 함수를 작성, glob 와 shutil.move()를 이용하여 imgae와 label을 분리

![image](https://github.com/9eun/aivle3th/assets/113655865/0a110e29-7c6f-45fc-bf48-e808893de4a0)
![image](https://github.com/9eun/aivle3th/assets/113655865/1fdc91ff-d875-4829-94f7-cc594c8d989c)
- JSON 파싱 이후 키값으로 yaml 파일 작성, 좌표들을 계산 한뒤 정규화시키고, txt파일로 작성하여 저장

![image](https://github.com/9eun/aivle3th/assets/113655865/1842a73c-0c5d-4b62-a23d-7d28389a30b9)
- data 빈 딕셔너리를 만들고 그안에 필요한 변수들을 넣고, yaml.dump()로 yaml파일 작성 
### 4.3. 모델 학습 및 결과
- yolo5s
![image](https://github.com/9eun/aivle3th/assets/113655865/5fd18e84-f19e-4f55-8619-69504cfe119f)
![image](https://github.com/9eun/aivle3th/assets/113655865/f021b70a-db52-4b40-9862-da4a401ea048)
![image](https://github.com/9eun/aivle3th/assets/113655865/b52806d6-cd77-4bce-bf19-ff1b9b54d485)

- yolo5m
![image](https://github.com/9eun/aivle3th/assets/113655865/ee8ca43d-d6b2-4710-a283-a976970b6f6b)
![image](https://github.com/9eun/aivle3th/assets/113655865/5a9ea2a5-8e48-439d-98fa-cf3a3c732898)

-yolo5x
![image](https://github.com/9eun/aivle3th/assets/113655865/12dc38a0-57f0-46c5-817b-fc7ce773e463)
![image](https://github.com/9eun/aivle3th/assets/113655865/20c60398-674d-4ddf-b7dc-e8d45af766e3)
 
</br>


