
### Comprehensive Docker Commands and Options

#### General Docker Commands

**`docker run`**
- `-d`: Run container in detached mode.
- `--name`: Specify a name for the container.
- `-p`: Map a port or range of ports.
- `-v`: Bind mount a volume.
- `-e`: Set an environment variable.
- `--rm`: Automatically remove the container when it exits.
- `-it`: Allocate a pseudo-TTY and keep STDIN open.

**`docker build`**
- `-t`: Tag the image.
- `--build-arg`: Pass a build-time variable.
- `--no-cache`: Build without using the cache.
- `-f`: Specify a Dockerfile location.

**`docker images`**
- `-a`: Show all images.
- `-q`: Only display image IDs.

**`docker ps`**
- `-a`: Show all containers.
- `-q`: Only display container IDs.

**`docker exec`**
- `-it`: Open an interactive terminal inside the container.
- `--env`: Set an environment variable.
- `--user`: Specify the username or UID.

#### Docker Debugging Commands

**`docker logs`**
- `--follow` or `-f`: Continuously stream the log output.
- `--tail <number>`: Output the last `<number>` lines of the log.
- `--since <timestamp>`: Show logs since a specific timestamp.
- `--timestamps` or `-t`: Show timestamps for each log entry.

**`docker inspect`**
- Provides detailed information on Docker objects in JSON format.
- `-f`, `--format`: Format the output using a Go template.

**`docker stats`**
- Displays a live stream of container(s) resource usage statistics.
- `--no-stream`: Show current statistics without streaming.

**`docker top`**
- Displays the running processes in a container.
- Accepts native `ps` options for detailed process information.

**`docker diff`**
- Shows changes in a container's filesystem since it was started.
- Lists added, deleted, or modified files.

**`docker exec`** (for debugging purposes)
- `-it`: Attach an interactive terminal to run diagnostic tools or shells inside the container.

**`docker network inspect`**
- Provides detailed information about a network.
- `-v`, `--verbose`: Display detailed information in verbose mode.

### Additional Commands for Debugging and Management

**`docker volume ls` / `docker volume inspect`**
- Useful for inspecting volumes and their mount points, aiding in debugging storage issues.

**`docker network ls` / `docker network inspect`**
- Helps in understanding and troubleshooting container networking.

**`docker stop`**
- `-t`: Specify the timeout for stopping.

**`docker rm` / `docker rmi`**
- `-f`: Force the removal.
- `-v`: Remove volumes associated with the container (`docker rm`).



