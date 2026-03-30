# Task 2 - Docker and Containers

This task containerizes the provided Python script from `adhwaithAS/shipyard-docker-task`.

## Files

- `script.py` - the original Python script
- `Dockerfile` - builds a lightweight Python image
- `.dockerignore` - keeps the build context small

## Build the image

```powershell
docker build -t shipyard-task2 .
```

## Run the container

```powershell
docker run --name shipyard-task2-container shipyard-task2
```

The container prints `Hello World` every 5 seconds after startup.

To run it in the background and inspect logs:

```powershell
docker run -d --name shipyard-task2-container shipyard-task2
docker logs -f shipyard-task2-container
```
