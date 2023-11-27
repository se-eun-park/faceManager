# Face Manager. 
<br>

![7조  3기 7조 썸네일](https://github.com/AIVLE-School-Third-Big-Project/KT_BigProject_07/assets/88769484/57a2b84b-aa2c-4361-9cbc-14303313214d)

<br>
   
## Index
### Table of contents
1. [Service](#example)   
    - [❓  Face Manager Background](#-easymemd가-뭐예요)   
    - [🛠 기능 설명](#-기능-엿보기)
2. [Stack](#write-title-here!)   
3. [Members](#only-lowercase)   
3. [Demo Video](#use"-"instead-of-spacing-words)   

<br>

## ❓Background
<br>

> 외모가 중요시되는 현대 사회에서 사람들은 자신 얼굴의 단점은 보완하고 장점은 부각시키기 위해 화장을 잘하기 위해 노력한다. 화장을 잘하기 위해 유튜브, sns 등에서 정보를 습득한다. 그러나 오늘 날 우리가 쉽게 얻을 수 있는 화장에 대한 정보들은 아주 기초적이거나 개인의 얼굴 특징에 맞지 않고, 공유자의 얼굴 특징에 국한된 정보들이다. 전문 메이크업 샵에 가면 자신 얼굴에 맞는 화장법을 얻을 수 있지만 비용이 높은 편이고 시간도 제약이 있어 자신의 얼굴 이목구비 하나하나에 대한 화장법은 얻기에는 무리가 있다.


<br>


>그렇다고 성형외과에 찾아가 자신의 얼굴 특징에 대해 물어보고 그에 맞는 화장법을 찾는 것은 현실적으로 불가능하다. 이러한 이유로 본 프로젝트는 얼굴 인식 AI를 활용해 황금비율의 얼굴과 사용자의 얼굴을 비교하여 사용자의 얼굴 특징을 파악하고, 그에 맞는 화장법을 추천하는 시스템을 목표로 시작되었습니다. 또한 생성 AI를 활용해 추천한 화장법을 사용자의 얼굴에 입혀주고 입력받은 피부타입을 기반으로 화장품 추천 서비스까지 담고자 노력하였습니다.


<br>


## 🛠 Function 

1. 얼굴 특징 추출
    - 이목구비 특징
        - 사용자의 얼굴 사진을 입력받아 Dlib 라이브러리를 사용해 얼굴 랜드마크 좌표 추출
        - 랜드마크 좌표값의 차이, 각도를 활용해 얼굴 특징 추출
    - 얼굴형
        - EfficientNetB6 모델을 fine tuning하여 Oblong, Heart, Round, Oval, Square 5가지로 구분
2. 화장법 추천
    - 이목구비, 얼굴형 특징별로 조사해둔 화장법을 데이터베이스에 저장
    - AI를 활용해 얼굴 특징 파악 후 그에 맞는 화장법을 텍스트로 추천

3. 화장 이미지 생성
    - BeautyGEN 모델을 사용해 색조 화장 생성
    - 눈썹, 입술 등 면적과 관련한 화장은 Stable Diffusion의 image2image 모델을 활용해 생성

4. 화장품 추천
    - 유수분 밸런스, 피부 민감도, 멜라닌 색소 활성도, 피부 탄력도 및 주름 4가지의 피부타입을 입력받아 바우만 피부타입 16종으로 구분하여 그에 맞는 화장품 추천
   
<br>

![7조  3기 7조 소개이미지](https://github.com/AIVLE-School-Third-Big-Project/KT_BigProject_07/assets/88769484/bcc65f1b-7987-475e-8108-fb61abd45d97)

<br>
 
## Stacks
<img src="https://img.shields.io/badge/React-61DAFB.svg?style=for-the-badge&logo=React&logoColor=black"/><img src="https://img.shields.io/badge/JavaScript-F7DF1E.svg?style=for-the-badge&logo=JavaScript&logoColor=black"><img src="https://img.shields.io/badge/styledcomponents-DB7093.svg?style=for-the-badge&logo=styled-components&logoColor=white"/><br>
<img src="https://img.shields.io/badge/Django-092E20.svg?style=for-the-badge&logo=Django&logoColor=white"/><img src="https://img.shields.io/badge/Python-3776AB.svg?style=for-the-badge&logo=Python&logoColor=white"/><img src="https://img.shields.io/badge/TensorFlow-FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white">

<br>
  
## Demo Video
<img src="https://github.com/AIVLE-School-Third-Big-Project/KT_BigProject_07/assets/88769484/22e9dea5-5c6d-4aa4-912c-81c856cfcef0" style="width:400px" >
<br>   
