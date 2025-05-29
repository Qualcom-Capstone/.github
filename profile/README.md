# <icon> Overspeed vehicle detection and alert system - with Qualcomm

<div align=center>
<img src="https://github.com/user-attachments/assets/cadc57b1-1806-4580-954d-ef898bd68f5f"/>
<h5>2025.03.20-2024.05.30</h5>
<h4>https://autonotify.store</h4>
<h2>실시간 과속탐지 및 알림 시스템</h2>
<h3>Rubik Pi 보드에서 YOLO 기반 객체 감지와 속도 측정을 통해 과속 차량을 탐지하고,<br>
서버로 정보를 전송해 실시간 알림까지 제공하는 스마트 교통 시스템</h3>
</div>
<br />



<h2>📖 Medium</h2>
https://medium.com/~~~
<br />
<br />

<h2>🖥️ Demo</h2>
<h3>시연 영상</h3>
https://www.youtube.com/watch?v=FDzbjOeika8

<h3>메인페이지(과속 차량 목록보기)</h3>
<img src="https://github.com/user-attachments/assets/812776f4-7dfe-4638-9ca1-0b6490662785" width="70%" >
<h3>과속 차량 개별 보기</h3>
<img src="https://github.com/user-attachments/assets/5c0a0853-0a12-4578-bc16-22947f388412" width="70%">
<h3>알림 확인하기</h3>
<img src="https://github.com/user-attachments/assets/c8415375-8a53-45be-b3bb-a0e9a2b20437" width="70%">



<br />
<br />
<br />


<h2>🏛️ System Architechture</h2>
<img src="https://github.com/user-attachments/assets/a08a74d6-340e-4ded-8cc3-6c6928831fda">
<br />
<br />

<h2>🛠️ Tech Stack</h2>
<div align=center>
<h4>Frontend</h4>
<img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=white">
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white">
<img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white">
<img src="https://img.shields.io/badge/Prettier-F7B93E?style=for-the-badge&logo=prettier&logoColor=white">
<img src="https://img.shields.io/badge/Axios-5A29E4?style=for-the-badge&logo=Axios&logoColor=white">

<br />
<br />
<h4>Backend</h4>
<img src="https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white">
<img src="https://img.shields.io/badge/Gunicorn-499848?style=for-the-badge&logo=gunicorn&logoColor=white">
<img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white">
<img src="https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white">
<img src="https://img.shields.io/badge/Celery-37814A?style=for-the-badge&logo=celery&logoColor=white">


<br />
<br />
<h4>Infra</h4>
<img src="https://img.shields.io/badge/Amazon EC2-FF9900?style=for-the-badge&logo=amazonec2&logoColor=white"/>
<img src="https://img.shields.io/badge/Amazon RDS-527FFF?style=for-the-badge&logo=amazonrds&logoColor=white"/>
<img src="https://img.shields.io/badge/Amazon S3-569A31?style=for-the-badge&logo=amazons3&logoColor=white"/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white">
<img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white">
<img src="https://img.shields.io/badge/Traefik-24A1C1?style=for-the-badge&logo=traefikproxy&logoColor=white">
<img src="https://img.shields.io/badge/Portainer-13BEF9?style=for-the-badge&logo=portainer&logoColor=white">


<br />
<br />
<h4>etc</h4>
<img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white">
<img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white">
<img src="https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=slack&logoColor=white">
<img src="https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=notion&logoColor=white">
<img src="https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white">
<img src="https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white">
<img src="https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=white">
<br />
<br />
</div>

<br />

<h2>Notification System Design</h2>

<h4>Django - RabbitMQ - Celery - FCM(3rd party Service) feat. Ack & Nack</h4>
<img src="https://github.com/user-attachments/assets/671d75ad-a1ab-441e-8159-f55080f38cb4">
<h4>Dead Letter Queue & Dead Letter Consumer</h4>
<img src="https://github.com/user-attachments/assets/75dc90c3-89d8-435b-a36e-5addbeaaf3ce">



<h4>reference</h4>  

- System Deisgn interview (Alex Xu)
- <a href="https://youtu.be/uk5fRLUsBfk?si=n6--PVE2CH4pQt_4">분산 시스템에서 데이터를 전달하는 효율적인 방법 - nhn 김병부</a>

<h2>Rubik Pi 3</h2>
Qualcomm 기반 Rubik Pi 하드웨어에서 YOLO 객체 탐지와 GStreamer를 활용해,
실시간으로 과속 차량을 감지하는 완전한 엣지 기반 시스템.
카메라 입력부터 추론, 트래킹, 속도 측정, 과속 차량 촬영까지 모든 과정을 로컬에서 처리하므로 클라우드 연산 불필요.

## Rubik Tech Stack

| Category             | Technologies                                                    |
|----------------------|-----------------------------------------------------------------|
| **Hardware**         | Rubik Pi 3, IMX477 image sensor, 10MP HQ Lens(16mm)             |
| **Object Detection** | YOLOv5m                                                         |
| **Acceleration**     | Qualcomm SNPE + TFLite delegate                                 |
| **Pipeline**         | GStreamer                                                       |
| **Programming**      | Python                                                          |
| **Features**         | On-device tracking, speed measurement, snapshot, multithreading |

## Object Tracking (IoU)

<img src="https://github.com/user-attachments/assets/868437d2-78e2-4d52-89a7-3d7f9e850517" width="300" height="200">

IoU를 계산하여, 다음프레임의 객체가 같은 객체인지 판단

## Speed Measurement

### Method 1 (Not Used)

<img src="https://github.com/user-attachments/assets/9980f43f-7990-47aa-a222-8e350e34666c" width="300" height="200">

프레임간 중심 좌표의 이동거리 변화로 속도를 측정

### Method 2 (✅Selected)

<img src="https://github.com/user-attachments/assets/e6d91e45-a950-47ad-8ef3-96aa008875cb" width="300" height="200">

가상의 두 선을 그어놓고, 두 선을 동과하는데 걸리는 시간을 측정

하지만, 이 방법은 가상의 두 선 사이의 실제 도로 거리를 알아야 정확히 측정 가능

## Multi Threading

병목 현상을 최소화 하기 위해서 멀티 스레딩을 사용

+ 메인 스레드
+ 트래킹, 속도 측정 스레드
+ 사진촬영 및 전송 스레드

<br />
<br />

<h2>📁 API</h2>
<h3>Swagger</h3>
<img src="https://github.com/user-attachments/assets/32f4389e-ef31-4ce1-b385-b369759a1f14">
<h3>Postman</h3>
<img src="https://github.com/user-attachments/assets/d319a2ae-ee50-462e-8224-131d4656af48">

<br />

<h2>🔍 Monitoring</h2>
<h3>Portainer</h3>
<img src="https://github.com/user-attachments/assets/c587e391-3b48-410a-b6aa-8c118952cfcd">


<h3>RabbitMQ</h3>
<img src="https://github.com/user-attachments/assets/a40a7cbb-0922-4fc4-9de5-710ec1b71a76">

<h3>Flower(celery monitoring</h3>
<img src="https://github.com/user-attachments/assets/c0f44488-142a-4f3d-bbab-c64479ee3e75">

<br />
<h2>📓 How to Start</h2>

### Clone Repository

docker repository를 클론합니다.



<details>
  <summary>Frontend</summary>

### Install Packages

패키지 설치를 합니다.

  ```
  npm install
  ```

### Add Environment Files

환경 파일을 생성해 줍니다.

#### .env

  ```
  VITE_API_BASE_URL=http://localhost:8000/api
  VITE_FIREBASE_API_KEY=YOUR_FIREBASE_API_KEY
  VITE_FIREBASE_AUTH_DOMAIN=YOUR_FIREBASE_AUTH_DOMAIN
  VITE_FIREBASE_PROJECT_ID=YOUR_FIREBASE_PROJECT_ID
  VITE_FIREBASE_STORAGE_BUCKET=YOUR_FIREBASE_STORAGE_BUCKET
  VITE_FIREBASE_MESSAGING_SENDER_ID=YOUR_SENDER_ID
  VITE_FIREBASE_APP_ID=YOUR_FIREBASE_APP_ID
  VITE_FIREBASE_VAPID_KEY=YOUR_FIREBASE_VAPID_KEY
  ```

### Getting Started

마지막으로 개발 서버를 열어줍니다.

  ```
  npm run dev
  ```

### See Result

http://localhost:5173 에 접속하여 결과물을 조회합니다.

</details>


<details>
  <summary>Backend</summary>

### Add Environment Files(.env)

**/.env**

  ```
  DATABASE_NAME= capstone
  DATABASE_USER= sa
  DATABASE_PASS= 1234
  DATABASE_HOST=
  DATABASE_PORT=
  SECRET_KEY=


  ```

  ```
  
  

  ```

### Docker Run Command

백엔드 서비스를 시작하기 위해 다음 Docker Compose 명령어를 실행합니다.

  ```bash
  docker-compose -p teaml -f Solomon-Docker/docker-compose.prod.yml up -d -—build
  ```

</details>
<br /> 
<!-- <h2>📂 Directory Structure</h2>

<br />
<br /> -->
<h2>Member</h2>

<table width="1000">
    <thead>
    </thead>
    <tbody>
    <tr>
        <th>Pictures</th>
         <td width="100" align="center">
            <a href="https://github.com/lsh1215">
                <img src="https://github.com/user-attachments/assets/5acaee97-6742-4f73-b47f-262cfdade814" width="80" height="80">
            </a>
        </td>
        <td width="100" align="center">
            <a href="https://github.com/Jminu">
                <img src="https://github.com/user-attachments/assets/27154e48-de61-4584-8309-3dab052b594d" width="80" height="80">
            </a>
        </td>
        <td width="100" align="center">
            <a href="https://github.com/choimh331">
                <img src="https://github.com/user-attachments/assets/aa6221bd-de3e-4926-8f98-ec0ecc1cbf72" width="80" height="80">
            </a>
        </td>
        <td width="100" align="center">
            <a href="https://github.com/Jeongchan-Seo">
                <img src="" width="80" height="80">
            </a>
        </td>
    </tr>
    <tr>
        <th>Name</th>
        <td width="100" align="center">이상훈</td>
        <td width="100" align="center">진민우</td>
        <td width="100" align="center">최명헌</td>
        <td width="100" align="center">서정찬</td>
    </tr>
    <tr>
        <th>Position</th>
        <td width="10" align="center">
            Leader<br>
            Backend<br>
            DevOps<br>
            Design<br/>
        </td>
        <td width="100" align="center">
            Rubik Pi<br>
            Tracking<br>
            Calculate<br>
            YOLO<br>
        </td>
        <td width="100" align="center">
            Backend<br>
        </td>
        <td width="100" align="center">
            Frontend<br>
        </td>
    </tr>
    <tr>
        <th>GitHub</th>
        <td width="100" align="center">
            <a href="https://github.com/lsh1215">
                <img src="http://img.shields.io/badge/lsh1215-green?style=social&logo=github"/>
            </a>
        </td>
        <td width="100" align="center">
            <a href="https://github.com/Jminu">
                <img src="http://img.shields.io/badge/Jminu-green?style=social&logo=github"/>
            </a>
        </td>
        <td width="100" align="center">
            <a href="https://github.com/choimh331">
                <img src="http://img.shields.io/badge/choimh331-green?style=social&logo=github"/>
            </a>
        </td>
        <td width="100" align="center">
            <a href="https://github.com/Jeongchan-Seo">
                <img src="http://img.shields.io/badge/Jeongchan-Seo-green?style=social&logo=github"/>
            </a>
        </td>
     </tr>
    </tbody>
</table>



<br />
<br />
