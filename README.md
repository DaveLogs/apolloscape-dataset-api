# ApolloScape DataSet API

본 프로젝트에서는 ApolloScape Dataset의 사용방법을 설명하는 Toolkit을 분석, 가이드를 작성하고자 한다. ApolloScape DataSet 및 API는 아래 참고를 통해 확인할 수 있다.

ApolloScape DataSet API Toolkit은 다음 세 가지 작업을 포함한다.

- 3D car instance understanding
- Lanemark Segmentation
- online self-localization

우선적으로 다음을 통해 필요한 패키지의 설치 및 환경변수 설정을 진행한다.

```
pip install -r requirements.txt
source source.rc
```

## 3D Car Instance Understanding

Dataset 폴더 구조는 다음과 같다.

```
{root}/{folder}/{content}/{image_name}{ext}
```

또한, ```folder```의 개별 요소는 다음과 같다.

- ```camera``` 카메라 내장 매개변수
- ```car_models``` python에 친숙한 pkl 형태로 다시 저장된 자동차 모델 세트. (인덱스는 1부터 시작)
- ```car_poses``` 이미지에 레이블된(labelled) 자동차 포즈 정보
- ```split``` 각각 train, val 용도로 분할한 이미지 리스트 정보
- ```images``` 이미지 집합






## 참고
ApolloScapeAuto DataSet API:
https://github.com/ApolloScapeAuto/dataset-api
ApolloScapeAuto DataSet:
http://apolloscape.auto/
