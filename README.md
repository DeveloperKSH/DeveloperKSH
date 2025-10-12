# 👋 안녕하세요, **김상현** 입니다!

로봇 소프트웨어 엔지니어로서 **실내/실외 자율주행**, **멀티로봇 관제 아키텍처** 분야에 관심을 가지고 프로젝트를 진행하고 있습니다.  
현장에서 직접 구동계/센서 하드웨어를 다루고, ROS2 및 시뮬레이션을 통해 **실제 적용 가능한 로보틱스 솔루션**을 구현하는 데 집중하고 있습니다.  

---

## 🛠 Tech Stack

- **Languages**  
  ![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)  
  ![C++](https://img.shields.io/badge/C++-00599C?style=flat&logo=c%2B%2B&logoColor=white)

- **Robotics / Simulation**  
  ![ROS2](https://img.shields.io/badge/ROS2-Foxglove?style=flat&logo=ros&logoColor=white)  
  ![Nav2](https://img.shields.io/badge/Nav2-00BFFF?style=flat)  
  ![OpenRMF](https://img.shields.io/badge/Open--RMF-22314E?style=flat)  
  ![Gazebo](https://img.shields.io/badge/Gazebo-orange?style=flat)

- **Others**  
  ![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)  
  ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)  
  ![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=flat&logo=ubuntu&logoColor=white)  

---

## 📌 Featured Projects

### 🚚 배달로봇 자율주행 & 다중 로봇 관제 (실외)
- **기간:** 2024.05 ~ 2025.01 (8개월)  
- **성과:** 한동대 캠퍼스 시범 서비스에서 배달 소요 시간 **30% 단축** (15분 40초 -> 11분), 사고 발생률 **75% 감소** (20% -> 5%)  
- **기술:** Python, C++, ROS2, Nav2, Open-RMF, Gazebo, API, Docker  
- **주요 기여:**  
  - Nav2 핵심 플러그인(Planner, Controller, BT) 운영 및 파라미터 최적화로 실외 주행 안정화  
  - 상위 FSM으로 주행 상태를 관리해 주행 취소, 정지, 변경, 재개 과정을 절차화하고 텔레메트리로 상태를 실시간 공유  
  - Open-RMF 기반 관제 구조와 플릿 연동을 설계하고, RMF 작업/경로를 FSM으로 관리해 Nav2 액션으로 실행하는 로봇 클라이언트 아키텍처를 구축  
  - RMF Core와 Traffic Editor 연계로 웨이포인트 운영 규칙을 체계화하고, 구간 속도, 대기 지점, 우선순위, 안전 거리 기준을 맵에 반영  
  - 한국 좌표계(EPSG 계열) 변환을 통해 구글 위성 타일을 Traffic Editor와 RViz Satellite에 적용해 편집 맵과 현장 간 오차 해소, 모니터링 효과 극대화  
  - Gazebo 시뮬레이션으로 사전 검증을 수행한 후 단계적 현장 적용 절차를 통해 운영 리스크 최소화
  - 로그 지표화를 바탕으로 지속적 성능 개선 프로세스 정립에 기여
  - Docker로 배달로봇 및 관제서버를 컨테이너화하고 서비스별 실행 가이드를 정리해 온보딩 시간을 단축  
- 🔗 [배달로봇](https://github.com/DeveloperKSH/Open-RMF_DeliveryRobot) / [관제서버](https://github.com/DeveloperKSH/Open-RMF_Server)

---

### 🏭 물류로봇 자율주행 (실내)
- **기간:** 2025.02 ~ 2025.08 (6개월)  
- **성과:** RTK-GNSS 없이 LiDAR 기반 Localization을 안정화해 주행 오차 **40% 감소** (25cm -> 15cm), 협소 구간 완주율을 **90%로 향상**  
- **기술:** Python, C++, ROS2, SLAM, Nav2, Gazebo, Serial, API, Docker   
- **주요 기여:**  
  - 물류로봇의 구동부와 센서를 통합한 하드웨어 레이어를 설계해 Nav2, SLAM 등 상위 스택에 일관된 토픽/TF를 제공  
  - Odom과 IMU를 EKF로 융합해 map, odom, base_link TF 체인을 안정화하고 전방 180도 LiDAR의 시야 한계를 각도 구간별 필터링으로 보완   
  - Cartographer로 맵핑과 loop closure를 수행하고 운영은 AMCL Localization으로 정착, 라이다 시야 한계를 고려해 단계별 파라미터를 지속 조정  
  - Nav2 핵심 플러그인(Planner, Controller, BT) 운영 및 파라미터 최적화로 실내 협소 구간 주행 안정화
  - 상위 FSM으로 주행 상태를 관리해 주행 취소, 정지, 변경, 재개 과정을 절차화하고 텔레메트리로 상태를 실시간 공유
  - Gazebo 시뮬레이션으로 사전 검증을 수행한 후 단계적 현장 적용 절차를 통해 리스크 최소화
  - 로그 기반 운영 지표화를 통해 지속적인 성능 개선 체계 정립에 기여  
  - Docker로 bringup, slam, nav2를 컨테이너화하고 서비스별 실행 가이드를 마련해 온보딩 시간을 단축  
- 🔗 [물류로봇](https://github.com/DeveloperKSH/Indoor_LogisticsRobot)

---

## 📫 Contact & Links

- GitHub: https://github.com/DeveloperKSH
- Email: kim1836113@naver.com

---

⭐️ **꾸준히 배우고 실험하며, 실제 환경에 적용 가능한 로보틱스 솔루션을 만들어가는 엔지니어**가 되고자 합니다.
