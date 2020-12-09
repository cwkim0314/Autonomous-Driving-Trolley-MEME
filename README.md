# Autonomous driving Trolley ⌜MEME⌟
## 딥러닝을 이용한 자율주행카트 ⌜미미⌟
본 프로젝트는 이화여자대학교 컴퓨터공학과 졸업프로젝트의 일환으로, 스타트 불사조(Phonix)팀입니다.
[Notion Link](https://bit.ly/3lN3iEF) / 
[GitHub Link](https://github.com/MEME-Phoenix)

### 문제 정의
1. 오프라인 매장의 매출 감소  
 오프라인 매장의 매출 감소에는 여러가지 이유가 있지만, 저희 팀은 그중 “오프라인 매장 사용은 힘이 들고 불편하다”는 문제점을 개선하고자 합니다. 저희 팀은 자율주행 카트 미미를 통해 오프라인 매장에서의 쇼핑 경험을 손쉬운, 편리한 경험이 되게 하고자합니다.
2. 기술적인 면에서 한계점에 봉착한 현 자율주행카트  
자율주행 스마트 카트를 오프라인 대형 마트에 도입하는데에는 비용적인 측면은 필수적으로 고려하기 마련입니다. 해당 대형마트에서만 사용 가능한 모델으로 맞춤제작되어 제작되므로, 카트의 가격이 나날이 치솟고 있습니다. 기술의 부족으로 나타나는 가격 상승은 곧 대형마트의 경영에 큰 타격을 입게 됩니다.
  
이에, 본 팀 불사조는
#### 반려동물처럼  해당 고객을 담당하는, 맞춤형 자율주행 스마트카트 MEME를 제안합니다.  
불사조팀의 미미는 마트 고객의 편의를 최우선으로하는 완벽한 쇼핑메이트입니다. 고객이 대형마트에서 쇼핑을 하는 동안, 미미는 반려동물처럼 해당 고객을 졸졸 따라다닙니다. 고객을 잃어버리는 경우에, 자동으로 찾아가서 쇼핑을 도와줍니다.

### 현재 진행 단계는?
#### 현재 본 팀 불사조는 기술 구현 단계 중에 있습니다. 다음 영상으로 진행단계를 확인할 수 있습니다.(해당 썸네일을 눌러주세요.)  

[![](http://img.youtube.com/vi/KcIz_Y_clhU/0.jpg)](http://www.youtube.com/watch?v=KcIz_Y_clhU ""). 

1. SW 알고리즘 | Object Tracking  
카메라 정보를 통해 화면에 해당 client를 찾아, 이를 tracking 하는 역할을 수행합니다. Object Detection 기술과 Tracking 기술을 합쳐 구현됩니다. Tracking 알고리즘은  위에서 나온 앞뒤 탐지 프레임 분석을 통해 자율 주행 카트를 사용하는 client를 정확히 탐지하게 됩니다. 이를 구현하기 위해 이미지 처리에 사용되는 Filter(칼만 필터과 헝가리안 필터 등)로 간단한 딥러닝 모델을 통해 구현하려 합니다.  

2. SW 알고리즘 | Wake up Word Detection
Wake up word를 통해 해당 client의 위치를 감지하는 기술을 의미합니다.

3. HW의 LiDAR 센서 | SLAM, Navigation 기능 구현  
하드웨어 부문은 크게 센서 부문과 이동 부문으로 나뉩니다.
 카메라를 사용한다고 해서 모든 장애물을 감지하고,  돌발상황을 예방할 수 없습니다 따라서 본 팀은 LiDAR Navigation client 센서의 기술을 통해 를 둘러싼 주변 환경을 완벽하게 인지하려 합니다. 장애물을 감지하고 client와의 적정거리를 유지하게 됩니다 이를 통해 고객을 졸졸 따라다닐 수 있는 자율주행 카트의 목적을 달성하게 됩니다.
이러한 기본적인 기능뿐만 아닌 센서의 LiDAR SLAM 기술을 통해 자율 주행 카트는 다양한 분야에서 의 확장 가능성을 가집니다 기술의 . SLAM Mapping 을 통해 매장 장소의 map을 형성하여 해당 카트의 위치까지 완벽히 파악/ 매장 장소를 완벽히 이해하여 다른 환경에서도 간단히 Mapping만 돌리면 바로 적용이 가능해지는 우위에 있습니다.

### 프로젝트 기술 소개 블로그  
- 한지수
    * [[졸업프로젝트 개요, 1탄 RNN] 딥러닝을 이용한 자율주행카트](https://jisuhan.tistory.com/entry/졸업프로젝트딥러닝을-이용한-자율주행카트)
    * [[졸업프로젝트 2탄, CNN] ResNet50 톺아보기: 구조와 코드 분석](https://jisuhan.tistory.com/entry/CNN-ResNet50-톺아보기-구조와-코드-분석)
    * [[졸업프로젝트 3탄, HW] turtlebot3로 SLAM, Navigation 구현(2020 Summer)](https://jisuhan.tistory.com/entry/turtlebot3로-SLAM-Navigation-구현하기)  

- 박지윤  
    * [[1탄] Yolo v3 를 이용한 인물 추적 프로젝트](https://yumissfortune.tistory.com/4)
    * [[2탄] Yolo v3 를 이용한 인물 추적 프로젝트](https://yumissfortune.tistory.com/5)

- 김채원  
    * [[IT/KR/Project] 자율 주행 카트를 만들어보자](https://blog.naver.com/cwkim0314/222156573981)
    * [[IT/KR] Object Detection - EfficientDet](https://blog.naver.com/cwkim0314/222156584109)
    * [[IT/KR/Project] Hardware: Alphabot2-pi](https://blog.naver.com/cwkim0314/222167401417)
    
### 현재까지의 수상기록
- 2020 캡스톤 디자인 경진대회 창업 아이디어 부문 우수상

### License
Copyright (c) 2020 MEME-Phoenix
See the file license.txt for copying permission. LICENSE를 참고하세요.
