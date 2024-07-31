# PIXELLER

## 프로젝트 개요
메타버스에서 실시간으로 중고 물품의 상태를 확인하고 중고 거래 및 실시간 경매를 진행해보세요!

https://pixeller.net/

## 개발 기간
2024년 6월 24일 ~ 7월 27일 (약 5주)

## 기능 소개

- 2D 메타버스
- 화상 연결
- DM
- 경매

## 포스터

<img src="./img/POSTER.png" alt="POSTER">

## PIXELLER 메인 화면

<img src="./img/픽셀러 UI.png">

## 경매장

<img src="./img/경매장 사진.png">

## 시스템 아키텍쳐

<img src="./img/Mixed Architecture.png">

## 참여 역할
> 저희 프론트 팀은 일 별로 구현할 메인 기능을 가져가고, 1주일 단위로 각종 버그, 마이너 이슈들과 기능들을 가져가며 개발에 임했습니다. 

### Fact that I did
- 경매 기능
- 유저간 위치 동기화

### Lesson that I learn
- nest.js 사용법
- CORS 해결방안
- Google OAUTH, JWT 토큰 인증, 인터셉터에 대한 개념

### 소스 트리 구조

```
src
│  app.controller.ts
│  app.module.ts
│  app.service.ts
│  main.ts
│
├─auction
│  │  auction.controller.spec.ts
│  │  auction.controller.ts
│  │  auction.gateway.spec.ts
│  │  auction.gateway.ts
│  │  auction.module.ts
│  │  auction.service.spec.ts
│  │  auction.service.ts
│  │
│  ├─dto
│  │      auction.dto.ts
│  │
│  ├─entity
│  │      auction.entity.ts
│  │
│  └─interfaces
│          auction.interface.ts
│
├─auth
│      AtStrategy.ts
│      auth.controller.spec.ts
│      auth.controller.ts
│      auth.module.ts
│      auth.service.ts
│      JwtWsInterceptor.ts
│      RtStrategy.ts
│
├─chat
│  │  chat.module.ts
│  │
│  └─chat
│          chat.gateway.ts
│
├─user
│  │  user.controller.ts
│  │  user.module.ts
│  │  user.service.ts
│  │
│  ├─dto
│  │      login-user.dto.ts
│  │
│  └─entity
│          user.entity.ts
│
└─util
        cryptoHandler.ts
        globalInterceptor.ts
```

## 기술 스택
## Front End

[![Phaser](https://img.shields.io/badge/Phaser-3.55.2-FAA61A?style=flat&logo=phaser)](https://phaser.io/)
[![React](https://img.shields.io/badge/React-17.0.2-61DAFB?style=flat&logo=react)](https://reactjs.org/)

## Back End

[![Nest.js](https://img.shields.io/badge/Nest.js-7.6.15-E0234E?style=flat&logo=nestjs)](https://nestjs.com/)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-2.5.4-6DB33F?style=flat&logo=springboot)](https://spring.io/projects/spring-boot)
[![RabbitMQ](https://img.shields.io/badge/RabbitMQ-3.8.16-FF6600?style=flat&logo=rabbitmq)](https://www.rabbitmq.com/)

## Database

[![AWS RDS: MySQL](https://img.shields.io/badge/AWS%20RDS-MySQL-527FFF?style=flat&logo=amazonaws)](https://aws.amazon.com/rds/)

## Object Storage

[![AWS S3](https://img.shields.io/badge/AWS%20S3-569A31?style=flat&logo=amazonaws)](https://aws.amazon.com/s3/)

## 통신

[![Socket.io](https://img.shields.io/badge/Socket.io-4.1.2-010101?style=flat&logo=socket.io)](https://socket.io/)
[![STOMP](https://img.shields.io/badge/STOMP-1.2-010101?style=flat&logo=stomp)](https://stomp.github.io/stomp-specification-1.2.html)
[![HTTPS](https://img.shields.io/badge/HTTPS-2.0-0058B0?style=flat&logo=https)](https://developer.mozilla.org/ko/docs/Web/HTTP/HTTPS)
[![OpenVidu](https://img.shields.io/badge/OpenVidu-2.17.0-3A3A3A?style=flat&logo=openvidu)](https://openvidu.io/)
[![Livekit](https://img.shields.io/badge/Livekit-1.2-8D8D8D?style=flat&logo=livekit)](https://docs.livekit.io/)

## CI/CD

[![Github](https://img.shields.io/badge/Github-Actions-181717?style=flat&logo=github)](https://github.com/features/actions)
[![AWS CodeDeploy](https://img.shields.io/badge/AWS%20CodeDeploy-527FFF?style=flat&logo=amazonaws)](https://aws.amazon.com/codedeploy/)

## Secure

[![AWS WAF](https://img.shields.io/badge/AWS%20WAF-527FFF?style=flat&logo=amazonaws)](https://aws.amazon.com/waf/)
[![AWS Shield](https://img.shields.io/badge/AWS%20Shield-527FFF?style=flat&logo=amazonaws)](https://aws.amazon.com/shield/)


## 팀원 소개

|이름   |역할               |Github                             |
|-------|------------------|-----------------------------------|
|류강현 |Leader,Frontend    |https://github.com/ryyugang        |
|김수민 |Backend            |https://github.com/kssumin         |
|민사빈 |Backend            |https://github.com/sabinKrafton    |
|최우성 |Frontend           |https://github.com/wooseong-choi   |
|최재혁 |Frontend           |https://github.com/Digit24-dev     |

## 프로젝트 산출물

- Trello
    - https://trello.com/b/VUpxKJBd/namanmu

## 시연 영상
[![Video Label](http://img.youtube.com/vi/awCNAZ6LixU/0.jpg)](https://youtu.be/awCNAZ6LixU)

## 실행 방법

React: `npm start`
NestJS: `nest start`
Spring:
(DB 별도 구축 필요)