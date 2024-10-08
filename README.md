# Resume

## Name : 채성욱<br/>

<img src = "https://user-images.githubusercontent.com/95071769/210631043-1fb14a8b-2bb8-4162-8d86-9da0722e2243.jpg" width="250px">

저는 AI와 관련한 개발에 관심이 많습니다.!

## Contact
- Email : nodang124@gmail.com
- GitHub : https://github.com/chae0328

<br/>
<br/>

## Projects
<!--### [E-S(Equiptment-Saftey) 시스템](https://github.com/chae0328/YOLOv4_darknet_ES_System.git)-->
### E-S(Equiptment-Safty) 시스템
* **골절기에 의한 손 부상을 방지하기 위한 시스템**
* 목적 : 산업 근로자들의 안전을 개선하기 위한 프로젝트
  
* 알고리즘 구성
  * **Darknet 프레임워크를 사용한 학습 진행** <br/><br/> YOLO-mark를 이용하여 손 데이터를 라벨링하여 C언어 기반의 DarkNet 프레임워크를 사용하여 데스크탑에서 학습을 진행하였습니다.

  * **Jetson Nano 보드에 YOLOv4-tiny 적용** <br/><br/> 골절기의 경우 주로 산업현장이나 공장에서 자주 사용되므로 데스크탑 처럼 부피가 큰 컴퓨터는 효율성이 떨어집니다. 따라서 부피에 부담이 적고 딥 러닝을 구현하는데 최적화된 소형 컴퓨터인 Jetson Nano 보드를 이용하였습니다. <br/><br/> Jetson Nano 보드에 YOLOv4-tiny를 적용하여 사람의 손과 골절기의 칼날을 인식할 수 있도록 시스템을 구성하였습니다.

  * **손과 골절기 칼날의 거리에 의한 골절기 정지 시스템 구현** <br/><br/> Jetson Nano 보드를 통하여 인식된 손이 칼날과 가까워지게되면 자동으로 칼날이 정지될 수 있도록 시스템을 구현하였습니다.

  * **개선할 부분** : 객체 탐지를 할때 배경에 따라 정확도가 낮게 나오는 경향을 개선할 필요가 있고, Jetson Nano 보드보다 가벼운 보드에도 원활히 실행될 수 있도록 경량화될 필요가 있습니다.<br/>
![](https://user-images.githubusercontent.com/95071769/210629246-be9a924a-355a-45cf-bc2a-b4cd93841aac.gif)

<br/>
<br/>

<!-- ### [객체 알고리즘을 활용한 젖소 분만 예정 탐지 및 난산 손실 예방 시스템](https://github.com/chae0328/YOLOv4_darknet_CowCalvingCare_System.git) -->
### 객체 알고리즘을 활용한 젖소 분만 예정 탐지 및 난산 손실 예방 시스템
* **비전 시스템을 활용해 난산 위험을 예측하고 분만 결과를 알릴 수 있는 시스템**
* 목적 : 1차 산업의 인력 부족의 불편함을 해소하기 위한 프로젝트
  
* 알고리즘 구성
  * **Darknet 기반 YOLOv4 모델을 통한 분만 및 난산 위험 탐지** <br/><br/> 소가 일정시간동안 꼬리를 지속적으로 들어올리는 행위는 분만 징후와 매우 밀접하게 관련되어있습니다. 목장 CCTV 영상 데이터를 활용하여 꼬리를 들어올리는 영역과 난산을 예방하고자 출산이 원할하게 됫는지 판단하기 위해 출산 데이터도 레이블링을 수행하여 학습을 진행하였습니다.  

  * **Firebase를 이용한 모바일 애플리케이션 알림 시스템 구현** <br/><br/> 목장 관리자가 위치에 상관없이 상황을 알수 있도록 하기 위해 분만 및 난산 위험 증상을 Firebase기반 애플리케이션을 통해 알림을 보낼 수 있도록 구현하였습니다.

  * **개선할 부분** : 젖소가 꼬리를 올린 형태에 대한 정확도가 부족하여 학습에 필요한 데이터를 추가로 수집하여야 합니다. <br/> Firebase를 통해 알림을 전송받을 때 지연시간이 존재하므로 추후 이를 개선하여야 합니다. <br/> 젖소의 꼬리를 올리는 행동이 얼마나 지속되어야 분만 예측이라 할수 있는지에 대한 정확한 연구도 진행되어야 합니다.<br/>
![](https://user-images.githubusercontent.com/95071769/210629375-2fa72cb6-76ec-4330-8e3d-8409f0ed7133.gif)

<br/>
<br/>

<!-- ### [자세 추정 모델을 이용한 젖소의 행동 변화에 따른 분만 징후 예측](https://github.com/chae0328/YOLOv4_darknet_CowCalvingCare_System.git) -->
### 자세 추정 모델을 이용한 젖소의 행동 변화에 따른 분만 징후 예측
* **포즈 추정과 시계열 예측 모델을 활용하여 꼬리를 지속적으로 올리는 행위를 탐지 하기 위한 연구**
* 목적 : 객체 알고리즘을 활용한 젖소 분만 예정 탐지 및 난산 손실 예방 시스템 성능을 개선하기 위한 프로젝트
  
* 알고리즘 구성
  * **Top-Down 방식을 통한 젖소의 골격 키포인트 도출** <br/><br/> YOLOv8을 활용하여 이미지에서 젖소를 탐지 하였습니다. 이후  [DeepLabCut](https://github.com/DeepLabCut/DeepLabCut)을 활용하여 개별 젖소를 탐지한 영상을 사각 이미지로 추출(cropping) 하였고 골격 키포인트를 생성하여 자세 추정을 진행하였습니다.
<br/><br/>
  * **젖소의 골격 키포인트 설정** <br/><br/> 꼬리 끝점, 꼬리 중간점, 꼬리 시작점, 장골, 흉추, 견갑골로 총 6개의 관절 좌표점을 정의하였습니다.
<br/><br/>
![관절키포인트지정](https://github.com/user-attachments/assets/ceada503-5c29-47da-8945-5255a8af543f)
<br/><br/>
  * **LSTM 모델을 활용한 분만 징후 예측** <br/><br/> L은 좌측, R은 우측을 의미하며 0은 꼬리의 각도가 0° 이상 20° 미만, 30은 꼬리의 각도가 30° 이상 60° 미만, 60은 꼬리의 각도가 60° 이상인 것을 의미합니다. 꼬리의 각도가 30° 이상 60° 미만, 또는 60° 이상일 경우는 꼬리를 올리는 행위로 판별하였고, 꼬리의 각도가 0° 이상 20° 미만일 경우는 꼬리를 들어올리지 않는 행위로 판별하였습니다.
<br/><br/>
![꼬리올리는 방식](https://github.com/user-attachments/assets/07a85415-c5e1-40da-b262-9f23adb50137)
<br/><br/>
  * **개선할 부분** :주위 환경이나 장애물로 인한 문제점을 겪었고 다양한 환경에서도 안정적인 성능을 보장하는 알고리즘이 필요합니다.<br/>
![cow_pose_estimation](https://github.com/user-attachments/assets/1bac7d6f-5e6e-464c-aa7f-2b2244e24607)

<br/>
<br/>

<!-- ### [얼굴형 분석에 따른 맞춤 헤어스타일 합성 시스템 구현](https://github.com/chae0328/Custom_HairStyle_Synthesis.git) -->
### 얼굴형 분석에 따른 맞춤 헤어스타일 합성 시스템 구현
* **어플리케이션을 통해 사용자가 얼굴형에 적합한 헤어스타일을 찾고, 시뮬레이션 할 수 있는 시스템**
* 목적 : 헤어스타일 선택에 대한 고민을 해결하기 위한 프로젝트
  
* 알고리즘 구성(This project contains code released by [Barbershop](https://github.com/ZPdesu/Barbershop).)
  * **StyleGAN2 모델과 Face Parsing 모델을 이용한 이미지 합성** <br/><br/> Face Parsing 모델을 이용하여 사용자의 이미지와 합성할 이미지의 segmentation 결합 후 FFHQ 데이터셋으로 사전 학습된 StyleGAN2 모델을 통해 합성된 이미지가 생성될 수 있도록 진행하였습니다.

  * **OpenCV를 활용한 얼굴 턱선 검출 및 얼굴형 분류** <br/><br/> 이미지의 합성을 원할하게 진행하고자 입력 받은 사용자의 사진 크기를 정규화 처리하였으며 얼굴정렬 모델 및 OpenCV를 활용하여 얼굴 턱선추출을 통해  얼굴형을 분류 할 수 있도록 컨볼루션 신경망을 활용하였습니다. <br/><br/> 이후 분류된 얼굴형에 적합한 헤어스타일을 선정하여 사용자의 이미지 합성을 이미지 합성 모델을 통해 진행하였습니다.

  * **Firebase를 이용한 모바일 애플리케이션 연동** <br/><br/> Firebase를 이용하여 이미지 합성 시스템에서 사용자의 옵션과 이미지를 전송받은 후 합성 결과를 받아서 출력할 수 있도록 애플리케이션을 제작하였습니다.
    
  * **개선할 부분** : 해당 시스템에서 사용한 합성모델은 결과 추출까지 상당한 시간이 소요되었으며 해당 관련된 성능 개선이 필요합니다.<br/> 외부 근거 자료로 인한 적합한 헤어스타일을 찾아주는 것이 아닌 데이터 분석을 비롯 하여 구현된 딥러닝 기반의 추천시스템 연구도 필요합니다.<br/>
![](https://user-images.githubusercontent.com/95071769/210629335-710384bf-4121-41fa-9d33-551e821cba13.gif)

<br/>
<br/>

### [1/5 자율 주행 프로젝트](https://github.com/chae0328/1_5_Autonomous-driving/blob/main/README.md) <-- Please access the link for more information. !! <br/>
* **컴퓨터 비전과 라이다 센서를 활용한 차량 제어**<br/><br/>
![corner_car_sample](https://github.com/user-attachments/assets/39c0a9a9-1a4a-4b75-b593-030270230401)
![corner-sample](https://github.com/user-attachments/assets/b6f249bb-3624-475e-aeb9-587d23cec4e1)

<br/>
<br/>

## Prizes

* **2024 1/5 자율주행 차량 제작 및 경진대회 [공로상]**
  * 수상년월 2024.7.10
  * 발행기관 : 대구대학교 공학교육혁신센터

* **2023 1/5 자율주행 차량 제작 및 경진대회 [장려상]**
  * 수상년월 2023.10.26
  * 발행기관 : 대구대학교 공학교육혁신센터
    
* **한국산업정보학회 추계학술대회 [우수논문상]**
  * 수상년월 2022.12.02
  * 발행기관 : 한국산업정보학회

* **2022학년도 정보통신대전 학생작품경진대회 [장려상]**
  * 수상년월 2022.11.17
  * 발행기관 : 대구대학교

* **한국산업정보학회 춘계학술대회 [우수논문상]**
  * 수상년월 2022.06.17
  * 발행기관 : 한국산업정보학회

* **2021-2학기 캡스톤디자인 경진대회 [우수상]**
  * 수상년월 2021.12.28
  * 발행기관 : 대구대학교 LINC+사업단

* **2021년 경북형 SW인력양성 및 일자리창출 사업 성과공유대회 [은상]**
  * 수상년월 2021.12.01
  * 발행기관 : 경북테크노파크
<br/>

## 학술회의(발표)

* **[자세 추정 알고리즘 기반 젖소의 행동 변화에 따른 분만 징후 예측](https://drive.google.com/file/d/1C3bY7Lui8t1goZIiIyd4dfAyA0xVJgnN/view?usp=sharing)**
  * 일시 : 2023.11.10
  * 주최기관 : 한국산업정보학회

* **[얼굴형 분석에 따른 맞춤 헤어스타일 합성 시스템 구현](https://drive.google.com/file/d/1JaSaX93qrTxa_MoR6r2zn5xS8wiJwW8T/view?usp=sharing)**
  * 일시 : 2022.12.02
  * 주최기관 : 한국산업정보학회

* **[객체 알고리즘을 활용한 젖소 분만 예정 탐지 및 난산 손실 예방 시스템](https://drive.google.com/file/d/16_rhO98BP18dDVhe6u2B2O9AGF2B-R-C/view?usp=sharing)**
  * 일시 : 2022.06.17
  * 주최기관 : 한국산업정보학회

* **[딥러닝 기반 젖소 꼬리 탐지 및 행동 분석](https://drive.google.com/file/d/1W_hA4Z9-mH4tZeSnDyQEr8B5-8OY1dSi/view?usp=sharing)**
  * 일시 : 2022.05.19
  * 주최기관 : 대한임베디드공학회
