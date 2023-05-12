![뮤직큐 기능 포스터 (1)](https://user-images.githubusercontent.com/68101656/236461347-00b15cfd-f26a-4f3c-aad9-1f3e6dd78180.png)

[**🎥 시연 영상**](https://youtu.be/G2NeFoAerD0)

<br>

# 🏆 카카오 클라우드 스쿨 우수 프로젝트 수상

<br>

# 👨‍👨‍👧‍👧 팀원

| Name    | 손병주 (팀장)                                                                                                                                                                                                       | 이현범                                                                                                                                                                                                                  | 정솔리                                                                                                                                                                                                          | 정채윤                                                                                                                                                                                                        |
| ------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Profile | <img src="https://user-images.githubusercontent.com/68101656/236481819-45b72b74-8d7f-4d0f-b1f0-2822e11ae63c.png" alt="image" width="150" height="150"><br>💯 우리들의 선장님<br>🧠 올라운더<br>🎨 그림으로 설명해요 | <img src="https://user-images.githubusercontent.com/68101656/236480936-3061fe30-a60f-473c-b5da-6fe57ace7b31.png" alt="image" width="150" height="150"><br>🔑 인증/인가의 대가<br>😤 안되면 될때까지<br>🐯 헬스계의 티거 | <img src="https://user-images.githubusercontent.com/68101656/236482642-de9bc82a-fba0-4c01-bffb-a6282aa76c06.jpeg" alt="image" width="150" height="150"><br>😇 매니징 천사<br>💡 아이디어 뱅크<br>👥 소통이 체질 | <img src="https://user-images.githubusercontent.com/68101656/236482986-ecf63975-cc07-49e9-8b60-80cbf71c31ef.png" alt="image" width="150" height="150"><br>💬 코드리뷰 공주<br>👀 Docs Hunter<br>👑 Git 마스터 |
| Github  | [@byeongJoo05](https://github.com/byeongJoo05)                                                                                                                                                                      | [@hb9397](https://github.com/hb9397)                                                                                                                                                                                    | [@sollyj](https://github.com/SollyJ)                                                                                                                                                                            | [@kkkwp](https://github.com/kkkwp)                                                                                                                                                                            |

<br>

# 🧑‍💻 기술 스택

### 👉 Front-End

<img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
<img src="https://img.shields.io/badge/react-61DAFB?style=for-the-badge&logo=react&logoColor=black">

<details>
<summary>라이브러리📚</summary>
<div markdown="1">

react<br>
react-dom<br>
react-multi-select-component<br>
react-router<br>
react-router-dom<br>
react-scripts<br>
react-toastify<br>
react-youtube<br>
axios<br>
dotenv<br>
openvidu-browser<br>
emotion<br>
material-ui<br>
mui/material<br>
styled-components<br>

</div>
</details>

[Go to Repository](https://github.com/Dream-Kakao/MusicQ-Client.git)

### 👉 Back-End

<img src="https://img.shields.io/badge/SpringBoot-6DB33F?style=for-the-badge&logo=SpringBoot&logoColor=white">
<img src="https://img.shields.io/badge/mariaDB-003545?style=for-the-badge&logo=mariaDB&logoColor=white"> <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=Redis&logoColor=white">

<details>
<summary>Service단 라이브러리📚</summary>
<div markdown="1">

spring-boot-starter-web<br>
spring-boot-starter-mail<br>
spring-boot-starter-data-redis<br>
spring-boot-starter-validation<br>
spring-cloud-starter-aws<br>
spring-security-crypto<br>
openvidu-java-client<br>
lombok<br>
json<br>
jjwt<br>

</div>
</details>

[Go to Repository](https://github.com/Dream-Kakao/MusicQ-Service.git)

<details>
<summary>Domain단 라이브러리📚</summary>
<div markdown="1">

spring-boot-starter-web<br>
spring-boot-starter-validation<br>
spring-boot-starter-data-jpa<br>
spring-boot-devtools<br>
mariadb-java-client<br>
json<br>
lombok<br>
querydsl<br>

</div>
</details>

[Go to Repository](https://github.com/Dream-Kakao/MusicQ-Domain.git)

### 👉 CI/CD

<img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=Kubernetes&logoColor=white">
<img src="https://img.shields.io/badge/docker-2496ED?style=for-the-badge&logo=docker&logoColor=white">
<img src="https://img.shields.io/badge/githubactions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white">
<img src="https://img.shields.io/badge/argo-EF7B4D?style=for-the-badge&logo=argo&logoColor=white">
<img src="https://img.shields.io/badge/nginx-009639?style=for-the-badge&logo=nginx&logoColor=white">

<br>

# 🎨 서비스 아키텍처

<img width="705" alt="아키텍처-service+domain" src="https://user-images.githubusercontent.com/68101656/236461790-9244d16d-ee41-4d3c-91e0-c46c88a9cf7b.png">

### `하이브리드 클라우드 아키텍처` 적용

- 유저들의 정보 등이 담겨 있는 RDBMS와 이 DB에서 데이터를 전처리하는 도메인 로직만 가지고 있는 MusicQ-Domain WAS를 Private한 공간에 배치
- 실제 유저들에게 서비스를 제공할 배포환경에는 Client Server 와 서비스 로직을 가지고 있는 MusicQ-Service WAS를 배치
- WebRTC를 통한 비디오, 마이크 스트림을 위해 Openvidu Deployment Server를 배치
- AccessToken 관리를 위한 Redis Container 배치

<br>

# 🔌 EC2 포트정리

| PORT | 이름                                            |
| ---- | ----------------------------------------------- |
| 443  | HTTPS                                           |
| 80   | HTTP - HTTPS 리다이렉트                         |
| 8443 | Openvidu                                        |
| 6379 | Redis                                           |
| 3306 | MariaDB                                         |
| 8080 | Service Spring Boot - Kubernetes Service Object |
| 81   | Domain Spring Boot                              |
| 3000 | React - Kubernetes Service Object               |

<br>

# ♻️ 배포 플로우

![아키텍처-CICD](https://user-images.githubusercontent.com/68101656/236461918-ce6eb66e-90bb-4cb0-8737-8af4d2d85013.png)

### CI

- FE, BE 레포지토리 Main 브랜치로 PR Merge가 되는 경우, Github Actions이 이를 감지하여 팀 계정 DockerHub로 Image를 Build 및 Push 한다. (Image Tag는 Commit ID로 설정)

### CD

- Kubernetes Object 자동 배포를 위한 Manifest Repository에 yml 파일에 새로운 Docker Image를 삽입한다.
- ArgoCD를 이용하여 Manifest Repository를 Webhook 하여 자동화 배포를 시작한다.

<br>

# 📄 Wiki

<table style="width:100%">
  <tr>
    <td><a href="https://github.com/Dream-Kakao/MusicQ/wiki/%EA%B8%B0%EB%8A%A5%EB%AA%85%EC%84%B8%EC%84%9C">기능 명세서</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/Dream-Kakao/MusicQ/wiki/Git-Convention">Git Convention</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/Dream-Kakao/MusicQ/wiki/Code-Convention">Code Convention</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/Dream-Kakao/MusicQ/wiki/Class-Diagram">Class Diagram</a></td>
  </tr>
  <tr>
    <td><a href="https://github.com/Dream-Kakao/MusicQ/wiki/3%EC%9B%94-3%EC%A3%BC%EC%B0%A8-%EC%8A%A4%ED%94%84%EB%A6%B0%ED%8A%B8-%ED%9A%8C%EC%9D%98">회의록</a></td>
  </tr>
</table>
