# Docker

## Useful commands

### Run Docker Daemon

```bash
sudo dockerd &
```
 > *The & at the end runs the process in the background*

### List available docker images

```bash
docker images
```

### Remove an image

```bash
docker rmi <image_id>
```

### Show all running containers

```bash
docker ps -a
```

### Removes container from execution

```bash
docker rm <container_id>
```

### Run docker-compose.yaml file

```bash
docker compose up -d
```

### Run docker compose with a different file

```bash
docker compose [-f <filename>] up -d
```

### Reverting a docker compose up

```bash
docker compose down
```

### Start a container

```bash
docker start <container_id>
```

### Stop a container

```bash
docker stop <container_id>
```

### Run a container

```bash
docker run <container_id>
```

## Related Commands

### List ports in use (linux)

```bash
sudo ss -tulpn
```

### List running processes (linux)

```bash
ps -ef
```

### Kill a process (linux)

```bash
kill -9 <process_id>
```
