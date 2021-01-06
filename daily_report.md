# 작업 일지

1/4 Mon.
- jetbot 초기 설정 및 부팅  
<img src="https://user-images.githubusercontent.com/47997946/103622166-a30b5c80-4f79-11eb-8190-2c74340478f2.png" width="30%"></img>

- 무선랜 설치  
<img src="https://user-images.githubusercontent.com/47997946/103621726-fd57ed80-4f78-11eb-8f4f-111bc2bfbd92.png" width="30%"></img>
<br/>

1/5 Tue.
- jetbot ssh 연결 - [docker](https://jetbot.org/master/software_setup/docker.html)
- jetbot 동작 확인 (모터, 카메라)
- 문제점 : 배터리가 보드만 연결 시에는 작동하나 모터까지 연결할 경우 전원이 꺼짐.
- jetbot 예제들 공부
    1. 기본 동작 확인 : 바퀴의 움직임 확인
    2. 충돌 회피 (Collision avoidance) : 장애물이 있는 이미지와 없는 이미지 학습으로 장애물 피하기
    3. 물체 따라가기 (Object following) : 훈련된 이미지로 해당 물체 따라가게 함
    4. 길 따라가기 (Line tracking) : 길이 주어졌을 때 갈 방향 학습시켜 길을 따라가게 함
- AWS DeepRacer tutorial 공부 : 트랙을 벗어나지 않으면 reward를 주는 방식으로 강화학습
- jetson community 프로젝트들을 살펴봄 - [link](https://developer.nvidia.com/embedded/community/jetson-projects)
    1. [open-source autocar](https://developer.nvidia.com/embedded/community/jetson-projects#autocar) : 컨트롤러로 jetbot이 움직일 때마다 화면, 이동 방향을 저장하여 학습
    2. 물체 인식 : 얼굴, 관절, 과일 등등
    3. [ROS NAVIBOT](https://developer.nvidia.com/embedded/community/jetson-projects#ros_navbot) : indoor mapping
    
<br/>

1/6 Wen.
- jetson community 프로젝트들을 이어서 살펴봄 - [link](https://developer.nvidia.com/embedded/community/jetson-projects)
    1. 물체 인식
          - [알파벳 sign language 인식](https://developer.nvidia.com/embedded/community/jetson-projects#sign_language_recognition)
          - [자동차 번호판 인식](https://developer.nvidia.com/embedded/community/jetson-projects#license_plate_recog)
          - [제스쳐 설명](https://developer.nvidia.com/embedded/community/jetson-projects#tsm_online) : 손을 인식해 취하고 있는 제스쳐에 대한 인식 및 설명
          - [pothole 인식](https://developer.nvidia.com/embedded/community/jetson-projects#ai_pothole_detector)
    2. 자율주행
          - [outdoor mapping](https://developer.nvidia.com/embedded/community/jetson-projects#panther)
          - [indoor mapping](https://developer.nvidia.com/embedded/community/jetson-projects#orbslam2_bebop2_nano) by 드론
          - [Traffic cone 피해 주행하기](https://developer.nvidia.com/embedded/community/jetson-projects#jetbot_traffic_cones) : 딥러닝모델(AlexNet)에 cone을 인식하게 하여 cone으로 길이 막혔을때 피해서 주행하게 함
          - [Self driving truck](https://developer.nvidia.com/embedded/community/jetson-projects#induction_charger_autonomous_truck) : jetbot으로 자율주행 구현
          
    3. IoT
        - [SHAIDES](https://developer.nvidia.com/embedded/community/jetson-projects#shaides) : AI와 IoT를 결합하여 앞에 보이는 전자기기를 컨트롤(on/off) 가능
    