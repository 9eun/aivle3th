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
- 세트를 분할 시킬 함수를 작성, glob 와 shutil.move()를 이용하여 imgae와 label을 분리
![image](https://github.com/9eun/aivle3th/assets/113655865/8accc5a7-1c95-42f7-b749-5e0f17793a74)

- JSON 파싱 이후 키값으로 yaml 파일 작성, 좌표들을 계산 한뒤 정규화시키고, txt파일로 작성하여 저장
![image](https://github.com/9eun/aivle3th/assets/113655865/a00cf0b8-a379-4046-a2c9-5491ae2c7036)
![image](https://github.com/9eun/aivle3th/assets/113655865/74db2e28-0b4c-4798-895f-1608450dddeb)


- data 빈 딕셔너리를 만들고 그안에 필요한 변수들을 넣고, yaml.dump()로 yaml파일 작성
![image](https://github.com/9eun/aivle3th/assets/113655865/3c9521f7-48ba-4515-9151-beba8ef62162)

### 4.3. 모델 학습 및 결과
- yolo5s
![image](https://github.com/9eun/aivle3th/assets/113655865/bdca4f86-6e09-43cb-9a68-4c0020f34d37)
![image](https://github.com/9eun/aivle3th/assets/113655865/e99b09d4-b3b0-4689-889c-08010980eee1)
![image](https://github.com/9eun/aivle3th/assets/113655865/5dd139f9-e38e-4b6c-81a8-dc541612c316)

- yolo5m
![image](https://github.com/9eun/aivle3th/assets/113655865/a521455e-7bf4-48ac-b0aa-b03619c7316f)
![image](https://github.com/9eun/aivle3th/assets/113655865/28024bab-eb15-4a66-b548-b3b6213a42dd)

-yolo5x
![image](https://github.com/9eun/aivle3th/assets/113655865/096f6872-81b5-4df6-b021-89ec347ea647)
![image](https://github.com/9eun/aivle3th/assets/113655865/1ecd5dc6-e398-461a-b6a7-c6e55ec3cc1e)

</br>


