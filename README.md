
* [Docker](#Docker)
  * [Commands](#essential-docker-commands)
  * [Dockerfile](#dockerfile)
  * [Example](#end-to-end-example)

# Docker
### 𝖶𝗁𝖺𝗍 𝗂𝗌 𝖣𝗈𝖼𝗄𝖾𝗋?
𝖣𝗈𝖼𝗄𝖾𝗋 𝗂𝗌 𝖺 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗂𝗓𝖺𝗍𝗂𝗈𝗇 𝗉𝗅𝖺𝗍𝖿𝗈𝗋𝗆 𝗍𝗁𝖺𝗍 𝖺𝗅𝗅𝗈𝗐𝗌 𝗍𝗈 𝗉𝗎𝗍 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇𝗌 𝖺𝗇𝖽 𝗍𝗁𝖾𝗂𝗋 𝖽𝖾𝗉𝖾𝗇𝖽𝖾𝗇𝖼𝗂𝖾𝗌 𝗂𝗇𝗍𝗈 𝗂𝗌𝗈𝗅𝖺𝗍𝖾𝖽, 𝗅𝗂𝗀𝗁𝗍𝗐𝖾𝗂𝗀𝗁𝗍 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌.
<𝖻𝗋>
𝖳𝗁𝖾𝗌𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 𝖼𝖺𝗇 𝗋𝗎𝗇 𝖼𝗈𝗇𝗌𝗂𝗌𝗍𝖾𝗇𝗍𝗅𝗒 𝖺𝖼𝗋𝗈𝗌𝗌 𝖽𝗂𝖿𝖿𝖾𝗋𝖾𝗇𝗍 𝖾𝗇𝗏𝗂𝗋𝗈𝗇𝗆𝖾𝗇𝗍𝗌, 𝗌𝗎𝖼𝗁 𝖺𝗌 𝖽𝖾𝗏𝖾𝗅𝗈𝗉𝗆𝖾𝗇𝗍, 𝗍𝖾𝗌𝗍𝗂𝗇𝗀, 𝖺𝗇𝖽 𝗉𝗋𝗈𝖽𝗎𝖼𝗍𝗂𝗈𝗇, 𝖾𝗇𝗌𝗎𝗋𝗂𝗇𝗀 𝗍𝗁𝖺𝗍 𝖺𝗇 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇 𝖻𝖾𝗁𝖺𝗏𝖾𝗌 𝗍𝗁𝖾 𝗌𝖺𝗆𝖾 𝗐𝖺𝗒 𝗋𝖾𝗀𝖺𝗋𝖽𝗅𝖾𝗌𝗌 𝗈𝖿 𝗍𝗁𝖾 𝗎𝗇𝖽𝖾𝗋𝗅𝗒𝗂𝗇𝗀 𝗂𝗇𝖿𝗋𝖺𝗌𝗍𝗋𝗎𝖼𝗍𝗎𝗋𝖾.

𝖣𝗈𝖼𝗄𝖾𝗋 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 𝗐𝗈𝗋𝗄 𝖻𝗒 𝗋𝗎𝗇𝗇𝗂𝗇𝗀 𝗈𝗇 𝗍𝗈𝗉 𝗈𝖿 𝗍𝗁𝖾 𝖣𝗈𝖼𝗄𝖾𝗋 𝖤𝗇𝗀𝗂𝗇𝖾, 𝗐𝗁𝗂𝖼𝗁 𝗎𝗌𝖾𝗌 𝗍𝗁𝖾 𝗁𝗈𝗌𝗍 𝗈𝗉𝖾𝗋𝖺𝗍𝗂𝗇𝗀 𝗌𝗒𝗌𝗍𝖾𝗆'𝗌 𝗄𝖾𝗋𝗇𝖾𝗅 𝖻𝗎𝗍 𝖺𝗅𝗅𝗈𝗐𝗌 𝖾𝖺𝖼𝗁 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗍𝗈 𝖻𝖾 𝗂𝗌𝗈𝗅𝖺𝗍𝖾𝖽, 𝗆𝖺𝗇𝖺𝗀𝖾 𝗂𝗍𝗌 𝗈𝗐𝗇 𝖽𝖾𝗉𝖾𝗇𝖽𝖾𝗇𝖼𝗂𝖾𝗌, 𝖺𝗇𝖽 𝖾𝗑𝖾𝖼𝗎𝗍𝖾 𝗂𝗇𝖽𝖾𝗉𝖾𝗇𝖽𝖾𝗇𝗍𝗅𝗒.

### Key Docker Concepts:
 - <kbd style='color:#cbb786'>**Images**:</kbd> Docker images are the building blocks of containers. They contain everything needed to run an application, including the code, runtime, system tools, and libraries.
 - <kbd style='color:#cbb786'>**Containers**:</kbd> Containers are instances of Docker images. They run in isolated environments and provide a consistent runtime environment for applications.
 - <kbd style='color:#cbb786'>**Docker Hub**:</kbd> Docker Hub is a repository for finding and sharing Docker images.

## Essential Docker Commands

- [docker build](#build)
- [docker run](#run)
- [docker ps](#ps)
- [docker start](#start)
- [docker stop](#stop)

---

### `docker build`

> [!NOTE]
>
> `𝚍𝚘𝚌𝚔𝚎𝚛 𝚋𝚞𝚒𝚕𝚍 [𝙾𝙿𝚃𝙸𝙾𝙽𝚂] 𝙿𝙰𝚃𝙷 | 𝚄𝚁𝙻`
>
>  - 𝖡𝗎𝗂𝗅𝖽𝗌 𝖺 𝖣𝗈𝖼𝗄𝖾𝗋 𝗂𝗆𝖺𝗀𝖾 𝖿𝗋𝗈𝗆 𝖺 𝖣𝗈𝖼𝗄𝖾𝗋𝖿𝗂𝗅𝖾. 𝖠 𝖣𝗈𝖼𝗄𝖾𝗋𝖿𝗂𝗅𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝗌 𝖺 𝗌𝖾𝗍 𝗈𝖿 𝗂𝗇𝗌𝗍𝗋𝗎𝖼𝗍𝗂𝗈𝗇𝗌 𝖿𝗈𝗋 𝖼𝗋𝖾𝖺𝗍𝗂𝗇𝗀 𝖺𝗇 𝗂𝗆𝖺𝗀𝖾 𝗍𝗁𝖺𝗍 𝗂𝗇𝖼𝗅𝗎𝖽𝖾𝗌 𝗍𝗁𝖾 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇, 𝗂𝗍𝗌 𝖽𝖾𝗉𝖾𝗇𝖽𝖾𝗇𝖼𝗂𝖾𝗌, 𝖺𝗇𝖽 𝗋𝗎𝗇𝗍𝗂𝗆𝖾 𝖾𝗇𝗏𝗂𝗋𝗈𝗇𝗆𝖾𝗇𝗍𝗌.
>
>  - Optional parameters
>    - `-𝚝, --𝚝𝚊𝚐` → 𝗇𝖺𝗆𝖾 𝖺𝗇𝖽 𝗈𝗉𝗍𝗂𝗈𝗇𝖺𝗅𝗅𝗒 𝖺 𝗍𝖺𝗀 𝗂𝗇 𝗍𝗁𝖾 '𝗇𝖺𝗆𝖾:𝗍𝖺𝗀' 𝖿𝗈𝗋𝗆𝖺𝗍
>    - `--𝚋𝚞𝚒𝚕𝚍-𝚊𝚛𝚐` → 𝗌𝖾𝗍 𝖻𝗎𝗂𝗅𝖽-𝗍𝗂𝗆𝖾 𝗏𝖺𝗋𝗂𝖺𝖻𝗅𝖾𝗌
>    - `--𝚗𝚘-𝚌𝚊𝚌𝚑𝚎` → 𝖽𝗈 𝗇𝗈𝗍 𝗎𝗌𝖾 𝖼𝖺𝖼𝗁𝖾 𝗐𝗁𝖾𝗇 𝖻𝗎𝗂𝗅𝖽𝗂𝗇𝗀 𝗍𝗁𝖾 𝗂𝗆𝖺𝗀𝖾
>    - `-𝚏, --𝚏𝚒𝚕𝚎` → 𝗇𝖺𝗆𝖾 𝗈𝖿 𝗍𝗁𝖾 𝖣𝗈𝖼𝗄𝖾𝗋𝖿𝗂𝗅𝖾 (𝖣𝖾𝖿𝖺𝗎𝗅𝗍 𝗂𝗌 𝖯𝖠𝖳𝖧/𝖣𝗈𝖼𝗄𝖾𝗋𝖿𝗂𝗅𝖾)
> 
>  - Example
>    - `𝚍𝚘𝚌𝚔𝚎𝚛 𝚋𝚞𝚒𝚕𝚍 -𝚝 {𝗂𝗆𝖺𝗀𝖾 𝗇𝖺𝗆𝖾}:{𝗍𝖺𝗀} -f Dockerfile .`

---

### `docker run`

> [!NOTE]
>
> `docker run [OPTIONS] IMAGE [COMMAND] [ARG...]`
>
>  - Creates a new container from a specified image and starts it. If the image is not available locally, Docker will attempt to pull it from the configured registry.
>
>  - Optional parameters
>    - `-d, --detach` Run container in background and print container ID.
>    - `--name` Assign a custom name to the container. If not specified, Docker generates a random name.
>    - `-p, --publish` Publish a container's port(s) to the host. Format: hostPort:containerPort.
>    - `-e, --env` Set environment variables. Format: VARIABLE=value.
>    - `--rm` Automatically remove the container when it exits. This is useful for not leaving behind any stopped containers.
>    - `-v, --volume` Mount a volume. Format: hostSrc:containerDest or just the volume name if using Docker volumes.
> 
>  - Example
>    - `docker run -d --name {container name} {image name}`

---

 ### `docker ps`

> [!NOTE]
>
> `docker ps [OPTIONS]`
>
>  - Lists containers. By default, it shows only running containers.
>
>  - Optional parameters
>     - `-a, --all`: Show all containers (default shows just running).
>     - `-q, --quiet`: Only display container IDs.
>     - `-f, --filter`: Filter the output based on conditions like status, id, name, etc.
> 
>  - Example
>     - `docker ps -a`

---

### `𝖽𝗈𝖼𝗄𝖾𝗋 𝗌𝗍𝖺𝗋𝗍`

> [!NOTE]
>
> `𝖽𝗈𝖼𝗄𝖾𝗋 𝗌𝗍𝖺𝗋𝗍 [𝖮𝖯𝖳𝖨𝖮𝖭𝖲] 𝖢𝖮𝖭𝖳𝖠𝖨𝖭𝖤𝖱 [𝖢𝖮𝖭𝖳𝖠𝖨𝖭𝖤𝖱...]`
>
>  - 𝖲𝗍𝖺𝗋𝗍𝗌 𝗈𝗇𝖾 𝗈𝗋 𝗆𝗈𝗋𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌.
>
>  - Optional parameters
>     - `-𝖺, --𝖺𝗍𝗍𝖺𝖼𝗁`: 𝖠𝗍𝗍𝖺𝖼𝗁 𝖲𝖳𝖣𝖮𝖴𝖳/𝖲𝖳𝖣𝖤𝖱𝖱 𝖺𝗇𝖽 𝖿𝗈𝗋𝗐𝖺𝗋𝖽 𝗌𝗂𝗀𝗇𝖺𝗅𝗌.
>     - `-𝗂, --𝗂𝗇𝗍𝖾𝗋𝖺𝖼𝗍𝗂𝗏𝖾`: 𝖠𝗍𝗍𝖺𝖼𝗁 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋'𝗌 𝖲𝖳𝖣𝖨𝖭.
> 
>  - Example
>     - `𝖽𝗈𝖼𝗄𝖾𝗋 𝗌𝗍𝖺𝗋𝗍 -𝖺 {𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗇𝖺𝗆𝖾 𝗈𝗋 𝖨𝖣}`

---

### `𝖽𝗈𝖼𝗄𝖾𝗋 𝗌𝗍𝗈𝗉`

> [!NOTE]
>
> `𝖽𝗈𝖼𝗄𝖾𝗋 𝗌𝗍𝗈𝗉 [𝖮𝖯𝖳𝖨𝖮𝖭𝖲] 𝖢𝖮𝖭𝖳𝖠𝖨𝖭𝖤𝖱 [𝖢𝖮𝖭𝖳𝖠𝖨𝖭𝖤𝖱...]`
>
>  - 𝖲𝗍𝖺𝗋𝗍𝗌 𝗈𝗇𝖾 𝗈𝗋 𝗆𝗈𝗋𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌.
>
>  - Example
>    - `𝖽𝗈𝖼𝗄𝖾𝗋 𝗌𝗍𝗈𝗉 {𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗇𝖺𝗆𝖾 𝗈𝗋 𝖨𝖣}`

---

### `𝖽𝗈𝖼𝗄𝖾𝗋 𝗋𝗆`

> [!NOTE]
>
> `𝖽𝗈𝖼𝗄𝖾𝗋 𝗋𝗆 [𝖮𝖯𝖳𝖨𝖮𝖭𝖲] 𝖢𝖮𝖭𝖳𝖠𝖨𝖭𝖤𝖱 [𝖢𝖮𝖭𝖳𝖠𝖨𝖭𝖤𝖱...]`
>
>  - 𝖱𝖾𝗆𝗈𝗏𝖾𝗌 𝗈𝗇𝖾 𝗈𝗋 𝗆𝗈𝗋𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌.
>
>  - Optional parameters
>     - `-𝖿, --𝖿𝗈𝗋𝖼𝖾`: 𝖥𝗈𝗋𝖼𝖾 𝗍𝗁𝖾 𝗋𝖾𝗆𝗈𝗏𝖺𝗅 𝗈𝖿 𝖺 𝗋𝗎𝗇𝗇𝗂𝗇𝗀 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 (𝗎𝗌𝖾𝗌 𝖲𝖨𝖦𝖪𝖨𝖫𝖫).
>     - `-𝗏, --𝗏𝗈𝗅𝗎𝗆𝖾𝗌`: 𝖱𝖾𝗆𝗈𝗏𝖾 𝗍𝗁𝖾 𝖺𝗌𝗌𝗈𝖼𝗂𝖺𝗍𝖾𝖽 𝗏𝗈𝗅𝗎𝗆𝖾𝗌 𝗐𝗂𝗍𝗁 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋.
> 
>  - Example
>     - `𝖽𝗈𝖼𝗄𝖾𝗋 𝗋𝗆 {𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗇𝖺𝗆𝖾 𝗈𝗋 𝖨𝖣}`
>     - `𝖽𝗈𝖼𝗄𝖾𝗋 𝗋𝗆 -𝖿 $(𝖽𝗈𝖼𝗄𝖾𝗋 𝗉𝗌 -𝖺 -𝗊)` 

---

> [!NOTE]
>
> `𝖽𝗈𝖼𝗄𝖾𝗋 𝗋𝗆𝗂 [𝖮𝖯𝖳𝖨𝖮𝖭𝖲] 𝖨𝖬𝖠𝖦𝖤 [𝖨𝖬𝖠𝖦𝖤...]`
>
>  - 𝖱𝖾𝗆𝗈𝗏𝖾𝗌 𝗈𝗇𝖾 𝗈𝗋 𝗆𝗈𝗋𝖾 𝗂𝗆𝖺𝗀𝖾𝗌 𝖿𝗋𝗈𝗆 𝗍𝗁𝖾 𝗅𝗈𝖼𝖺𝗅 𝗌𝗍𝗈𝗋𝖺𝗀𝖾. 𝖳𝗁𝗂𝗌 𝖼𝗈𝗆𝗆𝖺𝗇𝖽 𝗂𝗌 𝗎𝗌𝖾𝖽 𝗍𝗈 𝗆𝖺𝗇𝖺𝗀𝖾 𝗍𝗁𝖾 𝖽𝗂𝗌𝗄 𝗌𝗉𝖺𝖼𝖾 𝖻𝗒 𝖼𝗅𝖾𝖺𝗇𝗂𝗇𝗀 𝗎𝗉 𝗎𝗇𝗎𝗌𝖾𝖽 𝗂𝗆𝖺𝗀𝖾𝗌.
>
>  - **𝖨𝖬𝖠𝖦𝖤**: 𝖳𝗁𝖾 𝗂𝗆𝖺𝗀𝖾 𝖨𝖣, 𝗋𝖾𝗉𝗈𝗌𝗂𝗍𝗈𝗋𝗒, 𝗈𝗋 𝗍𝖺𝗀. 𝖸𝗈𝗎 𝖼𝖺𝗇 𝗌𝗉𝖾𝖼𝗂𝖿𝗒 𝗆𝗎𝗅𝗍𝗂𝗉𝗅𝖾 𝗂𝗆𝖺𝗀𝖾𝗌 𝗍𝗈 𝗋𝖾𝗆𝗈𝗏𝖾.
>
>  - Optional parameters
>     - `-𝖿, --𝖿𝗈𝗋𝖼𝖾`: 𝖥𝗈𝗋𝖼𝖾 𝗋𝖾𝗆𝗈𝗏𝖺𝗅 𝗈𝖿 𝗍𝗁𝖾 𝗂𝗆𝖺𝗀𝖾, 𝖾𝗏𝖾𝗇 𝗂𝖿 𝗂𝗍'𝗌 𝖻𝖾𝗂𝗇𝗀 𝗎𝗌𝖾𝖽 𝖻𝗒 𝗌𝗍𝗈𝗉𝗉𝖾𝖽 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 𝗈𝗋 𝗁𝖺𝗌 𝖽𝖾𝗉𝖾𝗇𝖽𝖾𝗇𝗍 𝖼𝗁𝗂𝗅𝖽 𝗂𝗆𝖺𝗀𝖾𝗌.
>     - `--𝗇𝗈-𝗉𝗋𝗎𝗇𝖾`: 𝖣𝗈 𝗇𝗈𝗍 𝗋𝖾𝗆𝗈𝗏𝖾 𝗎𝗇𝗍𝖺𝗀𝗀𝖾𝖽 𝗉𝖺𝗋𝖾𝗇𝗍𝗌.
> 
>  - Example
>     - `𝖽𝗈𝖼𝗄𝖾𝗋 𝗋𝗆𝗂 {𝗂𝗆𝖺𝗀𝖾 𝖨𝖣 𝗈𝗋 𝗋𝖾𝗉𝗈𝗌𝗂𝗍𝗈𝗋𝗒:𝗍𝖺𝗀}`

---

### `𝖽𝗈𝖼𝗄𝖾𝗋 𝗂𝗆𝖺𝗀𝖾`
𝖬𝖺𝗇𝖺𝗀𝖾𝗌 𝗂𝗆𝖺𝗀𝖾𝗌. 𝖳𝗁𝗂𝗌 𝗂𝗌 𝖺 𝗉𝖺𝗋𝖾𝗇𝗍 𝖼𝗈𝗆𝗆𝖺𝗇𝖽 𝖿𝗈𝗋 𝗌𝖾𝗏𝖾𝗋𝖺𝗅 𝗌𝗎𝖻𝖼𝗈𝗆𝗆𝖺𝗇𝖽𝗌 𝗎𝗌𝖾𝖽 𝗍𝗈 𝗆𝖺𝗇𝖺𝗀𝖾 𝗂𝗆𝖺𝗀𝖾𝗌 𝗂𝗇 𝖣𝗈𝖼𝗄𝖾𝗋.

`𝖽𝗈𝖼𝗄𝖾𝗋 𝗂𝗆𝖺𝗀𝖾 [𝖢𝖮𝖬𝖬𝖠𝖭𝖣]`

𝖲𝗈𝗆𝖾 𝖼𝗈𝗆𝗆𝗈𝗇 𝗌𝗎𝖻𝖼𝗈𝗆𝗆𝖺𝗇𝖽𝗌 𝗂𝗇𝖼𝗅𝗎𝖽𝖾:
- `𝗅𝗌`: 𝖫𝗂𝗌𝗍 𝗂𝗆𝖺𝗀𝖾𝗌.
- `𝗋𝗆`: 𝖱𝖾𝗆𝗈𝗏𝖾 𝗈𝗇𝖾 𝗈𝗋 𝗆𝗈𝗋𝖾 𝗂𝗆𝖺𝗀𝖾𝗌.
- `𝗉𝗎𝗅𝗅`: 𝖯𝗎𝗅𝗅 𝖺𝗇 𝗂𝗆𝖺𝗀𝖾 𝗈𝗋 𝖺 𝗋𝖾𝗉𝗈𝗌𝗂𝗍𝗈𝗋𝗒 𝖿𝗋𝗈𝗆 𝖺 𝗋𝖾𝗀𝗂𝗌𝗍𝗋𝗒.
- `𝗉𝗎𝗌𝗁`: 𝖯𝗎𝗌𝗁 𝖺𝗇 𝗂𝗆𝖺𝗀𝖾 𝗈𝗋 𝖺 𝗋𝖾𝗉𝗈𝗌𝗂𝗍𝗈𝗋𝗒 𝗍𝗈 𝖺 𝗋𝖾𝗀𝗂𝗌𝗍𝗋𝗒.
- `𝖻𝗎𝗂𝗅𝖽`: 𝖡𝗎𝗂𝗅𝖽 𝖺𝗇 𝗂𝗆𝖺𝗀𝖾 𝖿𝗋𝗈𝗆 𝖺 𝖣𝗈𝖼𝗄𝖾𝗋𝖿𝗂𝗅𝖾.

𝖤𝖺𝖼𝗁 𝗌𝗎𝖻𝖼𝗈𝗆𝗆𝖺𝗇𝖽 𝗁𝖺𝗌 𝗂𝗍𝗌 𝗈𝗐𝗇 𝗌𝖾𝗍 𝗈𝖿 𝗈𝗉𝗍𝗂𝗈𝗇𝗌 𝖺𝗇𝖽 𝗎𝗌𝖺𝗀𝖾.

**𝖤𝗑𝖺𝗆𝗉𝗅𝖾𝗌:**
- `𝖽𝗈𝖼𝗄𝖾𝗋 𝗂𝗆𝖺𝗀𝖾 𝗅𝗌` - 𝖫𝗂𝗌𝗍 𝖺𝗅𝗅 𝗂𝗆𝖺𝗀𝖾𝗌.
- `𝖽𝗈𝖼𝗄𝖾𝗋 𝗂𝗆𝖺𝗀𝖾 𝗋𝗆 {𝗂𝗆𝖺𝗀𝖾 𝖨𝖣 𝗈𝗋 𝗇𝖺𝗆𝖾:𝗍𝖺𝗀}` - 𝖱𝖾𝗆𝗈𝗏𝖾 𝖺 𝗌𝗉𝖾𝖼𝗂𝖿𝗂𝖼 𝗂𝗆𝖺𝗀𝖾.
- `𝖽𝗈𝖼𝗄𝖾𝗋 𝗂𝗆𝖺𝗀𝖾 𝗉𝗎𝗅𝗅 {𝗋𝖾𝗉𝗈𝗌𝗂𝗍𝗈𝗋𝗒:𝗍𝖺𝗀}` - 𝖯𝗎𝗅𝗅 𝖺𝗇 𝗂𝗆𝖺𝗀𝖾 𝖿𝗋𝗈𝗆 𝖺 𝗋𝖾𝗀𝗂𝗌𝗍𝗋𝗒.
- `𝖽𝗈𝖼𝗄𝖾𝗋 𝗂𝗆𝖺𝗀𝖾 𝗉𝗎𝗌𝗁 {𝗋𝖾𝗉𝗈𝗌𝗂𝗍𝗈𝗋𝗒:𝗍𝖺𝗀}` - 𝖯𝗎𝗌𝗁 𝖺𝗇 𝗂𝗆𝖺𝗀𝖾 𝗍𝗈 𝖺 𝗋𝖾𝗀𝗂𝗌𝗍𝗋𝗒.

---

### `𝖽𝗈𝖼𝗄𝖾𝗋 𝗂𝗆𝖺𝗀𝖾𝗌`
𝖫𝗂𝗌𝗍𝗌 𝖺𝗅𝗅 𝗅𝗈𝖼𝖺𝗅𝗅𝗒 𝗌𝗍𝗈𝗋𝖾𝖽 𝖣𝗈𝖼𝗄𝖾𝗋 𝗂𝗆𝖺𝗀𝖾𝗌. 𝖳𝗁𝗂𝗌 𝖼𝗈𝗆𝗆𝖺𝗇𝖽 𝗉𝗋𝗈𝗏𝗂𝖽𝖾𝗌 𝖺 𝗊𝗎𝗂𝖼𝗄 𝗐𝖺𝗒 𝗍𝗈 𝗌𝖾𝖾 𝗐𝗁𝖺𝗍 𝗂𝗆𝖺𝗀𝖾𝗌 𝖺𝗋𝖾 𝖺𝗏𝖺𝗂𝗅𝖺𝖻𝗅𝖾 𝗈𝗇 𝗒𝗈𝗎𝗋 𝗌𝗒𝗌𝗍𝖾𝗆.

`𝖽𝗈𝖼𝗄𝖾𝗋 𝗂𝗆𝖺𝗀𝖾𝗌 [𝖮𝖯𝖳𝖨𝖮𝖭𝖲] [𝖱𝖤𝖯𝖮𝖲𝖨𝖳𝖮𝖱𝖸[:𝖳𝖠𝖦]]`

- **𝖮𝗉𝗍𝗂𝗈𝗇𝖺𝗅 𝗉𝖺𝗋𝖺𝗆𝖾𝗍𝖾𝗋𝗌**
- `-𝖺, --𝖺𝗅𝗅`: 𝖲𝗁𝗈𝗐 𝖺𝗅𝗅 𝗂𝗆𝖺𝗀𝖾𝗌 (𝖽𝖾𝖿𝖺𝗎𝗅𝗍 𝗁𝗂𝖽𝖾𝗌 𝗂𝗇𝗍𝖾𝗋𝗆𝖾𝖽𝗂𝖺𝗍𝖾 𝗂𝗆𝖺𝗀𝖾𝗌).
- `-𝗊, --𝗊𝗎𝗂𝖾𝗍`: 𝖮𝗇𝗅𝗒 𝗌𝗁𝗈𝗐 𝗂𝗆𝖺𝗀𝖾 𝖨𝖣𝗌.
- `--𝖿𝗈𝗋𝗆𝖺𝗍`: 𝖯𝗋𝖾𝗍𝗍𝗒-𝗉𝗋𝗂𝗇𝗍 𝗂𝗆𝖺𝗀𝖾𝗌 𝗎𝗌𝗂𝗇𝗀 𝖺 𝖦𝗈 𝗍𝖾𝗆𝗉𝗅𝖺𝗍𝖾.
- `-𝖿, --𝖿𝗂𝗅𝗍𝖾𝗋`: 𝖥𝗂𝗅𝗍𝖾𝗋 𝗈𝗎𝗍𝗉𝗎𝗍 𝖻𝖺𝗌𝖾𝖽 𝗈𝗇 𝖼𝗈𝗇𝖽𝗂𝗍𝗂𝗈𝗇𝗌 𝗉𝗋𝗈𝗏𝗂𝖽𝖾𝖽.

**𝖤𝗑𝖺𝗆𝗉𝗅𝖾𝗌:**
- `𝖽𝗈𝖼𝗄𝖾𝗋 𝗂𝗆𝖺𝗀𝖾𝗌` - 𝖫𝗂𝗌𝗍 𝖺𝗅𝗅 𝗍𝗈𝗉-𝗅𝖾𝗏𝖾𝗅 𝗂𝗆𝖺𝗀𝖾𝗌, 𝗍𝗁𝖾𝗂𝗋 𝗋𝖾𝗉𝗈𝗌𝗂𝗍𝗈𝗋𝗒, 𝗍𝖺𝗀, 𝖨𝖣, 𝖼𝗋𝖾𝖺𝗍𝗂𝗈𝗇 𝗍𝗂𝗆𝖾, 𝖺𝗇𝖽 𝗌𝗂𝗓𝖾.
- `𝖽𝗈𝖼𝗄𝖾𝗋 𝗂𝗆𝖺𝗀𝖾𝗌 -𝖺` - 𝖫𝗂𝗌𝗍 𝖺𝗅𝗅 𝗂𝗆𝖺𝗀𝖾𝗌, 𝗂𝗇𝖼𝗅𝗎𝖽𝗂𝗇𝗀 𝗂𝗇𝗍𝖾𝗋𝗆𝖾𝖽𝗂𝖺𝗍𝖾 𝗂𝗆𝖺𝗀𝖾𝗌.
- `𝖽𝗈𝖼𝗄𝖾𝗋 𝗂𝗆𝖺𝗀𝖾𝗌 -𝗊` - 𝖫𝗂𝗌𝗍 𝗍𝗁𝖾 𝖨𝖣𝗌 𝗈𝖿 𝖺𝗅𝗅 𝗂𝗆𝖺𝗀𝖾𝗌.
- `𝖽𝗈𝖼𝗄𝖾𝗋 𝗂𝗆𝖺𝗀𝖾𝗌 --𝖿𝗈𝗋𝗆𝖺𝗍 "{{.𝖱𝖾𝗉𝗈𝗌𝗂𝗍𝗈𝗋𝗒}}:{{.𝖳𝖺𝗀}} {{.𝖲𝗂𝗓𝖾}}"` - 𝖫𝗂𝗌𝗍 𝗂𝗆𝖺𝗀𝖾𝗌 𝗐𝗂𝗍𝗁 𝖺 𝖼𝗎𝗌𝗍𝗈𝗆 𝖿𝗈𝗋𝗆𝖺𝗍 𝗌𝗁𝗈𝗐𝗂𝗇𝗀 𝗋𝖾𝗉𝗈𝗌𝗂𝗍𝗈𝗋𝗒, 𝗍𝖺𝗀, 𝖺𝗇𝖽 𝗌𝗂𝗓𝖾.
- `𝖽𝗈𝖼𝗄𝖾𝗋 𝗂𝗆𝖺𝗀𝖾𝗌 -𝖿 "𝖽𝖺𝗇𝗀𝗅𝗂𝗇𝗀=𝗍𝗋𝗎𝖾"` - 𝖫𝗂𝗌𝗍 𝖺𝗅𝗅 𝖽𝖺𝗇𝗀𝗅𝗂𝗇𝗀 𝗂𝗆𝖺𝗀𝖾𝗌 (𝗂𝗆𝖺𝗀𝖾𝗌 𝗐𝗂𝗍𝗁𝗈𝗎𝗍 𝗍𝖺𝗀𝗌).

---


## Dockerfile
𝖨𝗇 𝗌𝗎𝗆𝗆𝖺𝗋𝗒, 𝗍𝗁𝗂𝗌 𝖣𝗈𝖼𝗄𝖾𝗋𝖿𝗂𝗅𝖾 𝖽𝖾𝖿𝗂𝗇𝖾𝗌 𝖺 𝗆𝗎𝗅𝗍𝗂-𝗌𝗍𝖺𝗀𝖾 𝖻𝗎𝗂𝗅𝖽 𝗉𝗋𝗈𝖼𝖾𝗌𝗌 𝗐𝗁𝖾𝗋𝖾 𝗍𝗁𝖾 𝖿𝗂𝗋𝗌𝗍 𝗌𝗍𝖺𝗀𝖾 𝖻𝗎𝗂𝗅𝖽𝗌 𝗍𝗁𝖾 .𝖭𝖤𝖳 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇, 𝖺𝗇𝖽 𝗍𝗁𝖾 𝗌𝖾𝖼𝗈𝗇𝖽 𝗌𝗍𝖺𝗀𝖾 𝗉𝗋𝖾𝗉𝖺𝗋𝖾𝗌 𝖺 𝗅𝗂𝗀𝗁𝗍𝖾𝗋 𝗋𝗎𝗇𝗍𝗂𝗆𝖾 𝖾𝗇𝗏𝗂𝗋𝗈𝗇𝗆𝖾𝗇𝗍 𝗍𝗈 𝗋𝗎𝗇 𝗍𝗁𝖾 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇.

```dockerfile
FROM mcr.microsoft.com/dotnet/sdk:8.0 AS build-env
WORKDIR /App

COPY . ./

RUN dotnet restore

RUN dotnet publish -c Release -o out

FROM mcr.microsoft.com/dotnet/aspnet:8.0
WORKDIR /App
COPY --from=build-env /App/out .
ENTRYPOINT ["dotnet", "{service name}.dll"]
```

`𝖥𝖱𝖮𝖬 𝗆𝖼𝗋.𝗆𝗂𝖼𝗋𝗈𝗌𝗈𝖿𝗍.𝖼𝗈𝗆/𝖽𝗈𝗍𝗇𝖾𝗍/𝗌𝖽𝗄:𝟪.𝟢 𝖠𝖲 𝖻𝗎𝗂𝗅𝖽-𝖾𝗇𝗏` - 𝖳𝗁𝗂𝗌 𝗅𝗂𝗇𝖾 𝗂𝗌 𝗍𝖾𝗅𝗅𝗂𝗇𝗀 𝖣𝗈𝖼𝗄𝖾𝗋 𝗍𝗈 𝗎𝗌𝖾 𝗍𝗁𝖾 .𝖭𝖤𝖳 𝖲𝖣𝖪 𝗏𝖾𝗋𝗌𝗂𝗈𝗇 𝟪.𝟢 𝗂𝗆𝖺𝗀𝖾 𝖿𝗋𝗈𝗆 𝖬𝗂𝖼𝗋𝗈𝗌𝗈𝖿𝗍'𝗌 𝖢𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝖱𝖾𝗀𝗂𝗌𝗍𝗋𝗒 𝖺𝗌 𝗍𝗁𝖾 𝖻𝖺𝗌𝖾 𝗂𝗆𝖺𝗀𝖾 𝖿𝗈𝗋 𝗍𝗁𝖾 𝖻𝗎𝗂𝗅𝖽 𝗉𝗋𝗈𝖼𝖾𝗌𝗌.
- `𝖢𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝖱𝖾𝗀𝗂𝗌𝗍𝗋𝗒` - 𝖲𝗍𝗈𝗋𝖺𝗀𝖾 𝖿𝗈𝗋 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗂𝗆𝖺𝗀𝖾𝗌. 𝖨𝗇 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖾𝗑𝗍 𝗈𝖿 𝗍𝗁𝗂𝗌 𝖿𝗂𝗅𝖾: 𝖨𝗍 𝗂𝗌 𝖬𝗂𝖼𝗋𝗈𝗌𝗈𝖿𝗍'𝗌 𝗈𝗐𝗇 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗋𝖾𝗀𝗂𝗌𝗍𝗋𝗒 𝖽𝖾𝗌𝗂𝗀𝗇𝖾𝖽 𝗍𝗈 𝗉𝗋𝗈𝗏𝗂𝖽𝖾 𝖺 𝗀𝗅𝗈𝖻𝖺𝗅𝗅𝗒 𝖺𝗏𝖺𝗂𝗅𝖺𝖻𝗅𝖾 𝗌𝖾𝗋𝗏𝗂𝖼𝖾 𝖿𝗈𝗋 𝗉𝗎𝗅𝗅𝗂𝗇𝗀 𝖬𝗂𝖼𝗋𝗈𝗌𝗈𝖿𝗍'𝗌 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗂𝗆𝖺𝗀𝖾𝗌.
- `𝖠𝖲 𝖻𝗎𝗂𝗅𝖽-𝖾𝗇𝗏` - 𝖲𝖾𝗍 𝖺 𝗇𝖺𝗆𝖾 𝗍𝗈 𝗍𝗁𝗂𝗌 𝗌𝗍𝖺𝗀𝖾 𝗍𝗈 𝗎𝗌𝖾 𝗂𝗍 𝗅𝖺𝗍𝖾𝗋 𝗅𝗂𝗄𝖾 𝖺 𝗏𝖺𝗋𝗂𝖺𝖻𝗅𝖾.

`𝖶𝖮𝖱𝖪𝖣𝖨𝖱 /𝖠𝗉𝗉` - 𝖲𝖾𝗍𝗌 𝗍𝗁𝖾 𝗐𝗈𝗋𝗄𝗂𝗇𝗀 𝖽𝗂𝗋𝖾𝖼𝗍𝗈𝗋𝗒 𝗂𝗇𝗌𝗂𝖽𝖾 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗍𝗈 /𝖠𝗉𝗉. 𝖳𝗁𝗂𝗌 𝗂𝗌 𝗍𝗁𝖾 𝖽𝗂𝗋𝖾𝖼𝗍𝗈𝗋𝗒 𝗐𝗁𝖾𝗋𝖾 𝗒𝗈𝗎𝗋 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇'𝗌 𝖼𝗈𝖽𝖾 𝗐𝗂𝗅𝗅 𝗋𝖾𝗌𝗂𝖽𝖾 𝗐𝗂𝗍𝗁𝗂𝗇 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝖽𝗎𝗋𝗂𝗇𝗀 𝗍𝗁𝖾 𝖻𝗎𝗂𝗅𝖽 𝗉𝗋𝗈𝖼𝖾𝗌𝗌.

`𝖢𝖮𝖯𝖸 . ./` - 𝖢𝗈𝗉𝗂𝖾𝗌 𝖾𝗏𝖾𝗋𝗒𝗍𝗁𝗂𝗇𝗀 𝖿𝗋𝗈𝗆 𝗒𝗈𝗎𝗋 𝗉𝗋𝗈𝗃𝖾𝖼𝗍'𝗌 𝖿𝗈𝗅𝖽𝖾𝗋 (𝗐𝗁𝖾𝗋𝖾 𝗍𝗁𝖾 𝖣𝗈𝖼𝗄𝖾𝗋𝖿𝗂𝗅𝖾 𝗂𝗌 𝗅𝗈𝖼𝖺𝗍𝖾𝖽) 𝗂𝗇𝗍𝗈 𝗍𝗁𝖾 𝖼𝗎𝗋𝗋𝖾𝗇𝗍 𝗐𝗈𝗋𝗄𝗂𝗇𝗀 𝖽𝗂𝗋𝖾𝖼𝗍𝗈𝗋𝗒 𝗂𝗇𝗌𝗂𝖽𝖾 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 (*/𝖠𝗉𝗉*).

`𝖱𝖴𝖭 𝖽𝗈𝗍𝗇𝖾𝗍 𝗋𝖾𝗌𝗍𝗈𝗋𝖾` - 𝖤𝗑𝖾𝖼𝗎𝗍𝖾𝗌 𝗍𝗁𝖾 𝖽𝗈𝗍𝗇𝖾𝗍 𝗋𝖾𝗌𝗍𝗈𝗋𝖾 𝖼𝗈𝗆𝗆𝖺𝗇𝖽. 𝖳𝗁𝗂𝗌 𝖼𝗈𝗆𝗆𝖺𝗇𝖽 𝗅𝗈𝗈𝗄𝗌 𝖺𝗍 𝗍𝗁𝖾 .𝖭𝖤𝖳 𝗉𝗋𝗈𝗃𝖾𝖼𝗍 𝖿𝗂𝗅𝖾𝗌 𝗂𝗇 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝖺𝗇𝖽 𝖽𝗈𝗐𝗇𝗅𝗈𝖺𝖽𝗌 𝖺𝗇𝗒 𝖽𝖾𝗉𝖾𝗇𝖽𝖾𝗇𝖼𝗂𝖾𝗌 (*𝗅𝗂𝖻𝗋𝖺𝗋𝗂𝖾𝗌 𝖺𝗇𝖽 𝗉𝖺𝖼𝗄𝖺𝗀𝖾𝗌*) 𝗍𝗁𝖺𝗍 𝖺𝗋𝖾 𝗇𝖾𝖾𝖽𝖾𝖽 𝗍𝗈 𝖻𝗎𝗂𝗅𝖽 𝗍𝗁𝖾 𝗉𝗋𝗈𝗃𝖾𝖼𝗍.

`𝖱𝖴𝖭 𝖽𝗈𝗍𝗇𝖾𝗍 𝗉𝗎𝖻𝗅𝗂𝗌𝗁 -𝖼 𝖱𝖾𝗅𝖾𝖺𝗌𝖾 -𝗈 𝗈𝗎𝗍` - 𝖳𝗁𝗂𝗌 𝖼𝗈𝗆𝗆𝖺𝗇𝖽 𝖻𝗎𝗂𝗅𝖽𝗌 𝗒𝗈𝗎𝗋 .𝖭𝖤𝖳 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇 𝗂𝗇 𝗋𝖾𝗅𝖾𝖺𝗌𝖾 𝗆𝗈𝖽𝖾 (*𝗈𝗉𝗍𝗂𝗆𝗂𝗓𝖾𝖽 𝖿𝗈𝗋 𝗉𝗋𝗈𝖽𝗎𝖼𝗍𝗂𝗈𝗇*) 𝖺𝗇𝖽 𝗈𝗎𝗍𝗉𝗎𝗍𝗌 𝗍𝗁𝖾 𝖼𝗈𝗆𝗉𝗂𝗅𝖾𝖽 𝖿𝗂𝗅𝖾𝗌 𝗍𝗈 𝗍𝗁𝖾 *𝗈𝗎𝗍* 𝖽𝗂𝗋𝖾𝖼𝗍𝗈𝗋𝗒 𝗐𝗂𝗍𝗁𝗂𝗇 𝗍𝗁𝖾 */𝖠𝗉𝗉* 𝖽𝗂𝗋𝖾𝖼𝗍𝗈𝗋𝗒 𝗂𝗇 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋.
- `-𝖼 𝖱𝖾𝗅𝖾𝖺𝗌𝖾` - 𝖳𝗁𝖾 -𝖼 𝖱𝖾𝗅𝖾𝖺𝗌𝖾 𝗈𝗉𝗍𝗂𝗈𝗇 𝗌𝗉𝖾𝖼𝗂𝖿𝗂𝖾𝗌 𝗍𝗁𝖺𝗍 𝗍𝗁𝖾 𝖻𝗎𝗂𝗅𝖽 𝗌𝗁𝗈𝗎𝗅𝖽 𝖻𝖾 𝖽𝗈𝗇𝖾 𝗂𝗇 𝖱𝖾𝗅𝖾𝖺𝗌𝖾 𝖼𝗈𝗇𝖿𝗂𝗀𝗎𝗋𝖺𝗍𝗂𝗈𝗇, 𝗐𝗁𝗂𝖼𝗁 𝗂𝗌 𝗈𝗉𝗍𝗂𝗆𝗂𝗓𝖾𝖽 𝖿𝗈𝗋 𝗉𝖾𝗋𝖿𝗈𝗋𝗆𝖺𝗇𝖼𝖾.

`𝖥𝖱𝖮𝖬 𝗆𝖼𝗋.𝗆𝗂𝖼𝗋𝗈𝗌𝗈𝖿𝗍.𝖼𝗈𝗆/𝖽𝗈𝗍𝗇𝖾𝗍/𝖺𝗌𝗉𝗇𝖾𝗍:𝟪.𝟢` - 𝖠𝖿𝗍𝖾𝗋 𝖻𝗎𝗂𝗅𝖽𝗂𝗇𝗀 𝗍𝗁𝖾 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇, 𝗍𝗁𝗂𝗌 𝗅𝗂𝗇𝖾 𝗌𝗍𝖺𝗋𝗍𝗌 𝖺 𝗇𝖾𝗐 𝗌𝗍𝖺𝗀𝖾 𝗂𝗇 𝗍𝗁𝖾 𝖣𝗈𝖼𝗄𝖾𝗋𝖿𝗂𝗅𝖾. 𝖨𝗍 𝗎𝗌𝖾𝗌 𝗍𝗁𝖾 .𝖭𝖤𝖳 𝗋𝗎𝗇𝗍𝗂𝗆𝖾 𝗂𝗆𝖺𝗀𝖾 (*𝗇𝗈𝗍 𝗍𝗁𝖾 𝖲𝖣𝖪*) 𝗏𝖾𝗋𝗌𝗂𝗈𝗇 𝟪.𝟢 𝖺𝗌 𝗍𝗁𝖾 𝖻𝖺𝗌𝖾 𝗂𝗆𝖺𝗀𝖾. 𝖳𝗁𝗂𝗌 𝗂𝗆𝖺𝗀𝖾 𝗂𝗌 𝗅𝗂𝗀𝗁𝗍𝖾𝗋 𝗍𝗁𝖺𝗇 𝗍𝗁𝖾 𝖲𝖣𝖪 𝗂𝗆𝖺𝗀𝖾 𝖺𝗇𝖽 𝗂𝗌 𝗌𝗎𝗂𝗍𝖺𝖻𝗅𝖾 𝖿𝗈𝗋 𝗋𝗎𝗇𝗇𝗂𝗇𝗀 𝗍𝗁𝖾 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇 𝖻𝗎𝗍 𝗇𝗈𝗍 𝖿𝗈𝗋 𝖻𝗎𝗂𝗅𝖽𝗂𝗇𝗀 𝗂𝗍.

`𝖶𝖮𝖱𝖪𝖣𝖨𝖱 /𝖠𝗉𝗉` - 𝖲𝖾𝗍𝗌 𝗍𝗁𝖾 𝗐𝗈𝗋𝗄𝗂𝗇𝗀 𝖽𝗂𝗋𝖾𝖼𝗍𝗈𝗋𝗒 𝗂𝗇 𝗍𝗁𝗂𝗌 𝗇𝖾𝗐 𝗌𝗍𝖺𝗀𝖾 (𝗋𝗎𝗇𝗍𝗂𝗆𝖾 𝗌𝗍𝖺𝗀𝖾) 𝗍𝗈 */𝖠𝗉𝗉*, 𝗌𝗂𝗆𝗂𝗅𝖺𝗋 𝗍𝗈 𝗐𝗁𝖺𝗍 𝗐𝖺𝗌 𝖽𝗈𝗇𝖾 𝗂𝗇 𝗍𝗁𝖾 𝖻𝗎𝗂𝗅𝖽 𝗌𝗍𝖺𝗀𝖾.

`𝖢𝖮𝖯𝖸 --𝖿𝗋𝗈𝗆=𝖻𝗎𝗂𝗅𝖽-𝖾𝗇𝗏 /𝖠𝗉𝗉/𝗈𝗎𝗍 .` - 𝖢𝗈𝗉𝗂𝖾𝗌 𝗍𝗁𝖾 𝖼𝗈𝗆𝗉𝗂𝗅𝖾𝖽 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇 𝖿𝗋𝗈𝗆 𝗍𝗁𝖾 𝗈𝗎𝗍 𝖽𝗂𝗋𝖾𝖼𝗍𝗈𝗋𝗒 𝗈𝖿 𝗍𝗁𝖾 𝖻𝗎𝗂𝗅𝖽-𝖾𝗇𝗏 (*𝗍𝗁𝖾 𝖿𝗂𝗋𝗌𝗍 𝗌𝗍𝖺𝗀𝖾*) 𝗍𝗈 𝗍𝗁𝖾 𝖼𝗎𝗋𝗋𝖾𝗇𝗍 𝗐𝗈𝗋𝗄𝗂𝗇𝗀 𝖽𝗂𝗋𝖾𝖼𝗍𝗈𝗋𝗒 (*/𝖠𝗉𝗉*) 𝗈𝖿 𝗍𝗁𝖾 𝖼𝗎𝗋𝗋𝖾𝗇𝗍 𝗌𝗍𝖺𝗀𝖾. 𝖳𝗁𝗂𝗌 𝗆𝖾𝖺𝗇𝗌 𝗐𝖾 𝖺𝗋𝖾 𝗍𝗋𝖺𝗇𝗌𝖿𝖾𝗋𝗋𝗂𝗇𝗀 𝗈𝗇𝗅𝗒 𝗍𝗁𝖾 𝗇𝖾𝖼𝖾𝗌𝗌𝖺𝗋𝗒 𝖿𝗂𝗅𝖾𝗌 𝗇𝖾𝖾𝖽𝖾𝖽 𝗍𝗈 𝗋𝗎𝗇 𝗍𝗁𝖾 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇, 𝗅𝖾𝖺𝗏𝗂𝗇𝗀 𝖻𝖾𝗁𝗂𝗇𝖽 𝗍𝗁𝖾 𝗌𝗈𝗎𝗋𝖼𝖾 𝖼𝗈𝖽𝖾, 𝖲𝖣𝖪, 𝖺𝗇𝖽 𝖺𝗇𝗒 𝗈𝗍𝗁𝖾𝗋 𝗎𝗇𝗇𝖾𝖼𝖾𝗌𝗌𝖺𝗋𝗒 𝖿𝗂𝗅𝖾𝗌.

`𝖤𝖭𝖳𝖱𝖸𝖯𝖮𝖨𝖭𝖳 ["𝖽𝗈𝗍𝗇𝖾𝗍", "{𝗌𝖾𝗋𝗏𝗂𝖼𝖾 𝗇𝖺𝗆𝖾}.𝖽𝗅𝗅"]` - 𝖲𝗉𝖾𝖼𝗂𝖿𝗂𝖾𝗌 𝗍𝗁𝖾 𝖼𝗈𝗆𝗆𝖺𝗇𝖽 𝗍𝗈 𝗋𝗎𝗇 𝗐𝗁𝖾𝗇 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗌𝗍𝖺𝗋𝗍𝗌. 𝖳𝗁𝗂𝗌 𝗂𝗌 𝗍𝗁𝖾 𝗆𝖺𝗂𝗇 𝖺𝗌𝗌𝖾𝗆𝖻𝗅𝗒 𝗍𝗁𝖺𝗍 𝗐𝖺𝗌 𝖼𝗈𝗆𝗉𝗂𝗅𝖾𝖽 𝖺𝗇𝖽 𝗉𝗎𝖻𝗅𝗂𝗌𝗁𝖾𝖽 𝗂𝗇 𝗍𝗁𝖾 𝗉𝗋𝖾𝗏𝗂𝗈𝗎𝗌 𝗌𝗍𝖾𝗉𝗌.


# End-to-end example

**Create a Dockerfile**
```dockerfile
# Use the .NET 8 SDK image to build the application
FROM mcr.microsoft.com/dotnet/sdk:8.0 AS build-env
WORKDIR /App

# Copy csproj and restore any dependencies (via NuGet)
COPY *.csproj ./
RUN dotnet restore

# Copy the project files and build the application
COPY . ./
RUN dotnet publish -c Release -o out

# Use the .NET 8 runtime image to run the application
FROM mcr.microsoft.com/dotnet/aspnet:8.0
WORKDIR /App
COPY --from=build-env /App/out .
ENTRYPOINT ["dotnet", "MyApp.dll"]
```

𝖳𝗁𝗂𝗌 𝖣𝗈𝖼𝗄𝖾𝗋𝖿𝗂𝗅𝖾 𝖽𝗈𝖾𝗌 𝗍𝗁𝖾 𝖿𝗈𝗅𝗅𝗈𝗐𝗂𝗇𝗀:
- 𝖲𝗍𝖺𝗋𝗍𝗌 𝗐𝗂𝗍𝗁 𝗍𝗁𝖾 .𝖭𝖤𝖳 𝟪 𝖲𝖣𝖪 𝗂𝗆𝖺𝗀𝖾 𝗍𝗈 𝖻𝗎𝗂𝗅𝖽 𝗒𝗈𝗎𝗋 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇.
- 𝖲𝖾𝗍𝗌 𝗍𝗁𝖾 𝗐𝗈𝗋𝗄𝗂𝗇𝗀 𝖽𝗂𝗋𝖾𝖼𝗍𝗈𝗋𝗒 𝗍𝗈 /𝖠𝗉𝗉.
- 𝖢𝗈𝗉𝗂𝖾𝗌 𝗍𝗁𝖾 .𝖼𝗌𝗉𝗋𝗈𝗃 𝖿𝗂𝗅𝖾 𝖺𝗇𝖽 𝗋𝖾𝗌𝗍𝗈𝗋𝖾𝗌 𝖽𝖾𝗉𝖾𝗇𝖽𝖾𝗇𝖼𝗂𝖾𝗌.
- 𝖢𝗈𝗉𝗂𝖾𝗌 𝗍𝗁𝖾 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇'𝗌 𝗌𝗈𝗎𝗋𝖼𝖾 𝖼𝗈𝖽𝖾 𝖺𝗇𝖽 𝗉𝗎𝖻𝗅𝗂𝗌𝗁𝖾𝗌 𝗍𝗁𝖾 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇 𝗍𝗈 𝗍𝗁𝖾 𝗈𝗎𝗍 𝖽𝗂𝗋𝖾𝖼𝗍𝗈𝗋𝗒.
- 𝖥𝗈𝗋 𝗍𝗁𝖾 𝖿𝗂𝗇𝖺𝗅 𝗂𝗆𝖺𝗀𝖾, 𝗂𝗍 𝗌𝗐𝗂𝗍𝖼𝗁𝖾𝗌 𝗍𝗈 𝗍𝗁𝖾 .𝖭𝖤𝖳 𝟪 𝗋𝗎𝗇𝗍𝗂𝗆𝖾 𝗂𝗆𝖺𝗀𝖾.
- 𝖢𝗈𝗉𝗂𝖾𝗌 𝗍𝗁𝖾 𝗉𝗎𝖻𝗅𝗂𝗌𝗁𝖾𝖽 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇 𝖿𝗋𝗈𝗆 𝗍𝗁𝖾 𝖻𝗎𝗂𝗅𝖽 𝖾𝗇𝗏𝗂𝗋𝗈𝗇𝗆𝖾𝗇𝗍 𝗍𝗈 𝗍𝗁𝖾 𝗋𝗎𝗇𝗍𝗂𝗆𝖾 𝖾𝗇𝗏𝗂𝗋𝗈𝗇𝗆𝖾𝗇𝗍.
- 𝖲𝗉𝖾𝖼𝗂𝖿𝗂𝖾𝗌 𝗍𝗁𝖾 𝖼𝗈𝗆𝗆𝖺𝗇𝖽 𝗍𝗈 𝗋𝗎𝗇 𝗍𝗁𝖾 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇.

**𝖡𝗎𝗂𝗅𝖽 𝗍𝗁𝖾 𝖣𝗈𝖼𝗄𝖾𝗋 𝖨𝗆𝖺𝗀𝖾** - `𝖽𝗈𝖼𝗄𝖾𝗋 𝖻𝗎𝗂𝗅𝖽 -𝗍 𝗆𝗒-𝖽𝗈𝗍𝗇𝖾𝗍-𝗂𝗆𝖺𝗀𝖾 .`

**𝖱𝗎𝗇 𝗍𝗁𝖾 𝖢𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋** - `𝖽𝗈𝖼𝗄𝖾𝗋 𝗋𝗎𝗇 -𝖽 -𝗉 𝟪𝟢𝟪𝟢:𝟪𝟢 --𝗇𝖺𝗆𝖾 𝗆𝗒-𝖽𝗈𝗍𝗇𝖾𝗍-𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗆𝗒-𝖽𝗈𝗍𝗇𝖾𝗍-𝗂𝗆𝖺𝗀𝖾`

**𝖵𝗂𝖾𝗐 𝗍𝗁𝖾 𝖢𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋'𝗌 𝖫𝗈𝗀𝗌** - `𝖽𝗈𝖼𝗄𝖾𝗋 𝗅𝗈𝗀𝗌 𝗆𝗒-𝖽𝗈𝗍𝗇𝖾𝗍-𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋`
