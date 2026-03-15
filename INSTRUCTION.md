# Todo Django App

## Run MySQL container

Create volume:

```
docker volume create mysql-data
```

Run container:

```
docker run -d \
--name mysql-container \
-v mysql-data:/var/lib/mysql \
-p 3306:3306 \
<your_dockerhub>/mysql-local:1.0.0
```
---
## Run App container
```
docker run -p 8000:8000 <your_dockerhub>/todoapp:2.0.0
```
---

## Open Application

Open browser:
http://localhost:8000