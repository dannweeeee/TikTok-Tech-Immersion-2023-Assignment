![Tests](https://github.com/TikTokTechImmersion/assignment_demo_2023/actions/workflows/test.yml/badge.svg)
# TikTok Tech Immersion 2023 (Backend) Assignment

Task: Design and develop an Instant Messaging system implementing a set of specific APIs using Golang. 

## Introduction
This is a submission of the TikTok Tech Immersion 2023 Backend Assignment. <br>
Code base is based upon the [demo template](https://github.com/TikTokTechImmersion/assignment_demo_2023).

### Setup Instructions
Run the following command in the same directory as `docker-compose.yml` to initialise the necessary Docker containers:
```bash
docker compose up -d
```

### To Send Messages
```bash
curl -X POST 'localhost:8080/api/send?chat=a:b&sender=a&text=hello'
```

### To Retrieve all Messages
```bash
curl 'localhost:8080/api/pull?chat=a:b&reverse=false'
```