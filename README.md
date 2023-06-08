![Tests](https://github.com/TikTokTechImmersion/assignment_demo_2023/actions/workflows/test.yml/badge.svg)
# TikTok Tech Immersion 2023 (Backend) Assignment

### Assignment Task
Design and Develop an Instant Messaging System implementing a set of specific APIs using Golang. 

### Architecture
The system contains:
* HTTP server
* RPC server
* Redis (Data Storage)
<br>
![whiteboard_exported_image](https://github.com/dannweeeee/TikTok-Tech-Immersion-2023-Assignment/assets/42776950/5fb1f573-85ba-4ae0-b1bf-7fe105dc3c92)


### Additional Feature
* Created a multi-module workspace to simplify dependency management controlled by a `go.work` file in the root directory.

## Introduction
This is a submission of the TikTok Tech Immersion 2023 Backend Assignment. <br>
Code base is based upon the [demo template](https://github.com/TikTokTechImmersion/assignment_demo_2023). <br>
<br>
NOTE: This assignment is only focused on the development of the backend side of the system, with any frontend features.

## Tools Used
* Golang
* Docker
* Redis

## Setup Instructions
Run the following command in the same directory as `docker-compose.yml` to initialise docker containers:
```bash
docker compose up
```
