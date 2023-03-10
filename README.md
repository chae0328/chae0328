# Resume

안녕하세요<br/>
저는 AI 개발자를 꿈꾸는 채성욱 입니다.

<img src = "https://user-images.githubusercontent.com/95071769/210631043-1fb14a8b-2bb8-4162-8d86-9da0722e2243.jpg" width="250px">


저는 AI 개발에 관심이 많습니다!:smiley:

## Contact
- Email : nodang124@gmail.com
- GitHub : https://github.com/chae0328

<br/>

## Tech Stack
#### Platforms & Languages


<img src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=Docker&logoColor=white"/> <img src="https://img.shields.io/badge/Visual%20Studio%20Code-007ACC?style=flat&logo=Visual%20Studio%20Code&logoColor=white"/> <img src="https://img.shields.io/badge/Android%20Studio-3DDC84?style=flat&logo=Android&logoColor=white"/>

<img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=Python&logoColor=white"/> <img src="https://img.shields.io/badge/C++-00599C?style=flat&logo=Cplusplus&logoColor=white"/> <img src="https://img.shields.io/badge/Java-007396?style=flat"/> <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=HTML5&logoColor=white"/> <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=JavaScript&logoColor=black"/>


#### Tools

<img src="https://img.shields.io/badge/Firebase-FFCA28?style=flat&logo=Firebase&logoColor=white"/> <img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=GitHub&logoColor=white"/>


<br/>
<br/>

## Projects

### [얼굴형 분석에 따른 맞춤 헤어스타일 합성 시스템 구현](https://github.com/chae0328/Custom_HairStyle_Synthesis.git)
* **프로그램을 통한 사용자에게 적합한 헤어스타일 이미지 합성 시스템**
* 헤어스타일 선택에 대한 고민을 해결하기 위한 프로젝트
* 개발기간
  * 2022.04 ~ 2022.10
* 역할
  * **StyleGEN 모델과 Face Parsing 모델을 이용한 이미지 합성 시스템 구현** <br/><br/> 사용자의 이미지와 합성할 이미지를 Face Parsing 모델을 이용하여 분할 결합하여 FFHQ 데이터셋으로 사전 학습된 StyleGEN 모델을 통해 합성된 이미지가 생성될 수 있도록 시스템을 구현하였습니다.

  * **OpenCV를 활용한 얼굴 턱선 검출 및 얼굴형 분류** <br/><br/> 사용자의 이미지를 정규화하여 얼굴정렬 모델 및 OpenCV를 활용하여 얼굴 턱선을 추출하여 이를 통해 얼굴형을 분류할수 있도록 구현하였습니다. <br/><br/> 이미지 합성 시스템에서는 분류된 얼굴형에 적합한 헤어스타일을 선정하여 사용자의 이미지와 합성을 진행합니다.

  * **Firebase를 이용한 모바일 애플리케이션 연동** <br/><br/> Firebase를 이용하여 이미지 합성 시스템에서 사용자의 옵션과 이미지를 전송받은 후 합성 결과를 받아서 출력할 수 있도록 애플리케이션을 제작하였습니다.

  * **개선할 부분** : 이미지 합성 모델을 이용하여 합성을 할 때 상당한 시간이 소요되므로 모델 경량화를 통해 합성 속도를 향상시킬수 있어야 한다. <br/><br/> 외부적 근거 자료로 인한 적합한 헤어스타일을 찾아주는 것이 아닌 데이터 분석을 비롯하여 구현된 딥러닝 기반의 추천시스템 연구도 필요하다.<br/>
![](https://user-images.githubusercontent.com/95071769/210629335-710384bf-4121-41fa-9d33-551e821cba13.gif)



<br/>
<br/>


### [객체 알고리즘을 활용한 젖소 분만 예정 탐지 및 난산 손실 예방 시스템](https://github.com/chae0328/YOLOv4_darknet_CowCalvingCare_System.git)
* **비전 시스템을 활용해 난산 위험을 예측하고 분만 결과를 알릴 수 있는 시스템**
* 1차 산업의 인력 부족의 불편함을 해소하기 위한 프로젝트
* 개발기간
  * 2021.04 ~ 2021.12
* 역할
  * **Darknet 기반 YOLOv4 모델을 통한 탐지 시스템 구현** <br/><br/> 젖소의 분만 현상과 출산을 탐지하기 위해 분만 현상 중 젖소가 꼬리를 올린 형태와 젖소가 출산하는 모습을 학습시키고 일정 시간 이상 탐지될 경우 분만 예정 및 난산 위험과 젖소의 출산을 알릴 수 있는 기능을 구현하였습니다.

  * **Firebase를 이용한 모바일 애플리케이션 알림 시스템 구현** <br/><br/> 목장의 관리자가 위치에 상관없이 상황을 알수 있도록 하기 위해 Firebase를 이용해 분만예정 및 난산위험과 젖소의 출산에 대한 정보를 받아서 애플리케이션을 통해 알림을 보낼 수 있도록 구현하였습니다.

  * **개선할 부분** : 젖소가 꼬리를 올린 형태에 대한 정확도가 부족하여 학습에 필요한 데이터를 추가로 수집하여야 한다. <br/><br/> Firebase를 통해 알림을 전송받을 때 지연시간이 존재하므로 추후 이를 개선하여야 한다. <br/><br/> 젖소의 꼬리를 올리는 행동이 얼마나 지속되어야 분만 예측이라 할수 있는지에 대한 정확한 연구도 진행되어야 한다.<br/>
![](https://user-images.githubusercontent.com/95071769/210629375-2fa72cb6-76ec-4330-8e3d-8409f0ed7133.gif)



<br/>
<br/>

### [E-S 시스템](https://github.com/chae0328/YOLOv4_darknet_ES_System.git)
* **골절기에 의한 손 부상을 방지하기 위한 시스템**
* 산업 근로자들의 안전을 개선하기 위한 프로젝트
* 개발기간
  * 2021.04 ~ 2021.09
* 역할
  * **Darknet 프레임워크를 사용한 학습 진행** <br/><br/> YOLO-mark2를 이용하여 손 데이터를 라벨링하여 C언어 기반의 DarkNet 프레임워크를 사용하여 데스크탑에서 학습을 진행하였습니다.

  * **Jetson Nano 보드에 YOLOv4-tiny 적용** <br/><br/> 골절기의 경우 주로 산업현장이나 공장에서 자주 사용되므로 데스크탑 처럼 부피가 큰 컴퓨터는 효율성이 떨어집니다. 따라서 부피에 부담이 적고 딥 러닝을 구현하는데 최적화된 소형 컴퓨터인 Jetson Nano 보드를 이용하였습니다. <br/><br/> Jetson Nano 보드에 YOLOv4-tiny를 적용하여 사람의 손과 골절기의 칼날을 인식할 수 있도록 시스템을 구성하였습니다.

  * **손과 골절기 칼날의 거리에 의한 골절기 정지 시스템 구현** <br/><br/> Jetson Nano 보드를 통하여 인식된 손이 칼날과 가까워지게되면 자동으로 칼날이 정지될 수 있도록 시스템을 구현하였습니다.

  * **개선할 부분** : 객체 탐지를 할때 배경에 따라 정확도가 낮게 나오는 경향을 개선할 필요가 있고, Jetson Nano 보드보다 가벼운 보드에도 원활히 실행될 수 있도록 경량화를 시킬 필요가 있다.<br/>
![](https://user-images.githubusercontent.com/95071769/210629246-be9a924a-355a-45cf-bc2a-b4cd93841aac.gif)


<br/>
<br/>

## Prizes

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

## Thesis

* **[얼굴형 분석에 따른 맞춤 헤어스타일 합성 시스템 구현](https://drive.google.com/file/d/1JaSaX93qrTxa_MoR6r2zn5xS8wiJwW8T/view?usp=sharing)**
  * 일시 : 2022.12.02
  * 주최기관 : 한국산업정보학회

* **[객체 알고리즘을 활용한 젖소 분만 예정 탐지 및 난산 손실 예방 시스템](https://drive.google.com/file/d/16_rhO98BP18dDVhe6u2B2O9AGF2B-R-C/view?usp=sharing)**
  * 일시 : 2022.06.17
  * 주최기관 : 한국산업정보학회

* **[딥러닝 기반 젖소 꼬리 탐지 및 행동 분석](https://drive.google.com/file/d/1W_hA4Z9-mH4tZeSnDyQEr8B5-8OY1dSi/view?usp=sharing)**
  * 일시 : 2022.05.19
  * 주최기관 : 대한임베디드공학회
