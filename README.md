![Tests](https://github.com/TikTokTechImmersion/assignment_demo_2023/actions/workflows/test.yml/badge.svg)
# TikTok Tech Immersion 2023 (Backend) Assignment

Task: Design and develop an Instant Messaging system implementing a set of specific APIs using Golang. 

## Introduction
This is a submission of the TikTok Tech Immersion 2023 Backend Assignment. <br>
Code base is based upon the [demo template](https://github.com/TikTokTechImmersion/assignment_demo_2023).

### Setup Instructions
Run the following command in the same directory as `docker-compose.yml`:
```bash
docker compose up -d
```

### To Send Messages
Send a `POST` request to `localhost:808-/api/send`
```bash
curl -X POST 'localhost:8080/api/send?chat=a:b&sender=a&text=hello'
```

### To Retrieve Messages
Send a `GET` request to `localhost:8080/api/pull`
```bash
curl 'localhost:8080/api/pull?chat=a:b&reverse=false'
```

### Additional Changes:
* Created a multi-module workspace.
* Compatible MySQL database for Linux platforms.