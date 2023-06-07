![Tests](https://github.com/TikTokTechImmersion/assignment_demo_2023/actions/workflows/test.yml/badge.svg)
# TikTok Tech Immersion 2023 (Backend) Assignment

## Introduction
This is a submission of the TikTok Tech Immersion 2023 Backend Assignment.
Code base is based upon the [demo template](https://github.com/TikTokTechImmersion/assignment_demo_2023).

### Setup Instructions
Run the following command in the same directory as `docker-compose.yml` to initialise the necessary Docker containers:
```bash
docker compose up -d
```
### To Send Messages
Send a `POST` request to `localhost:8080/api/send`, specifying the following URL parameters:
* `chat`: Name of chat in the form `[USER A]:[USER B]`
* `sender`: Name of sender
* `text`: Text in message

Example:
```bash
curl -X POST 'localhost:8080/api/send?chat=a:b&sender=a&text=hi'
```

### To Pull Messages
Send a `GET` request to
`localhost:8080/api/pull`, specifying the following URL
parameters:
* `chat`: Name of chat in the form `[USER A]:[USER B]`
* `cursor`: Earliest epoch time of messages to retrieve, 0 by default
* `limit`: Maximum number of messages to retrieve, 10 by default
* `reverse`: Boolean value of whether to sort messages in ascending order by time

Example:
```bash
curl 'localhost:8080/api/pull?chat=a:b&cursor=0&limit=10&reverse=false'
```
