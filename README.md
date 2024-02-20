
* [Docker](#docker)
  * [Run](#run)
  * [Network](#docker-networking)
  * [Volumes](#volumes)
  * [Compose](#compose)
* [Kubernetes](#kubernetes) 

# Docker
### 𝖶𝗁𝖺𝗍 𝗂𝗌 𝖣𝗈𝖼𝗄𝖾𝗋?
𝖣𝗈𝖼𝗄𝖾𝗋 𝗂𝗌 𝖺 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗂𝗓𝖺𝗍𝗂𝗈𝗇 𝗉𝗅𝖺𝗍𝖿𝗈𝗋𝗆 𝗍𝗁𝖺𝗍 𝖺𝗅𝗅𝗈𝗐𝗌 𝗍𝗈 𝗉𝗎𝗍 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇𝗌 𝖺𝗇𝖽 𝗍𝗁𝖾𝗂𝗋 𝖽𝖾𝗉𝖾𝗇𝖽𝖾𝗇𝖼𝗂𝖾𝗌 𝗂𝗇𝗍𝗈 𝗂𝗌𝗈𝗅𝖺𝗍𝖾𝖽, 𝗅𝗂𝗀𝗁𝗍𝗐𝖾𝗂𝗀𝗁𝗍 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌.
<br>
𝖳𝗁𝖾𝗌𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 𝖼𝖺𝗇 𝗋𝗎𝗇 𝖼𝗈𝗇𝗌𝗂𝗌𝗍𝖾𝗇𝗍𝗅𝗒 𝖺𝖼𝗋𝗈𝗌𝗌 𝖽𝗂𝖿𝖿𝖾𝗋𝖾𝗇𝗍 𝖾𝗇𝗏𝗂𝗋𝗈𝗇𝗆𝖾𝗇𝗍𝗌, 𝗌𝗎𝖼𝗁 𝖺𝗌 𝖽𝖾𝗏𝖾𝗅𝗈𝗉𝗆𝖾𝗇𝗍, 𝗍𝖾𝗌𝗍𝗂𝗇𝗀, 𝖺𝗇𝖽 𝗉𝗋𝗈𝖽𝗎𝖼𝗍𝗂𝗈𝗇, 𝖾𝗇𝗌𝗎𝗋𝗂𝗇𝗀 𝗍𝗁𝖺𝗍 𝖺𝗇 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇 𝖻𝖾𝗁𝖺𝗏𝖾𝗌 𝗍𝗁𝖾 𝗌𝖺𝗆𝖾 𝗐𝖺𝗒 𝗋𝖾𝗀𝖺𝗋𝖽𝗅𝖾𝗌𝗌 𝗈𝖿 𝗍𝗁𝖾 𝗎𝗇𝖽𝖾𝗋𝗅𝗒𝗂𝗇𝗀 𝗂𝗇𝖿𝗋𝖺𝗌𝗍𝗋𝗎𝖼𝗍𝗎𝗋𝖾.

𝖣𝗈𝖼𝗄𝖾𝗋 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 𝗐𝗈𝗋𝗄 𝖻𝗒 𝗋𝗎𝗇𝗇𝗂𝗇𝗀 𝗈𝗇 𝗍𝗈𝗉 𝗈𝖿 𝗍𝗁𝖾 𝖣𝗈𝖼𝗄𝖾𝗋 𝖤𝗇𝗀𝗂𝗇𝖾, 𝗐𝗁𝗂𝖼𝗁 𝗎𝗌𝖾𝗌 𝗍𝗁𝖾 𝗁𝗈𝗌𝗍 𝗈𝗉𝖾𝗋𝖺𝗍𝗂𝗇𝗀 𝗌𝗒𝗌𝗍𝖾𝗆'𝗌 𝗄𝖾𝗋𝗇𝖾𝗅 𝖻𝗎𝗍 𝖺𝗅𝗅𝗈𝗐𝗌 𝖾𝖺𝖼𝗁 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗍𝗈 𝖻𝖾 𝗂𝗌𝗈𝗅𝖺𝗍𝖾𝖽, 𝗆𝖺𝗇𝖺𝗀𝖾 𝗂𝗍𝗌 𝗈𝗐𝗇 𝖽𝖾𝗉𝖾𝗇𝖽𝖾𝗇𝖼𝗂𝖾𝗌, 𝖺𝗇𝖽 𝖾𝗑𝖾𝖼𝗎𝗍𝖾 𝗂𝗇𝖽𝖾𝗉𝖾𝗇𝖽𝖾𝗇𝗍𝗅𝗒.

### Key Docker Concepts:
 - `Images:` Docker images are the building blocks of containers. They contain everything needed to run an application, including the code, runtime, system tools, and libraries.
 - `Containers:` Containers are instances of Docker images. They run in isolated environments and provide a consistent runtime environment for applications.
 - `Docker Hub:` Docker Hub is a repository for finding and sharing Docker images.

## Run

#### Running a Container from Docker Registry

𝖳𝗁𝖾 𝖣𝗈𝖼𝗄𝖾𝗋 𝖱𝖾𝗀𝗂𝗌𝗍𝗋𝗒, 𝗌𝗎𝖼𝗁 𝖺𝗌 𝖣𝗈𝖼𝗄𝖾𝗋 𝖧𝗎𝖻 𝗈𝗋 𝖺𝗇𝗒 𝗉𝗋𝗂𝗏𝖺𝗍𝖾 𝗋𝖾𝗀𝗂𝗌𝗍𝗋𝗒, 𝗂𝗌 𝖺 𝗋𝖾𝗉𝗈𝗌𝗂𝗍𝗈𝗋𝗒 𝖿𝗈𝗋 𝖣𝗈𝖼𝗄𝖾𝗋 𝗂𝗆𝖺𝗀𝖾𝗌 𝖿𝗋𝗈𝗆 𝗐𝗁𝖾𝗋𝖾 𝗒𝗈𝗎 𝖼𝖺𝗇 𝗉𝗎𝗅𝗅 𝖺𝗇𝖽 𝗋𝗎𝗇 𝗉𝗋𝖾-𝖻𝗎𝗂𝗅𝖽 𝖽𝗈𝖼𝗄𝖾𝗋 𝗂𝗆𝖺𝗀𝖾𝗌.

 - Pull Image<br> `docker pull <image_name>:<tag>`
   - 𝖱𝖾𝗉𝗅𝖺𝖼𝖾 <𝗂𝗆𝖺𝗀𝖾_𝗇𝖺𝗆𝖾> 𝗐𝗂𝗍𝗁 𝗍𝗁𝖾 𝗇𝖺𝗆𝖾 𝗈𝖿 𝗍𝗁𝖾 𝗂𝗆𝖺𝗀𝖾 𝖺𝗇𝖽 <𝗍𝖺𝗀> 𝗐𝗂𝗍𝗁 𝗍𝗁𝖾 𝗏𝖾𝗋𝗌𝗂𝗈𝗇 𝗈𝖿 𝗍𝗁𝖾 𝗂𝗆𝖺𝗀𝖾 𝗒𝗈𝗎 𝗐𝖺𝗇𝗍 𝗍𝗈 𝗎𝗌𝖾.
 - Run the Container<br> `docker run -p <external port>:<internal port> <options> <image_name>:<tag>`
   - 𝖳𝗁𝖾 <𝗈𝗉𝗍𝗂𝗈𝗇𝗌> 𝖼𝖺𝗇 𝖻𝖾 𝗏𝖺𝗋𝗂𝗈𝗎𝗌 𝖿𝗅𝖺𝗀𝗌 𝗒𝗈𝗎 𝗉𝗋𝗈𝗏𝗂𝖽𝖾 𝗍𝗈 𝖣𝗈𝖼𝗄𝖾𝗋 𝗍𝗈 𝗆𝗈𝖽𝗂𝖿𝗒 𝗍𝗁𝖾 𝖻𝖾𝗁𝖺𝗏𝗂𝗈𝗋 𝗈𝖿 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋.
   - `-d, --detach` 𝗋𝗎𝗇 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗂𝗇 𝖻𝖺𝖼𝗄𝗀𝗋𝗈𝗎𝗇𝖽 𝖺𝗇𝖽 𝗉𝗋𝗂𝗇𝗍 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝖨𝖽
   - `-p, --publish` 𝗉𝗎𝖻𝗅𝗂𝗌𝗁 𝖺 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋'𝗌 𝗉𝗈𝗋𝗍(𝗌) 𝗍𝗈 𝗍𝗁𝖾 𝗁𝗈𝗌𝗍
   - `--name` 𝖺𝗌𝗌𝗂𝗀𝗇 𝖺 𝗇𝖺𝗆𝖾 𝗍𝗈 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋

---

#### Building Container and Running It

 - Create a Dockerfile
   - 𝖠 𝗌𝗂𝗆𝗉𝗅𝖾 𝗍𝖾𝗑𝗍 𝖿𝗂𝗅𝖾 𝗇𝖺𝗆𝖾𝖽 '𝖣𝗈𝖼𝗄𝖾𝗋𝖿𝗂𝗅𝖾' 𝗍𝗁𝖺𝗍 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝗌 𝗂𝗇𝗌𝗍𝗋𝗎𝖼𝗍𝗂𝗈𝗇𝗌 𝗈𝗇 𝗁𝗈𝗐 𝗍𝗈 𝖻𝗎𝗂𝗅𝖽 𝗍𝗁𝖾 𝗂𝗆𝖺𝗀𝖾. T𝗁𝗂𝗌 𝖣𝗈𝖼𝗄𝖾𝗋𝖿𝗂𝗅𝖾 𝖽𝖾𝖿𝗂𝗇𝖾𝗌 𝖺 𝗆𝗎𝗅𝗍𝗂-𝗌𝗍𝖺𝗀𝖾 𝖻𝗎𝗂𝗅𝖽 𝗉𝗋𝗈𝖼𝖾𝗌𝗌 𝗐𝗁𝖾𝗋𝖾 𝗍𝗁𝖾 𝖿𝗂𝗋𝗌𝗍 𝗌𝗍𝖺𝗀𝖾 𝖻𝗎𝗂𝗅𝖽𝗌 𝗍𝗁𝖾 .𝖭𝖤𝖳 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇, 𝖺𝗇𝖽 𝗍𝗁𝖾 𝗌𝖾𝖼𝗈𝗇𝖽 𝗌𝗍𝖺𝗀𝖾 𝗉𝗋𝖾𝗉𝖺𝗋𝖾𝗌 𝖺 𝗅𝗂𝗀𝗁𝗍𝖾𝗋 𝗋𝗎𝗇𝗍𝗂𝗆𝖾 𝖾𝗇𝗏𝗂𝗋𝗈𝗇𝗆𝖾𝗇𝗍 𝗍𝗈 𝗋𝗎𝗇 𝗍𝗁𝖾 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇.
     ```dockerfile
     # 𝖳𝗁𝗂𝗌 𝗅𝗂𝗇𝖾 𝗂𝗌 𝗍𝖾𝗅𝗅𝗂𝗇𝗀 𝖣𝗈𝖼𝗄𝖾𝗋 𝗍𝗈 𝗎𝗌𝖾 𝗍𝗁𝖾 .𝖭𝖤𝖳 𝖲𝖣𝖪 𝗏𝖾𝗋𝗌𝗂𝗈𝗇 𝟪.𝟢 𝗂𝗆𝖺𝗀𝖾
     # 𝖿𝗋𝗈𝗆 𝖬𝗂𝖼𝗋𝗈𝗌𝗈𝖿𝗍'𝗌 𝖢𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝖱𝖾𝗀𝗂𝗌𝗍𝗋𝗒 𝖺𝗌 𝗍𝗁𝖾 𝖻𝖺𝗌𝖾 𝗂𝗆𝖺𝗀𝖾 𝖿𝗈𝗋 𝗍𝗁𝖾 𝖻𝗎𝗂𝗅𝖽 𝗉𝗋𝗈𝖼𝖾𝗌𝗌.
     # `𝖠𝖲 𝖻𝗎𝗂𝗅𝖽-𝖾𝗇𝗏` s𝖾𝗍 𝖺 𝗇𝖺𝗆𝖾 𝗍𝗈 𝗍𝗁𝗂𝗌 𝗌𝗍𝖺𝗀𝖾 𝗍𝗈 𝗎𝗌𝖾 𝗂𝗍 𝗅𝖺𝗍𝖾𝗋 𝗅𝗂𝗄𝖾 𝖺 𝗏𝖺𝗋𝗂𝖺𝖻𝗅𝖾.
     FROM mcr.microsoft.com/dotnet/sdk:8.0 AS build-env

     # 𝖲𝖾𝗍 𝗍𝗁𝖾 𝗐𝗈𝗋𝗄𝗂𝗇𝗀 𝖽𝗂𝗋𝖾𝖼𝗍𝗈𝗋𝗒 𝗂𝗇𝗌𝗂𝖽𝖾 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗍𝗈 /𝖠𝗉𝗉.
     # 𝖳𝗁𝗂𝗌 𝗂𝗌 𝗐𝗁𝖾𝗋𝖾 𝗒𝗈𝗎𝗋 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇'𝗌 𝖼𝗈𝖽𝖾 𝗐𝗂𝗅𝗅 𝗋𝖾𝗌𝗂𝖽𝖾 𝗐𝗂𝗍𝗁𝗂𝗇 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝖽𝗎𝗋𝗂𝗇𝗀 𝗍𝗁𝖾 𝖻𝗎𝗂𝗅𝖽 𝗉𝗋𝗈𝖼𝖾𝗌𝗌.
     WORKDIR /App

     # Copy 𝖾𝗏𝖾𝗋𝗒𝗍𝗁𝗂𝗇𝗀 𝖿𝗋𝗈𝗆 𝗒𝗈𝗎𝗋 𝗉𝗋𝗈𝗃𝖾𝖼𝗍'𝗌 𝖿𝗈𝗅𝖽𝖾𝗋 (𝗐𝗁𝖾𝗋𝖾 𝗍𝗁𝖾 𝖣𝗈𝖼𝗄𝖾𝗋𝖿𝗂𝗅𝖾 𝗂𝗌 𝗅𝗈𝖼𝖺𝗍𝖾𝖽)
     # 𝗂𝗇𝗍𝗈 𝗍𝗁𝖾 𝖼𝗎𝗋𝗋𝖾𝗇𝗍 𝗐𝗈𝗋𝗄𝗂𝗇𝗀 𝖽𝗂𝗋𝖾𝖼𝗍𝗈𝗋𝗒 𝗂𝗇𝗌𝗂𝖽𝖾 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 (/𝖠𝗉𝗉).
     COPY . ./

     # 𝖤𝗑𝖾𝖼𝗎𝗍𝖾 𝗍𝗁𝖾 𝖽𝗈𝗍𝗇𝖾𝗍 𝗋𝖾𝗌𝗍𝗈𝗋𝖾 𝖼𝗈𝗆𝗆𝖺𝗇𝖽. 𝖳𝗁𝗂𝗌 𝖼𝗈𝗆𝗆𝖺𝗇𝖽 𝗅𝗈𝗈𝗄𝗌 𝖺𝗍 𝗍𝗁𝖾 .𝖭𝖤𝖳 𝗉𝗋𝗈𝗃𝖾𝖼𝗍 𝖿𝗂𝗅𝖾𝗌 𝗂𝗇 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋
     # 𝖺𝗇𝖽 𝖽𝗈𝗐𝗇𝗅𝗈𝖺𝖽𝗌 𝖺𝗇𝗒 𝖽𝖾𝗉𝖾𝗇𝖽𝖾𝗇𝖼𝗂𝖾𝗌 (*𝗅𝗂𝖻𝗋𝖺𝗋𝗂𝖾𝗌 𝖺𝗇𝖽 𝗉𝖺𝖼𝗄𝖺𝗀𝖾𝗌*) 𝗍𝗁𝖺𝗍 𝖺𝗋𝖾 𝗇𝖾𝖾𝖽𝖾𝖽 𝗍𝗈 𝖻𝗎𝗂𝗅𝖽 𝗍𝗁𝖾 𝗉𝗋𝗈𝗃𝖾𝖼𝗍.
     RUN dotnet restore

     # 𝖳𝗁𝗂𝗌 𝖼𝗈𝗆𝗆𝖺𝗇𝖽 𝖻𝗎𝗂𝗅𝖽𝗌 the .𝖭𝖤𝖳 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇 𝗂𝗇 𝗋𝖾𝗅𝖾𝖺𝗌𝖾 𝗆𝗈𝖽𝖾 (-c Release)
     # 𝖺𝗇𝖽 𝗈𝗎𝗍𝗉𝗎𝗍𝗌 𝗍𝗁𝖾 𝖼𝗈𝗆𝗉𝗂𝗅𝖾𝖽 𝖿𝗂𝗅𝖾𝗌 𝗍𝗈 𝗍𝗁𝖾 /𝗈𝗎𝗍 𝖽𝗂𝗋𝖾𝖼𝗍𝗈𝗋𝗒 𝗐𝗂𝗍𝗁𝗂𝗇 𝗍𝗁𝖾 /𝖠𝗉𝗉 𝖽𝗂𝗋𝖾𝖼𝗍𝗈𝗋𝗒 𝗂𝗇 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋.
     RUN dotnet publish -c Release -o out

     # 𝖠𝖿𝗍𝖾𝗋 𝖻𝗎𝗂𝗅𝖽𝗂𝗇𝗀 𝗍𝗁𝖾 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇, 𝗍𝗁𝗂𝗌 𝗅𝗂𝗇𝖾 𝗌𝗍𝖺𝗋𝗍𝗌 𝖺 𝗇𝖾𝗐 𝗌𝗍𝖺𝗀𝖾 𝗂𝗇 𝗍𝗁𝖾 𝖣𝗈𝖼𝗄𝖾𝗋𝖿𝗂𝗅𝖾.
     # 𝖨𝗍 𝗎𝗌𝖾𝗌 𝗍𝗁𝖾 .𝖭𝖤𝖳 𝗋𝗎𝗇𝗍𝗂𝗆𝖾 𝗂𝗆𝖺𝗀𝖾 (𝗇𝗈𝗍 𝗍𝗁𝖾 𝖲𝖣𝖪) 𝗏𝖾𝗋𝗌𝗂𝗈𝗇 𝟪.𝟢 𝖺𝗌 𝗍𝗁𝖾 𝖻𝖺𝗌𝖾 𝗂𝗆𝖺𝗀𝖾.
     # 𝖳𝗁𝗂𝗌 𝗂𝗆𝖺𝗀𝖾 𝗂𝗌 𝗅𝗂𝗀𝗁𝗍𝖾𝗋 𝗍𝗁𝖺𝗇 𝗍𝗁𝖾 𝖲𝖣𝖪 𝗂𝗆𝖺𝗀𝖾 𝖺𝗇𝖽 𝗂𝗌 𝗌𝗎𝗂𝗍𝖺𝖻𝗅𝖾 𝖿𝗈𝗋 𝗋𝗎𝗇𝗇𝗂𝗇𝗀 it 𝖻𝗎𝗍 𝗇𝗈𝗍 𝖿𝗈𝗋 𝖻𝗎𝗂𝗅𝖽𝗂𝗇𝗀 𝗂𝗍.
     FROM mcr.microsoft.com/dotnet/aspnet:8.0

     # Set 𝗍𝗁𝖾 𝗐𝗈𝗋𝗄𝗂𝗇𝗀 𝖽𝗂𝗋𝖾𝖼𝗍𝗈𝗋𝗒 𝗂𝗇 𝗍𝗁𝗂𝗌 𝗇𝖾𝗐 𝗌𝗍𝖺𝗀𝖾 (𝗋𝗎𝗇𝗍𝗂𝗆𝖾 𝗌𝗍𝖺𝗀𝖾)
     # 𝗍𝗈 */𝖠𝗉𝗉*, 𝗌𝗂𝗆𝗂𝗅𝖺𝗋 𝗍𝗈 𝗐𝗁𝖺𝗍 𝗐𝖺𝗌 𝖽𝗈𝗇𝖾 𝗂𝗇 𝗍𝗁𝖾 𝖻𝗎𝗂𝗅𝖽 𝗌𝗍𝖺𝗀𝖾.
     WORKDIR /App

     # Copy 𝗍𝗁𝖾 𝖼𝗈𝗆𝗉𝗂𝗅𝖾𝖽 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇 𝖿𝗋𝗈𝗆 /𝗈𝗎𝗍 𝖽𝗂𝗋𝖾𝖼𝗍𝗈𝗋𝗒 𝗈𝖿 𝗍𝗁𝖾 𝖻𝗎𝗂𝗅𝖽-𝖾𝗇𝗏 (𝗍𝗁𝖾 𝖿𝗂𝗋𝗌𝗍 𝗌𝗍𝖺𝗀𝖾)
     # 𝗍𝗈 𝗍𝗁𝖾 𝖼𝗎𝗋𝗋𝖾𝗇𝗍 𝗐𝗈𝗋𝗄𝗂𝗇𝗀 𝖽𝗂𝗋𝖾𝖼𝗍𝗈𝗋𝗒 (/𝖠𝗉𝗉) 𝗈𝖿 𝗍𝗁𝖾 𝖼𝗎𝗋𝗋𝖾𝗇𝗍 𝗌𝗍𝖺𝗀𝖾.
     # 𝖳𝗁𝗂𝗌 𝗆𝖾𝖺𝗇𝗌 𝗐𝖾 𝖺𝗋𝖾 𝗍𝗋𝖺𝗇𝗌𝖿𝖾𝗋𝗋𝗂𝗇𝗀 𝗈𝗇𝗅𝗒 𝗍𝗁𝖾 𝗇𝖾𝖼𝖾𝗌𝗌𝖺𝗋𝗒 𝖿𝗂𝗅𝖾𝗌 𝗇𝖾𝖾𝖽𝖾𝖽 𝗍𝗈 𝗋𝗎𝗇 𝗍𝗁𝖾 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇,
     # 𝗅𝖾𝖺𝗏𝗂𝗇𝗀 𝖻𝖾𝗁𝗂𝗇𝖽 𝗍𝗁𝖾 𝗌𝗈𝗎𝗋𝖼𝖾 𝖼𝗈𝖽𝖾, 𝖲𝖣𝖪, 𝖺𝗇𝖽 𝖺𝗇𝗒 𝗈𝗍𝗁𝖾𝗋 𝗎𝗇𝗇𝖾𝖼𝖾𝗌𝗌𝖺𝗋𝗒 𝖿𝗂𝗅𝖾𝗌.
     COPY --from=build-env /App/out .
     
     # 𝖲𝗉𝖾𝖼𝗂𝖿𝗂𝖾𝗌 𝗍𝗁𝖾 𝖼𝗈𝗆𝗆𝖺𝗇𝖽 𝗍𝗈 𝗋𝗎𝗇 𝗐𝗁𝖾𝗇 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗌𝗍𝖺𝗋𝗍𝗌.
     # 𝖳𝗁𝗂𝗌 𝗂𝗌 𝗍𝗁𝖾 𝗆𝖺𝗂𝗇 𝖺𝗌𝗌𝖾𝗆𝖻𝗅𝗒 𝗍𝗁𝖺𝗍 𝗐𝖺𝗌 𝖼𝗈𝗆𝗉𝗂𝗅𝖾𝖽 𝖺𝗇𝖽 𝗉𝗎𝖻𝗅𝗂𝗌𝗁𝖾𝖽 𝗂𝗇 𝗍𝗁𝖾 𝗉𝗋𝖾𝗏𝗂𝗈𝗎𝗌 𝗌𝗍𝖾𝗉𝗌.
     ENTRYPOINT ["dotnet", "{service name}.dll"]
     ```
   - Build the Image - 𝗐𝗂𝗍𝗁 𝗍𝗁𝖾 𝖣𝗈𝖼𝗄𝖾𝗋𝖿𝗂𝗅𝖾 𝗂𝗇 𝗍𝗁𝖾 𝗌𝖺𝗆𝖾 𝖽𝗂𝗋𝖾𝖼𝗍𝗈𝗋𝗒, 𝗋𝗎𝗇 𝗍𝗁𝖾 𝖿𝗈𝗅𝗅𝗈𝗐𝗂𝗇𝗀 𝖼𝗈𝗆𝗆𝖺𝗇𝖽 𝗍𝗈 𝖻𝗎𝗂𝗅𝖽 𝗍𝗁𝖾 𝖣𝗈𝖼𝗄𝖾𝗋 𝗂𝗆𝖺𝗀𝖾 <br> `docker build -t <your_image_name>:<tag> .`
   - Run Your Container<br> `docker run -p <external port>:<internal port> <options> <image_name>:<tag>`

---

#### Port Forwarding in Docker

Port forwarding in Docker is a technique used to allow external access to applications running inside a container.
<br>
This is achieved by mapping a port on the host machine to a port inside the Docker container.


```json
{
  "profiles": {
      "applicationUrl": "https://localhost:5000"
  }
}
```

𝖨𝖿 𝗐𝖾 𝗁𝖺𝗏𝖾 𝖺𝗇 𝖺𝗉𝗉, 𝗍𝗁𝖺𝗍 𝗋𝗎𝗇𝗌 𝗈𝗇 𝗉𝗈𝗋𝗍 `𝟧𝟢𝟢𝟢`, 𝗍𝗁𝗂𝗌 𝗉𝗈𝗋𝗍 `𝟧𝟢𝟢𝟢` 𝗂𝗌 𝗈𝗇𝗅𝗒 𝖺𝖼𝖼𝖾𝗌𝗌𝗂𝖻𝗅𝖾 𝖿𝗋𝗈𝗆 𝗂𝗇𝗌𝗂𝖽𝖾 𝗍𝗁𝖾 𝖽𝗈𝖼𝗄𝖾𝗋 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋. 𝖳𝗈 𝖺𝖼𝖼𝖾𝗌𝗌 𝖺𝗉𝗉 𝗂𝗇 𝖽𝗈𝖼𝗄𝖾𝗋 𝗐𝖾 𝗆𝗎𝗌𝗍 '𝖯𝗈𝗋𝗍 𝖿𝗈𝗋𝗐𝖺𝗋𝖽' 𝖾𝗑𝗍𝖾𝗋𝗇𝖺𝗅 𝗉𝗈𝗋𝗍 𝗍𝗈 𝗍𝗁𝗂𝗌 𝗂𝗇𝗍𝖾𝗋𝗇𝖺𝗅 𝗉𝗈𝗋𝗍 `𝟧𝟢𝟢𝟢`.

𝖯𝗈𝗋𝗍 𝖿𝗈𝗋𝗐𝖺𝗋𝖽𝗂𝗇𝗀 𝗂𝗌 𝖾𝗌𝗌𝖾𝗇𝗍𝗂𝖺𝗅 𝖿𝗈𝗋 𝖺𝖼𝖼𝖾𝗌𝗌𝗂𝗇𝗀 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗂𝗓𝖾𝖽 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇𝗌 𝖿𝗋𝗈𝗆 𝗈𝗎𝗍𝗌𝗂𝖽𝖾 𝗍𝗁𝖾 𝖣𝗈𝖼𝗄𝖾𝗋 𝗁𝗈𝗌𝗍. 𝖶𝗂𝗍𝗁𝗈𝗎𝗍 𝗉𝗈𝗋𝗍 𝖿𝗈𝗋𝗐𝖺𝗋𝖽𝗂𝗇𝗀, 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇𝗌 𝗋𝗎𝗇𝗇𝗂𝗇𝗀 𝗂𝗇𝗌𝗂𝖽𝖾 𝖺 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗐𝗈𝗎𝗅𝖽 𝖻𝖾 𝗂𝗌𝗈𝗅𝖺𝗍𝖾𝖽 𝖺𝗇𝖽 𝗂𝗇𝖺𝖼𝖼𝖾𝗌𝗌𝗂𝖻𝗅𝖾 𝖽𝗎𝖾 𝗍𝗈 𝖣𝗈𝖼𝗄𝖾𝗋'𝗌 𝗇𝖾𝗍𝗐𝗈𝗋𝗄 𝗂𝗌𝗈𝗅𝖺𝗍𝗂𝗈𝗇.

```console
docker run --name webapp -p 50:5000 webapp
```
 - 𝖡𝗒 𝗌𝗉𝖾𝖼𝗂𝖿𝗒𝗂𝗇𝗀 `-𝗉 𝟧𝟢:𝟧𝟢𝟢𝟢`, 𝗐𝖾 𝗂𝗇𝗌𝗍𝗋𝗎𝖼𝗍 𝖣𝗈𝖼𝗄𝖾𝗋 𝗍𝗈 𝖿𝗈𝗋𝗐𝖺𝗋𝖽 𝗋𝖾𝗊𝗎𝖾𝗌𝗍𝗌 𝗆𝖺𝖽𝖾 𝗍𝗈 𝗉𝗈𝗋𝗍 `𝟧𝟢` 𝗈𝗇 𝗍𝗁𝖾 𝗁𝗈𝗌𝗍 𝗍𝗈 𝗉𝗈𝗋𝗍 `𝟧𝟢𝟢𝟢` 𝗂𝗇𝗌𝗂𝖽𝖾 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋. 𝖳𝗁𝗂𝗌 𝖺𝗅𝗅𝗈𝗐𝗌 𝗒𝗈𝗎 𝗍𝗈 𝖺𝖼𝖼𝖾𝗌𝗌 𝗍𝗁𝖾 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇 𝖻𝗒 𝗏𝗂𝗌𝗂𝗍𝗂𝗇𝗀 `𝗅𝗈𝖼𝖺𝗅𝗁𝗈𝗌𝗍:𝟧𝟢` 𝗈𝗇 𝗒𝗈𝗎𝗋 𝗁𝗈𝗌𝗍 𝗆𝖺𝖼𝗁𝗂𝗇𝖾

---

#### Start/Stop Containers
 - 𝖲𝗍𝗈𝗉 𝖠 𝖱𝗎𝗇𝗇𝗂𝗇𝗀 𝖢𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋<br> `docker stop <container Id>`
 - 𝖱𝖾-𝗌𝗍𝖺𝗋𝗍 𝖺 𝖢𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋<br> `docker start <container Id>`

---

## Docker Networking

𝖶𝗁𝖾𝗇 𝗒𝗈𝗎 𝗂𝗇𝗌𝗍𝖺𝗅𝗅 𝖽𝗈𝖼𝗄𝖾𝗋 𝗂𝗍 𝖼𝗋𝖾𝖺𝗍𝖾𝗌 𝗍𝗁𝗋𝖾𝖾 𝗇𝖾𝗍𝗐𝗈𝗋𝗄𝗌 𝖺𝗎𝗍𝗈𝗆𝖺𝗍𝗂𝖼𝖺𝗅𝗅𝗒 - `𝖡𝗋𝗂𝖽𝗀𝖾`, `𝖧𝗈𝗌𝗍`, 𝖺𝗇𝖽 `𝖭𝗈𝗇𝖾`.
<br>
𝖮𝖿 𝗐𝗁𝗂𝖼𝗁, 𝖡𝗋𝗂𝖽𝗀𝖾 𝗂𝗌 𝗍𝗁𝖾 𝖽𝖾𝖿𝖺𝗎𝗅𝗍 𝗇𝖾𝗍𝗐𝗈𝗋𝗄 𝖺 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗀𝖾𝗍𝗌 𝖺𝗍𝗍𝖺𝖼𝗁𝖾𝖽 𝗍𝗈 𝗐𝗁𝖾𝗇 𝗂𝗍 𝗂𝗌 𝗋𝗎𝗇. 𝖳𝗈 𝖺𝗍𝗍𝖺𝖼𝗁 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗍𝗈 𝖺𝗇𝗒 𝗈𝗍𝗁𝖾𝗋 𝗇𝖾𝗍𝗐𝗈𝗋𝗄 𝗒𝗈𝗎 𝖼𝖺𝗇 𝗎𝗌𝖾 𝗍𝗁𝖾 --𝗇𝖾𝗍𝗐𝗈𝗋𝗄 𝖿𝗅𝖺𝗀 𝗈𝖿 𝗍𝗁𝖾 𝗋𝗎𝗇 𝖼𝗈𝗆𝗆𝖺𝗇𝖽.


- `𝖡𝗋𝗂𝖽𝗀𝖾`: 𝖳𝗁𝖾 𝖡𝗋𝗂𝖽𝗀𝖾 𝗇𝖾𝗍𝗐𝗈𝗋𝗄 𝖺𝗌𝗌𝗂𝗀𝗇𝗌 𝖨𝖯𝗌 𝗂𝗇 𝗍𝗁𝖾 𝗋𝖺𝗇𝗀𝖾 𝗈𝖿 𝟣𝟩𝟤.𝟣𝟩.𝗑.𝗑 𝗍𝗈 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 𝗐𝗂𝗍𝗁𝗂𝗇 𝗂𝗍.<br>
𝖳𝗈 𝖺𝖼𝖼𝖾𝗌𝗌 𝗍𝗁𝖾𝗌𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 𝖿𝗋𝗈𝗆 𝗈𝗎𝗍𝗌𝗂𝖽𝖾 𝗒𝗈𝗎 𝗇𝖾𝖾𝖽 𝗍𝗈 𝗆𝖺𝗉 𝗍𝗁𝖾 𝗉𝗈𝗋𝗍𝗌 𝗈𝖿 𝗍𝗁𝖾𝗌𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 𝗍𝗈 𝗍𝗁𝖾 𝗉𝗈𝗋𝗍𝗌 𝗈𝗇 𝗍𝗁𝖾 𝗁𝗈𝗌𝗍.
- `𝖧𝗈𝗌𝗍`: 𝖲𝖾𝗅𝖾𝖼𝗍𝗂𝗇𝗀 𝗍𝗁𝖾 𝖧𝗈𝗌𝗍 𝗇𝖾𝗍𝗐𝗈𝗋𝗄 𝗐𝗂𝗅𝗅 𝗋𝖾𝗆𝗈𝗏𝖾 𝖺𝗇𝗒 𝗇𝖾𝗍𝗐𝗈𝗋𝗄 𝗂𝗌𝗈𝗅𝖺𝗍𝗂𝗈𝗇 𝖻𝖾𝗍𝗐𝖾𝖾𝗇 𝗍𝗁𝖾 𝖽𝗈𝖼𝗄𝖾𝗋 𝗁𝗈𝗌𝗍 𝖺𝗇𝖽 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌.<br>
𝖥𝗈𝗋 𝗂𝗇𝗌𝗍𝖺𝗇𝖼𝖾, 𝗂𝖿 𝗒𝗈𝗎 𝗋𝗎𝗇 𝖺 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗈𝗇 𝗉𝗈𝗋𝗍 𝟧𝟢𝟢𝟢, 𝗂𝗍 𝗐𝗂𝗅𝗅 𝖻𝖾 𝖺𝖼𝖼𝖾𝗌𝗌𝗂𝖻𝗅𝖾 𝗈𝗇 𝗍𝗁𝖾 𝗌𝖺𝗆𝖾 𝗉𝗈𝗋𝗍 𝗈𝗇 𝗍𝗁𝖾 𝖽𝗈𝖼𝗄𝖾𝗋 𝗁𝗈𝗌𝗍 𝗐𝗂𝗍𝗁𝗈𝗎𝗍 𝖺𝗇𝗒 𝖾𝗑𝗉𝗅𝗂𝖼𝗂𝗍 𝗉𝗈𝗋𝗍 𝗆𝖺𝗉𝗉𝗂𝗇𝗀. 𝖳𝗁𝖾 𝗈𝗇𝗅𝗒 𝖽𝗈𝗐𝗇𝗌𝗂𝖽𝖾 𝗈𝖿 𝗍𝗁𝗂𝗌 𝖺𝗉𝗉𝗋𝗈𝖺𝖼𝗁 𝗂𝗌 𝗍𝗁𝖺𝗍 𝗒𝗈𝗎 𝖼𝖺𝗇 𝗇𝗈𝗍 𝗎𝗌𝖾 𝗍𝗁𝖾 𝗌𝖺𝗆𝖾 𝗉𝗈𝗋𝗍 𝗍𝗐𝗂𝖼𝖾 𝖿𝗈𝗋 𝖺𝗇𝗒 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋.
- `𝖭𝗈𝗇𝖾`: 𝖳𝗁𝖾 𝖭𝗈𝗇𝖾 𝗇𝖾𝗍𝗐𝗈𝗋𝗄 𝗄𝖾𝖾𝗉𝗌 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗂𝗇 𝖼𝗈𝗆𝗉𝗅𝖾𝗍𝖾 𝗂𝗌𝗈𝗅𝖺𝗍𝗂𝗈𝗇, 𝗂.𝖾. 𝗍𝗁𝖾𝗒 𝖺𝗋𝖾 𝗇𝗈𝗍 𝖼𝗈𝗇𝗇𝖾𝖼𝗍𝖾𝖽 𝗍𝗈 𝖺𝗇𝗒 𝗇𝖾𝗍𝗐𝗈𝗋𝗄 𝗈𝗋 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋.

𝖡𝗒 𝖽𝖾𝖿𝖺𝗎𝗅𝗍 𝖺𝗅𝗅 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 𝖺𝗋𝖾 𝗂𝗇 `𝖡𝗋𝗂𝖽𝗀𝖾` 𝗇𝖾𝗍𝗐𝗈𝗋𝗄.
𝖨𝖿 𝗐𝖾 𝗐𝖺𝗇𝗍 𝗍𝗈 𝗋𝗎𝗇 𝗍𝗐𝗈 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 𝗂𝗇 𝖺 𝗌𝖾𝗉𝖺𝗋𝖺𝗍𝖾 𝗇𝖾𝗍𝗐𝗈𝗋𝗄,<br>
𝗐𝖾 𝖼𝖺𝗇 𝖽𝖾𝖿𝗂𝗇𝖾 𝖺 𝖼𝗎𝗌𝗍𝗈𝗆(𝗎𝗌𝖾𝗋-𝖽𝖾𝖿𝗂𝗇𝖾𝖽) 𝗇𝖾𝗍𝗐𝗈𝗋𝗄 𝖿𝗈𝗋 𝗍𝗁𝗂𝗌 𝗉𝗎𝗋𝗉𝗈𝗌𝖾 𝖻𝗒 𝗎𝗌𝗂𝗇𝗀 𝗍𝗁𝖾 𝖿𝗈𝗅𝗅𝗈𝗐𝗂𝗇𝗀 𝖼𝗈𝗆𝗆𝖺𝗇𝖽 𝖺𝗇𝖽 𝖺𝗌𝗌𝗂𝗀𝗇𝗂𝗇𝗀 𝗍𝗁𝗂𝗌 𝗇𝖾𝗍𝗐𝗈𝗋𝗄 𝗐𝗁𝖾𝗇 𝗋𝗎𝗇𝗇𝗂𝗇𝗀 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌.
 - `docker network create <options> <network_name>`

𝖥𝗈𝗋 𝖾𝗑𝖺𝗆𝗉𝗅𝖾, 𝗂𝖿 𝗐𝖾 𝗐𝖺𝗇𝗍 𝗍𝗈 𝖼𝗋𝖾𝖺𝗍𝖾 𝖺 𝗌𝖾𝗉𝖺𝗋𝖺𝗍𝖾 𝗇𝖾𝗍𝗐𝗈𝗋𝗄 𝖿𝗈𝗋 𝖺 𝗐𝖾𝖻𝖠𝗉𝗉 𝗐𝗂𝗍𝗁 𝖽𝖺𝗍𝖺𝖻𝖺𝗌𝖾:

 - 𝖣𝖾𝖿𝗂𝗇𝖾 𝖺 𝗇𝖾𝗍𝗐𝗈𝗋𝗄 (𝗌𝗉𝖾𝖼𝗂𝖿𝗒𝗂𝗇𝗀 𝖽𝗋𝗂𝗏𝖾𝗋 𝖺𝗇𝖽 𝗌𝗎𝖻𝗇𝖾𝗍 𝖺𝗋𝖾 𝗈𝗉𝗍𝗂𝗈𝗇𝖺𝗅)
   ```console
   docker network create \
      --driver bridge \
      --subnet 192.168.0.0/24 \
      user-net
   ```
 - 𝖢𝗋𝖾𝖺𝗍𝖾 𝖺 𝖯𝗈𝗌𝗍𝗀𝗋𝖾𝗌 𝗂𝗇𝗌𝗍𝖺𝗇𝖼𝖾
   - 𝖯𝗎𝗅𝗅 𝗅𝖺𝗍𝖾𝗌𝗍 𝖯𝗈𝗌𝗍𝗀𝗋𝖾𝗌 𝗂𝗆𝖺𝗀𝖾
     ```console
     docker pull postgres
     ```
   - 𝖡𝗎𝗂𝗅𝖽 𝗉𝗈𝗌𝗍𝗀𝗋𝖾𝗌 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋
     ```console
     docker run --name postgres-db \
        -e POSTGRES_USER=postgres \
        -e POSTGRES_PASSWORD=12345678 \
        -e POSTGRES_DB=postgres_db \
        --network user-net \
        -p 5432:5432 \
        --detach \
        postgres
     ```
 - 𝖢𝗋𝖾𝖺𝗍𝖾 𝖺 𝗐𝖾𝖻𝖠𝗉𝗉 𝗂𝗇𝗌𝗍𝖺𝗇𝖼𝖾
   - 𝖡𝗎𝗂𝗅𝖽 𝗐𝖾𝖻𝖠𝗉𝗉 𝗂𝗆𝖺𝗀𝖾
     ```console
     docker build -t webapp-img .
     ```
   - 𝖡𝗎𝗂𝗅𝖽 𝗐𝖾𝖻𝖠𝗉𝗉 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋
     ```console
     docker run \
        --name webApp-container \
        --network user-net \
        -p 5000:5000 \
        --detach \
        webapp-img
     ```


 - 𝖵𝖾𝗋𝗂𝖿𝗒 𝖻𝗈𝗍𝗁 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 𝖺𝗋𝖾 𝗂𝗇 𝗍𝗁𝖾 𝗌𝖺𝗆𝖾 𝗇𝖾𝗍𝗐𝗈𝗋𝗄
     ```console
        docker network inspect user-net
     ```
     ```json
     [
      {
        "Name": "user-net",
        "Id": "9347e11baa1980196bf057c5423ea17aba7d27f322f87f8672abd660bb66618f",

        ...........
     
        "ConfigOnly": false,
        "Containers": {
            "47154a58b83f213dc95dc82df776e4738d96ccbb2b7e3d205ae59dd212326e1d": {
                "Name": "postgres-db",
                "EndpointID": "55227205e9f90f09c612becc5dbd936eeca60e5123e5d6da486c1fe325b5bd51",
                "MacAddress": "02:42:c0:a8:00:02",
                "IPv4Address": "192.168.0.2/24",
                "IPv6Address": ""
            },
            "4e032ad8e55a3bec9207cba652bf8a3d2a89e1a155b2d4d8166f82af5c1a35aa": {
                "Name": "webapp-container",
                "EndpointID": "369656ce018825a47d51c57d7ca1391468df015e3649c871d98c6790a7485d68",
                "MacAddress": "02:42:c0:a8:00:03",
                "IPv4Address": "192.168.0.3/24",
                "IPv6Address": ""
            }
        },
        "Options": {},
        "Labels": {}
      }
     ]
     ```

## Volumes

𝖣𝖺𝗍𝖺 𝗂𝗇𝗌𝗂𝖽𝖾 𝖣𝗈𝖼𝗄𝖾𝗋 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 𝗂𝗌 𝗇𝗈𝗍 𝗉𝖾𝗋𝗌𝗂𝗌𝗍𝖾𝗇𝗍 𝖻𝗒 𝖽𝖾𝖿𝖺𝗎𝗅𝗍. 𝖳𝗁𝗂𝗌 𝗆𝖾𝖺𝗇𝗌 𝗍𝗁𝖺𝗍 𝗐𝗁𝖾𝗇 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗂𝗌 𝖽𝖾𝗌𝗍𝗋𝗈𝗒𝖾𝖽, 𝗌𝗈 𝗂𝗌 𝗍𝗁𝖾 𝖽𝖺𝗍𝖺. <br>
𝖳𝗁𝖾𝗋𝖾 𝗆𝖺𝗒 𝖻𝖾 𝗌𝗂𝗍𝗎𝖺𝗍𝗂𝗈𝗇𝗌 𝗐𝗁𝖾𝗋𝖾 𝗒𝗈𝗎 𝗐𝖺𝗇𝗍 𝗍𝗈 𝗆𝖺𝗂𝗇𝗍𝖺𝗂𝗇 𝖽𝖺𝗍𝖺 𝖻𝖾𝗒𝗈𝗇𝖽 𝗍𝗁𝖾 𝗅𝗂𝖿𝖾𝖼𝗒𝖼𝗅𝖾 𝗈𝖿 𝖺 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋, 𝖺𝗇𝖽 𝗍𝗁𝗂𝗌 𝖼𝖺𝗇 𝖻𝖾 𝖺𝖼𝗁𝗂𝖾𝗏𝖾𝖽 𝗎𝗌𝗂𝗇𝗀 𝗉𝖾𝗋𝗌𝗂𝗌𝗍𝖾𝗇𝗍 𝖽𝖺𝗍𝖺 𝗌𝗍𝗈𝗋𝖺𝗀𝖾.
𝖮𝗇𝖾 𝗈𝗉𝗍𝗂𝗈𝗇 𝖿𝗈𝗋 𝗉𝖾𝗋𝗌𝗂𝗌𝗍𝖾𝗇𝗍 𝖽𝖺𝗍𝖺 𝗌𝗍𝗈𝗋𝖺𝗀𝖾 𝖺𝗏𝖺𝗂𝗅𝖺𝖻𝗅𝖾 𝗐𝗂𝗍𝗁 𝖣𝗈𝖼𝗄𝖾𝗋 𝗂𝗌 `𝗏𝗈𝗅𝗎𝗆𝖾𝗌`

- 𝖠𝗅𝗅 𝗏𝗈𝗅𝗎𝗆𝖾𝗌 𝖺𝗋𝖾 𝗆𝖺𝗇𝖺𝗀𝖾𝖽 𝖻𝗒 𝖣𝗈𝖼𝗄𝖾𝗋 𝖺𝗇𝖽 𝗌𝗍𝗈𝗋𝖾𝖽 𝗂𝗇 𝖺 𝖽𝖾𝖽𝗂𝖼𝖺𝗍𝖾𝖽 𝖽𝗂𝗋𝖾𝖼𝗍𝗈𝗋𝗒 𝗈𝗇 𝗒𝗈𝗎𝗋 𝗁𝗈𝗌𝗍, 𝗎𝗌𝗎𝖺𝗅𝗅𝗒 `/𝗏𝖺𝗋/𝗅𝗂𝖻/𝖽𝗈𝖼𝗄𝖾𝗋/𝗏𝗈𝗅𝗎𝗆𝖾𝗌`
- 𝖣𝖺𝗍𝖺 𝖯𝖾𝗋𝗌𝗂𝗌𝗍𝖾𝗇𝖼𝖾 - 𝖵𝗈𝗅𝗎𝗆𝖾𝗌 𝗉𝗋𝗈𝗏𝗂𝖽𝖾 𝖺 𝗐𝖺𝗒 𝗍𝗈 𝗌𝗍𝗈𝗋𝖾 𝖽𝖺𝗍𝖺 𝗈𝗎𝗍𝗌𝗂𝖽𝖾 𝗈𝖿 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋'𝗌 𝖿𝗂𝗅𝖾 𝗌𝗒𝗌𝗍𝖾𝗆, 𝖾𝗇𝗌𝗎𝗋𝗂𝗇𝗀 𝖽𝖺𝗍𝖺 𝗉𝖾𝗋𝗌𝗂𝗌𝗍𝗌 𝖾𝗏𝖾𝗇 𝖺𝖿𝗍𝖾𝗋 𝖺 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗂𝗌 𝖽𝖾𝗅𝖾𝗍𝖾𝖽
- 𝖣𝖺𝗍𝖺 𝖲𝗁𝖺𝗋𝗂𝗇𝗀 - 𝖵𝗈𝗅𝗎𝗆𝖾𝗌 𝖼𝖺𝗇 𝖻𝖾 𝗌𝗁𝖺𝗋𝖾𝖽 𝖻𝖾𝗍𝗐𝖾𝖾𝗇 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌, 𝖿𝖺𝖼𝗂𝗅𝗂𝗍𝖺𝗍𝗂𝗇𝗀 𝖽𝖺𝗍𝖺 𝖾𝗑𝖼𝗁𝖺𝗇𝗀𝖾 𝗈𝗋 𝗋𝖾𝗎𝗌𝖾 𝗈𝖿 𝖽𝖺𝗍𝖺 𝖺𝖼𝗋𝗈𝗌𝗌 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌
- 𝖯𝖾𝗋𝖿𝗈𝗋𝗆𝖺𝗇𝖼𝖾: 𝖠𝖼𝖼𝖾𝗌𝗌𝗂𝗇𝗀 𝖽𝖺𝗍𝖺 𝗂𝗇 𝖺 𝗏𝗈𝗅𝗎𝗆𝖾 𝗂𝗌 𝖿𝖺𝗌𝗍𝖾𝗋 𝗍𝗁𝖺𝗇 𝖺𝖼𝖼𝖾𝗌𝗌𝗂𝗇𝗀 𝖽𝖺𝗍𝖺 𝗂𝗇 𝖺 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋'𝗌 𝗐𝗋𝗂𝗍𝖺𝖻𝗅𝖾 𝗅𝖺𝗒𝖾𝗋, 𝖺𝗌 𝗏𝗈𝗅𝗎𝗆𝖾𝗌 𝖺𝗋𝖾 𝖽𝗂𝗋𝖾𝖼𝗍𝗅𝗒 𝗆𝗈𝗎𝗇𝗍𝖾𝖽 𝖿𝗋𝗈𝗆 𝗍𝗁𝖾 𝗁𝗈𝗌𝗍.
- 𝖲𝖾𝖼𝗎𝗋𝗂𝗍𝗒: 𝖵𝗈𝗅𝗎𝗆𝖾𝗌 𝖼𝖺𝗇 𝖻𝖾 𝗆𝗈𝗋𝖾 𝗌𝖾𝖼𝗎𝗋𝖾 𝗍𝗁𝖺𝗇 𝖻𝗂𝗇𝖽 𝗆𝗈𝗎𝗇𝗍𝗌 𝗌𝗂𝗇𝖼𝖾 𝗍𝗁𝖾𝗂𝗋 𝖼𝗈𝗇𝗍𝖾𝗇𝗍𝗌 𝖺𝗋𝖾 𝗇𝗈𝗍 𝖽𝗂𝗋𝖾𝖼𝗍𝗅𝗒 𝖾𝗑𝗉𝗈𝗌𝖾𝖽 𝗍𝗈 𝗍𝗁𝖾 𝗁𝗈𝗌𝗍 𝗌𝗒𝗌𝗍𝖾𝗆. 𝖣𝗈𝖼𝗄𝖾𝗋 𝖼𝖺𝗇 𝗆𝖺𝗇𝖺𝗀𝖾 𝗉𝖾𝗋𝗆𝗂𝗌𝗌𝗂𝗈𝗇𝗌 𝖺𝗇𝖽 𝖺𝖼𝖼𝖾𝗌𝗌 𝗍𝗈 𝗍𝗁𝖾 𝖽𝖺𝗍𝖺.

#### Using Volumes
𝖴𝗌𝗎𝖺𝗅𝗅𝗒 𝗍𝗁𝖾 𝗏𝗈𝗅𝗎𝗆𝖾𝗌 𝖺𝗋𝖾 𝖼𝗋𝖾𝖺𝗍𝖾𝖽 𝗐𝗂𝗍𝗁 `𝗋𝗎𝗇` 𝖼𝗈𝗆𝗆𝖺𝗇𝖽.<br>
𝖳𝗈 𝗎𝗌𝖾 𝗏𝗈𝗅𝗎𝗆𝖾𝗌, 𝗒𝗈𝗎 𝖼𝖺𝗇 𝗌𝗉𝖾𝖼𝗂𝖿𝗒 𝗍𝗁𝖾𝗆 𝗐𝗁𝖾𝗇 𝗒𝗈𝗎 𝗋𝗎𝗇 𝖺 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗐𝗂𝗍𝗁 𝗍𝗁𝖾 `-𝗏` 𝗈𝗋 `--𝗏𝗈𝗅𝗎𝗆𝖾 𝖿𝗅𝖺𝗀`.<br>
𝖳𝗁𝖾𝗋𝖾 𝖺𝗋𝖾 𝗍𝗐𝗈 𝗆𝖺𝗂𝗇 𝗐𝖺𝗒𝗌 𝗍𝗈 𝗎𝗌𝖾 𝗏𝗈𝗅𝗎𝗆𝖾𝗌:
 - 𝖭𝖺𝗆𝖾𝖽 𝖵𝗈𝗅𝗎𝗆𝖾𝗌: 𝖭𝖺𝗆𝖾𝖽 𝗏𝗈𝗅𝗎𝗆𝖾𝗌 𝖺𝗋𝖾 𝖾𝗑𝗉𝗅𝗂𝖼𝗂𝗍𝗅𝗒 𝗇𝖺𝗆𝖾𝖽 𝖺𝗍 𝗍𝗁𝖾 𝗍𝗂𝗆𝖾 𝗈𝖿 𝗍𝗁𝖾𝗂𝗋 𝖼𝗋𝖾𝖺𝗍𝗂𝗈𝗇 𝖺𝗇𝖽 𝖼𝖺𝗇 𝖻𝖾 𝗋𝖾𝗎𝗌𝖾𝖽 𝖺𝖼𝗋𝗈𝗌𝗌 𝗆𝗎𝗅𝗍𝗂𝗉𝗅𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌.<br>
   𝖶𝖾 𝖼𝖺𝗇 𝖼𝗋𝖾𝖺𝗍𝖾 𝖺 𝗇𝖺𝗆𝖾𝖽 𝗏𝗈𝗅𝗎𝗆𝖾 𝖻𝗒 𝗌𝗉𝖾𝖼𝗂𝖿𝗒𝗂𝗇𝗀 𝖺 𝗇𝖺𝗆𝖾
   - `𝖽𝗈𝖼𝗄𝖾𝗋 𝗋𝗎𝗇 --𝗇𝖺𝗆𝖾 <𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋_𝗇𝖺𝗆𝖾> -𝗏 <𝗏𝗈𝗅𝗎𝗆𝖾_𝗇𝖺𝗆𝖾>:<𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋_𝖽𝖺𝗍𝖺_𝗉𝖺𝗍𝗁> <𝗂𝗆𝖺𝗀𝖾_𝗇𝖺𝗆𝖾>`
     - `-𝗏` - 𝗍𝗁𝗂𝗌 𝖿𝗅𝖺𝗀 𝗂𝗌 𝗎𝗌𝖾𝖽 𝗍𝗈 𝗌𝗉𝖾𝖼𝗂𝖿𝗒 𝖺 𝗏𝗈𝗅𝗎𝗆𝖾 𝗆𝗈𝗎𝗇𝗍 𝗂𝗇 𝖺 𝖽𝗈𝖼𝗄𝖾𝗋 𝗋𝗎𝗇 𝖼𝗈𝗆𝗆𝖺𝗇𝖽.
     - `<𝗏𝗈𝗅𝗎𝗆𝖾_𝗇𝖺𝗆𝖾>` - 𝗍𝗁𝗂𝗌 𝗂𝗌 𝗍𝗁𝖾 𝗇𝖺𝗆𝖾 𝗈𝖿 𝗍𝗁𝖾 𝗏𝗈𝗅𝗎𝗆𝖾 𝗍𝗁𝖺𝗍 𝗒𝗈𝗎 𝗐𝖺𝗇𝗍 𝗍𝗈 𝗆𝗈𝗎𝗇𝗍 𝗂𝗇𝗍𝗈 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋. 𝖳𝗁𝗂𝗌 𝗂𝗌 𝖺 𝗇𝖺𝗆𝖾𝖽 𝗏𝗈𝗅𝗎𝗆𝖾 𝗍𝗁𝖺𝗍 𝗒𝗈𝗎 𝗁𝖺𝗏𝖾 𝖾𝗂𝗍𝗁𝖾𝗋 𝖼𝗋𝖾𝖺𝗍𝖾𝖽 𝖻𝖾𝖿𝗈𝗋𝖾𝗁𝖺𝗇𝖽 𝗎𝗌𝗂𝗇𝗀 `𝖽𝗈𝖼𝗄𝖾𝗋 𝗏𝗈𝗅𝗎𝗆𝖾 𝖼𝗋𝖾𝖺𝗍𝖾 <𝗏𝗈𝗅𝗎𝗆𝖾_𝗇𝖺𝗆𝖾>` 𝗈𝗋 𝖣𝗈𝖼𝗄𝖾𝗋 𝗐𝗂𝗅𝗅 𝖼𝗋𝖾𝖺𝗍𝖾 
     𝖺𝗎𝗍𝗈𝗆𝖺𝗍𝗂𝖼𝖺𝗅𝗅𝗒 𝗂𝖿 𝗂𝗍 𝖽𝗈𝖾𝗌𝗇'𝗍 𝖺𝗅𝗋𝖾𝖺𝖽𝗒 𝖾𝗑𝗂𝗌𝗍 𝗐𝗁𝖾𝗇 𝗒𝗈𝗎 𝗋𝗎𝗇 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋.
     - `<𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋_𝖽𝖺𝗍𝖺_𝗉𝖺𝗍𝗁>` - 𝗍𝗁𝗂𝗌 𝗂𝗌 𝗍𝗁𝖾 𝗉𝖺𝗍𝗁 𝗂𝗇𝗌𝗂𝖽𝖾 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗐𝗁𝖾𝗋𝖾 𝗍𝗁𝖾 𝗏𝗈𝗅𝗎𝗆𝖾 𝗐𝗂𝗅𝗅 𝖻𝖾 𝗆𝗈𝗎𝗇𝗍𝖾𝖽. <br> 𝖥𝗈𝗋 𝖺 𝖯𝗈𝗌𝗍𝗀𝗋𝖾𝖲𝖰𝖫 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋, `/𝗏𝖺𝗋/𝗅𝗂𝖻/𝗉𝗈𝗌𝗍𝗀𝗋𝖾𝗌𝗊𝗅/𝖽𝖺𝗍𝖺` 𝗂𝗌 𝗍𝗁𝖾 𝖽𝖾𝖿𝖺𝗎𝗅𝗍 𝗅𝗈𝖼𝖺𝗍𝗂𝗈𝗇 𝗐𝗁𝖾𝗋𝖾 𝖯𝗈𝗌𝗍𝗀𝗋𝖾𝖲𝖰𝖫 𝗌𝗍𝗈𝗋𝖾𝗌 𝗂𝗍𝗌 𝖽𝖺𝗍𝖺 𝖿𝗂𝗅𝖾𝗌. 𝖡𝗒 𝗆𝗈𝗎𝗇𝗍𝗂𝗇𝗀 𝖺 𝗏𝗈𝗅𝗎𝗆𝖾 
     𝖺𝗍 𝗍𝗁𝗂𝗌 𝗉𝖺𝗍𝗁, 𝗒𝗈𝗎 𝖾𝗇𝗌𝗎𝗋𝖾 𝗍𝗁𝖺𝗍 𝗍𝗁𝖾 𝖯𝗈𝗌𝗍𝗀𝗋𝖾𝖲𝖰𝖫 𝖽𝖺𝗍𝖺 𝗉𝖾𝗋𝗌𝗂𝗌𝗍𝗌 𝖺𝖼𝗋𝗈𝗌𝗌 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗋𝖾𝗌𝗍𝖺𝗋𝗍𝗌 𝖺𝗇𝖽 𝗋𝖾𝗆𝗈𝗏𝖺𝗅𝗌, 𝖻𝖾𝖼𝖺𝗎𝗌𝖾 𝗍𝗁𝖾 𝖽𝖺𝗍𝖺 𝗂𝗌 𝖺𝖼𝗍𝗎𝖺𝗅𝗅𝗒 𝗌𝗍𝗈𝗋𝖾𝖽 𝗈𝗇 𝗍𝗁𝖾 𝗁𝗈𝗌𝗍 𝗌𝗒𝗌𝗍𝖾𝗆 𝖺𝗇𝖽 𝗆𝖾𝗋𝖾𝗅𝗒 𝗅𝗂𝗇𝗄𝖾𝖽 𝗍𝗈 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋.
 - 𝖠𝗇𝗈𝗇𝗒𝗆𝗈𝗎𝗌 𝖵𝗈𝗅𝗎𝗆𝖾𝗌: 𝖳𝗁𝖾𝗒 𝖺𝗋𝖾 𝗏𝗈𝗅𝗎𝗆𝖾𝗌 𝗍𝗁𝖺𝗍 𝖺𝗋𝖾 𝗇𝗈𝗍 𝖾𝗑𝗉𝗅𝗂𝖼𝗂𝗍𝗅𝗒 𝗇𝖺𝗆𝖾𝖽 𝖻𝗒 𝗍𝗁𝖾 𝗎𝗌𝖾𝗋 𝗐𝗁𝖾𝗇 𝗍𝗁𝖾𝗒 𝖺𝗋𝖾 𝖼𝗋𝖾𝖺𝗍𝖾𝖽. <br>
   𝖳𝗁𝖾𝗒 𝖺𝗋𝖾 𝖺𝗎𝗍𝗈𝗆𝖺𝗍𝗂𝖼𝖺𝗅𝗅𝗒 𝖼𝗋𝖾𝖺𝗍𝖾𝖽 𝖻𝗒 𝖣𝗈𝖼𝗄𝖾𝗋 𝗐𝗁𝖾𝗇 𝖺 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗂𝗌 𝗋𝗎𝗇 𝖺𝗇𝖽 𝖺 𝗏𝗈𝗅𝗎𝗆𝖾 𝗂𝗌 𝗌𝗉𝖾𝖼𝗂𝖿𝗂𝖾𝖽 𝗐𝗂𝗍𝗁𝗈𝗎𝗍 𝖺 𝗇𝖺𝗆𝖾. <br>
   𝖠𝗇𝗈𝗇𝗒𝗆𝗈𝗎𝗌 𝗏𝗈𝗅𝗎𝗆𝖾𝗌 𝖺𝗋𝖾 𝗆𝖺𝗂𝗇𝗅𝗒 𝗎𝗌𝖾𝖽 𝖿𝗈𝗋 𝖽𝖺𝗍𝖺 𝗍𝗁𝖺𝗍 𝖽𝗈𝖾𝗌𝗇'𝗍 𝗇𝖾𝖾𝖽 𝗍𝗈 𝖻𝖾 𝗉𝖾𝗋𝗌𝗂𝗌𝗍𝖾𝖽 𝖺𝖿𝗍𝖾𝗋 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗂𝗌 𝗋𝖾𝗆𝗈𝗏𝖾𝖽 𝗈𝗋 𝖿𝗈𝗋 𝗍𝖾𝗆𝗉𝗈𝗋𝖺𝗋𝗒 𝖽𝖺𝗍𝖺 𝗍𝗁𝖺𝗍 𝗂𝗌 𝗌𝗉𝖾𝖼𝗂𝖿𝗂𝖼 𝗍𝗈 𝖺 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋'𝗌 𝗂𝗇𝗌𝗍𝖺𝗇𝖼𝖾.
   - `𝖽𝗈𝖼𝗄𝖾𝗋 𝗋𝗎𝗇 -𝗏 <𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋_𝖽𝖺𝗍𝖺_𝗉𝖺𝗍𝗁> <𝗂𝗆𝖺𝗀𝖾_𝗇𝖺𝗆𝖾>`

#### 𝖬𝖺𝗇𝖺𝗀𝗂𝗇𝗀 𝖵𝗈𝗅𝗎𝗆𝖾𝗌
- `𝖽𝗈𝖼𝗄𝖾𝗋 𝗏𝗈𝗅𝗎𝗆𝖾 𝖼𝗋𝖾𝖺𝗍𝖾 <𝗏𝗈𝗅𝗎𝗆𝖾_𝗇𝖺𝗆𝖾>` - 𝖼𝗋𝖾𝖺𝗍𝖾 𝖺 𝗇𝖾𝗐 𝗏𝗈𝗅𝗎𝗆𝖾.
- `𝖽𝗈𝖼𝗄𝖾𝗋 𝗏𝗈𝗅𝗎𝗆𝖾 𝗅𝗌` - 𝗅𝗂𝗌𝗍 𝖺𝗅𝗅 𝗏𝗈𝗅𝗎𝗆𝖾𝗌.
- `𝖽𝗈𝖼𝗄𝖾𝗋 𝗏𝗈𝗅𝗎𝗆𝖾 𝗂𝗇𝗌𝗉𝖾𝖼𝗍 <𝗏𝗈𝗅𝗎𝗆𝖾_𝗇𝖺𝗆𝖾>` - 𝗏𝗂𝖾𝗐 𝖽𝖾𝗍𝖺𝗂𝗅𝖾𝖽 𝗂𝗇𝖿𝗈𝗋𝗆𝖺𝗍𝗂𝗈𝗇 𝖺𝖻𝗈𝗎𝗍 𝖺 𝗏𝗈𝗅𝗎𝗆𝖾.
- `𝖽𝗈𝖼𝗄𝖾𝗋 𝗏𝗈𝗅𝗎𝗆𝖾 𝗋𝗆 <𝗏𝗈𝗅𝗎𝗆𝖾_𝗇𝖺𝗆𝖾>` - 𝗋𝖾𝗆𝗈𝗏𝖾 𝖺 𝗏𝗈𝗅𝗎𝗆𝖾.

> [!NOTE]
> 𝖵𝗈𝗅𝗎𝗆𝖾𝗌 𝖺𝗋𝖾 𝗇𝗈𝗍 𝖺𝗎𝗍𝗈𝗆𝖺𝗍𝗂𝖼𝖺𝗅𝗅𝗒 𝗋𝖾𝗆𝗈𝗏𝖾𝖽 𝗐𝗁𝖾𝗇 𝖺 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗂𝗌 𝗋𝖾𝗆𝗈𝗏𝖾𝖽, 𝗌𝗈 𝗍𝗁𝖾𝗒 𝗇𝖾𝖾𝖽 𝗍𝗈 𝖻𝖾 𝖼𝗅𝖾𝖺𝗇𝖾𝖽 𝗎𝗉 𝗆𝖺𝗇𝗎𝖺𝗅𝗅𝗒 𝗂𝖿 𝗇𝗈 𝗅𝗈𝗇𝗀𝖾𝗋 𝗇𝖾𝖾𝖽𝖾𝖽.

<br>
The same exapmle as before - "*𝖼𝗋𝖾𝖺𝗍𝖾 𝖺 𝗌𝖾𝗉𝖺𝗋𝖺𝗍𝖾 𝗇𝖾𝗍𝗐𝗈𝗋𝗄 𝖿𝗈𝗋 𝖺 𝗐𝖾𝖻𝖠𝗉𝗉 𝗐𝗂𝗍𝗁 𝖽𝖺𝗍𝖺𝖻𝖺𝗌𝖾*", but this time with volume for the database:

 - 𝖳𝗁𝖾 𝖼𝗈𝗆𝗆𝖺𝗇𝖽 𝖿𝗈𝗋 𝗍𝗁𝖾 𝗇𝖾𝗍𝗐𝗈𝗋𝗄 𝗂𝗌 𝗍𝗁𝖾 𝗌𝖺𝗆𝖾:
   ```console
   docker network create \
      --driver bridge \
      --subnet 192.168.0.0/24 \
      user-net
   ```
 - 𝖢𝗋𝖾𝖺𝗍𝖾 𝖺 𝖯𝗈𝗌𝗍𝗀𝗋𝖾𝗌 𝗂𝗇𝗌𝗍𝖺𝗇𝖼𝖾
   - 𝖯𝗎𝗅𝗅 𝗅𝖺𝗍𝖾𝗌𝗍 𝖯𝗈𝗌𝗍𝗀𝗋𝖾𝗌 𝗂𝗆𝖺𝗀𝖾
     ```console
     docker pull postgres
     ```
   - 𝖭𝖾𝗑𝗍 𝗐𝖾 𝖼𝖺𝗇 b𝗎𝗂𝗅𝖽 𝗉𝗈𝗌𝗍𝗀𝗋𝖾𝗌 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 and 𝖼𝗋𝖾𝖺𝗍𝖾 𝗍𝗁𝖾 𝗏𝗈𝗅𝗎𝗆𝖾 𝗂𝗇 𝗍𝗐𝗈 𝗐𝖺𝗒𝗌
     - 𝖥𝗂𝗋𝗌𝗍 𝖼𝗋𝖾𝖺𝗍𝗂𝗇𝗀 𝖺 𝖭𝖺𝗆𝖾𝖽 𝖵𝗈𝗅𝗎𝗆𝖾 𝖿𝗈𝗋 𝖯𝗈𝗌𝗍𝗀𝗋𝖾𝖲𝖰𝖫 𝖺𝗇𝖽 𝗍𝗁𝖾𝗇 𝖼𝗋𝖾𝖺𝗍𝖾 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋:
       ```console
         𝖽𝗈𝖼𝗄𝖾𝗋 𝗏𝗈𝗅𝗎𝗆𝖾 𝖼𝗋𝖾𝖺𝗍𝖾 𝗉𝗈𝗌𝗍𝗀𝗋𝖾𝗌-𝖽𝖻-𝗏𝗈𝗅𝗎𝗆𝖾
       ```
       ```console
          𝖽𝗈𝖼𝗄𝖾𝗋 𝗋𝗎𝗇 --𝗇𝖺𝗆𝖾 𝗉𝗈𝗌𝗍𝗀𝗋𝖾𝗌-𝖽𝖻 \
            -𝖾 𝖯𝖮𝖲𝖳𝖦𝖱𝖤𝖲_𝖴𝖲𝖤𝖱=𝗉𝗈𝗌𝗍𝗀𝗋𝖾𝗌 \
            -𝖾 𝖯𝖮𝖲𝖳𝖦𝖱𝖤𝖲_𝖯𝖠𝖲𝖲𝖶𝖮𝖱𝖣=𝟣𝟤𝟥𝟦𝟧𝟨𝟩𝟪 \
            -𝖾 𝖯𝖮𝖲𝖳𝖦𝖱𝖤𝖲_𝖣𝖡=𝗉𝗈𝗌𝗍𝗀𝗋𝖾𝗌_𝖽𝖻 \
            --𝗇𝖾𝗍𝗐𝗈𝗋𝗄 𝗎𝗌𝖾𝗋-𝗇𝖾𝗍 \
            -𝗏 𝗉𝗈𝗌𝗍𝗀𝗋𝖾𝗌-𝖽𝖻-𝗏𝗈𝗅𝗎𝗆𝖾:/𝗏𝖺𝗋/𝗅𝗂𝖻/𝗉𝗈𝗌𝗍𝗀𝗋𝖾𝗌𝗊𝗅/𝖽𝖺𝗍𝖺 \
            -𝗉 𝟧𝟦𝟥𝟤:𝟧𝟦𝟥𝟤 \
            --𝖽𝖾𝗍𝖺𝖼𝗁 \
            𝗉𝗈𝗌𝗍𝗀𝗋𝖾𝗌
       ```
     - 𝖮𝗋 𝗌𝗄𝗂𝗉 𝗍𝗁𝖾 `𝖽𝗈𝖼𝗄𝖾𝗋 𝗏𝗈𝗅𝗎𝗆𝖾 𝖼𝗋𝖾𝖺𝗍𝖾` 𝗌𝗍𝖾𝗉 𝖺𝗇𝖽 𝗃𝗎𝗌𝗍 𝖾𝗑𝖾𝖼𝗎𝗍𝖾 𝗍𝗁𝖾 `𝗋𝗎𝗇` 𝖼𝗈𝗆𝗆𝖺𝗇𝖽 𝗐𝗂𝗍𝗁 `-𝗏` 𝗍𝖺𝗀. 𝖳𝗁𝗂𝗌 𝗐𝖺𝗒 𝗂𝖿 𝗍𝗁𝖾 𝗏𝗈𝗅𝗎𝗆𝖾 𝖽𝗈𝖾𝗌𝗇'𝗍 𝖾𝗑𝗂𝗌𝗍, 𝖣𝗈𝖼𝗄𝖾𝗋 𝗐𝗂𝗅𝗅 𝖼𝗋𝖾𝖺𝗍𝖾 𝗂𝗍 𝖺𝗎𝗍𝗈𝗆𝖺𝗍𝗂𝖼𝖺𝗅𝗅𝗒.
       ```console
          𝖽𝗈𝖼𝗄𝖾𝗋 𝗋𝗎𝗇 --𝗇𝖺𝗆𝖾 𝗉𝗈𝗌𝗍𝗀𝗋𝖾𝗌-𝖽𝖻 \
            -𝖾 𝖯𝖮𝖲𝖳𝖦𝖱𝖤𝖲_𝖴𝖲𝖤𝖱=𝗉𝗈𝗌𝗍𝗀𝗋𝖾𝗌 \
            -𝖾 𝖯𝖮𝖲𝖳𝖦𝖱𝖤𝖲_𝖯𝖠𝖲𝖲𝖶𝖮𝖱𝖣=𝟣𝟤𝟥𝟦𝟧𝟨𝟩𝟪 \
            -𝖾 𝖯𝖮𝖲𝖳𝖦𝖱𝖤𝖲_𝖣𝖡=𝗉𝗈𝗌𝗍𝗀𝗋𝖾𝗌_𝖽𝖻 \
            --𝗇𝖾𝗍𝗐𝗈𝗋𝗄 𝗎𝗌𝖾𝗋-𝗇𝖾𝗍 \
            -𝗏 𝗉𝗈𝗌𝗍𝗀𝗋𝖾𝗌-𝖽𝖻-𝗏𝗈𝗅𝗎𝗆𝖾:/𝗏𝖺𝗋/𝗅𝗂𝖻/𝗉𝗈𝗌𝗍𝗀𝗋𝖾𝗌𝗊𝗅/𝖽𝖺𝗍𝖺 \
            -𝗉 𝟧𝟦𝟥𝟤:𝟧𝟦𝟥𝟤 \
            --𝖽𝖾𝗍𝖺𝖼𝗁 \
            𝗉𝗈𝗌𝗍𝗀𝗋𝖾𝗌
       ```
 - 𝖭𝖾𝗑𝗍 𝗌𝗍𝖾𝗉𝗌 𝖿𝗈𝗋 𝖼𝗋𝖾𝖺𝗍𝗂𝗇𝗀 𝖺 𝗐𝖾𝖻𝖠𝗉𝗉 𝗂𝗇𝗌𝗍𝖺𝗇𝖼𝖾 𝖺𝗋𝖾 𝗍𝗁𝖾 𝗌𝖺𝗆𝖾
   - 𝖡𝗎𝗂𝗅𝖽 𝗐𝖾𝖻𝖠𝗉𝗉 𝗂𝗆𝖺𝗀𝖾
     ```console
     docker build -t webapp-img .
     ```
   - 𝖡𝗎𝗂𝗅𝖽 𝗐𝖾𝖻𝖠𝗉𝗉 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋
     ```console
     docker run \
        --name webApp-container \
        --network user-net \
        -p 5000:5000 \
        --detach \
        webapp-img
     ```
 
 ---

## Compose

#### What is Docker Compose

To create and run containers, you use the command docker run . You can provide many configuration options, like --volume , --name , --publish , and more. <br>
Basically, Docker Compose is a tool to run docker commands from configuration files. Let’s consider the following command:

#### 𝖶𝗁𝖺𝗍 𝗂𝗌 𝖣𝗈𝖼𝗄𝖾𝗋 𝖢𝗈𝗆𝗉𝗈𝗌𝖾

𝖳𝗈 𝖼𝗋𝖾𝖺𝗍𝖾 𝖺𝗇𝖽 𝗋𝗎𝗇 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌, 𝗒𝗈𝗎 𝗎𝗌𝖾 𝗍𝗁𝖾 𝖼𝗈𝗆𝗆𝖺𝗇𝖽 𝖽𝗈𝖼𝗄𝖾𝗋 `𝗋𝗎𝗇`. 𝖸𝗈𝗎 𝖼𝖺𝗇 𝗉𝗋𝗈𝗏𝗂𝖽𝖾 𝗆𝖺𝗇𝗒 𝖼𝗈𝗇𝖿𝗂𝗀𝗎𝗋𝖺𝗍𝗂𝗈𝗇 𝗈𝗉𝗍𝗂𝗈𝗇𝗌, 𝗅𝗂𝗄𝖾 `--𝗏𝗈𝗅𝗎𝗆𝖾`, `--𝗇𝖺𝗆𝖾`, `--𝗉𝗎𝖻𝗅𝗂𝗌𝗁`, 𝖺𝗇𝖽 𝗆𝗈𝗋𝖾. <br>
𝖡𝖺𝗌𝗂𝖼𝖺𝗅𝗅𝗒, 𝖣𝗈𝖼𝗄𝖾𝗋 𝖢𝗈𝗆𝗉𝗈𝗌𝖾 𝗂𝗌 𝖺 𝗍𝗈𝗈𝗅 𝗍𝗈 𝗋𝗎𝗇 𝖽𝗈𝖼𝗄𝖾𝗋 𝖼𝗈𝗆𝗆𝖺𝗇𝖽𝗌 𝖿𝗋𝗈𝗆 𝖼𝗈𝗇𝖿𝗂𝗀𝗎𝗋𝖺𝗍𝗂𝗈𝗇 𝖿𝗂𝗅𝖾𝗌. <br>
𝖫𝖾𝗍’𝗌 𝖼𝗈𝗇𝗌𝗂𝖽𝖾𝗋 𝗍𝗁𝖾 𝖿𝗈𝗅𝗅𝗈𝗐𝗂𝗇𝗀 𝖼𝗈𝗆𝗆𝖺𝗇𝖽:

```console
  𝖽𝗈𝖼𝗄𝖾𝗋 𝗋𝗎𝗇 -𝗏 𝗆𝗒-𝗇𝖺𝗆𝖾𝖽-𝗏𝗈𝗅𝗎𝗆𝖾:/𝖽𝖺𝗍𝖺 -𝗉 𝟧𝟢𝟢𝟢:𝟧𝟢𝟢𝟢 --𝗇𝖺𝗆𝖾 𝗆𝗒-𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗆𝗒-𝗂𝗆𝖺𝗀𝖾
```

𝖳𝗁𝗂𝗌 𝖼𝗈𝗆𝗆𝖺𝗇𝖽 𝖼𝗋𝖾𝖺𝗍𝖾𝖽 𝖺 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗐𝗂𝗍𝗁 𝖺 𝗇𝖺𝗆𝖾𝖽 𝗏𝗈𝗅𝗎𝗆𝖾, 𝖺 𝗉𝗎𝖻𝗅𝗂𝗌𝗁𝖾𝖽 𝗉𝗈𝗋𝗍, 𝖺𝗇𝖽 𝖺 𝗇𝖺𝗆𝖾. 𝖸𝗈𝗎 𝖼𝖺𝗇 𝖺𝖼𝗁𝗂𝖾𝗏𝖾 𝗍𝗁𝖾 𝗌𝖺𝗆𝖾 𝗍𝗁𝗂𝗇𝗀 𝗐𝗂𝗍𝗁 𝖣𝗈𝖼𝗄𝖾𝗋 𝖢𝗈𝗆𝗉𝗈𝗌𝖾 𝗐𝗂𝗍𝗁 𝗍𝗁𝖾 𝖿𝗈𝗅𝗅𝗈𝗐𝗂𝗇𝗀 𝖼𝗈𝗇𝖿𝗂𝗀𝗎𝗋𝖺𝗍𝗂𝗈𝗇 𝖿𝗂𝗅𝖾:

```yaml
version: "3.0"
services:
  my-app:
    image: my-image
    container_name: my-container
    volumes:
      - my-named-volume:/data
    ports:
      - 5000:5000
```

> [!NOTE]
> Docker compose configuration file in most of the time is named docker-compose.yaml

From 𝗍𝗁𝖾 𝖽𝗂𝗋𝖾𝖼𝗍𝗈𝗋𝗒 𝗐𝗁𝖾𝗋𝖾 𝗍𝗁𝖾 𝖽𝗈𝖼𝗄𝖾𝗋-𝖼𝗈𝗆𝗉𝗈𝗌𝖾.𝗒𝗆𝗅 𝖿𝗂𝗅𝖾 𝗂𝗌 𝗅𝗈𝖼𝖺𝗍𝖾𝖽, we 𝖼𝖺𝗇 run the file and 𝖼𝗋𝖾𝖺𝗍𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋s 𝗐𝗂𝗍𝗁 𝗍𝗁𝖾 𝖿𝗈𝗅𝗅𝗈𝗐𝗂𝗇𝗀 𝖼𝗈𝗆𝗆𝖺𝗇𝖽:
```console
  docker compose up
```


#### Using Docker Compose

𝖠𝗌 𝖻𝖾𝖿𝗈𝗋𝖾, 𝗐𝖾 𝖼𝗋𝖾𝖺𝗍𝖾 𝖺 𝖣𝗈𝖼𝗄𝖾𝗋𝖿𝗂𝗅𝖾, 𝗐𝗂𝗍𝗁 𝗐𝗁𝗂𝖼𝗁 𝗐𝖾 𝖼𝗋𝖾𝖺𝗍𝖾 𝖺𝗇 𝗂𝗆𝖺𝗀𝖾. <br>
𝖠𝖿𝗍𝖾𝗋 𝗍𝗁𝖾 𝗂𝗆𝖺𝗀𝖾 𝗂𝗌 𝖼𝗋𝖾𝖺𝗍𝖾𝖽 𝗐𝗂𝗍𝗁 `𝖽𝗈𝖼𝗄𝖾𝗋 𝖻𝗎𝗂𝗅𝖽 -𝗍 <𝗒𝗈𝗎𝗋_𝗂𝗆𝖺𝗀𝖾_𝗇𝖺𝗆𝖾>:<𝗍𝖺𝗀> .` 𝖼𝗈𝗆𝗆𝖺𝗇𝖽, <br>
𝗐𝖾 𝖼𝖺𝗇 𝗎𝗌𝖾 𝖽𝗈𝖼𝗄𝖾𝗋 𝖼𝗈𝗆𝗉𝗈𝗌𝖾 𝗍𝗈 𝗋𝗎𝗇 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌:

 - 𝖥𝗂𝗋𝗌𝗍 𝗐𝖾 𝗇𝖾𝖾𝖽 𝗍𝗈 𝖼𝗋𝖾𝖺𝗍𝖾 `𝖽𝗈𝖼𝗄𝖾𝗋-𝖼𝗈𝗆𝗉𝗈𝗌𝖾.𝗒𝖺𝗆𝗅` 𝖿𝗂𝗅𝖾
   ```yaml
   𝗏𝖾𝗋𝗌𝗂𝗈𝗇: "𝟥.𝟪" # 𝖳𝗁𝖾 𝗏𝖾𝗋𝗌𝗂𝗈𝗇 𝖽𝗂𝖼𝗍𝖺𝗍𝖾𝗌 𝗐𝗁𝗂𝖼𝗁 𝖿𝖾𝖺𝗍𝗎𝗋𝖾𝗌 𝖺𝗇𝖽 𝗌𝗒𝗇𝗍𝖺𝗑 𝖺𝗋𝖾 𝖺𝗏𝖺𝗂𝗅𝖺𝖻𝗅𝖾 𝗂𝗇 𝗍𝗁𝖾 𝖢𝗈𝗆𝗉𝗈𝗌𝖾 𝖿𝗂𝗅𝖾

   # 𝖻𝖾𝗀𝗂𝗇𝗌 𝗍𝗁𝖾 𝖽𝖾𝖿𝗂𝗇𝗂𝗍𝗂𝗈𝗇 𝗈𝖿 𝗍𝗁𝖾 𝗌𝖾𝗋𝗏𝗂𝖼𝖾𝗌 𝗌𝖾𝖼𝗍𝗂𝗈𝗇. 𝖲𝖾𝗋𝗏𝗂𝖼𝖾𝗌 𝖽𝖾𝖿𝗂𝗇𝖾 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 𝗍𝗁𝖺𝗍 𝗇𝖾𝖾𝖽 𝗍𝗈 𝖻𝖾 𝖼𝗋𝖾𝖺𝗍𝖾𝖽
   𝗌𝖾𝗋𝗏𝗂𝖼𝖾𝗌:
     # 𝗌𝖾𝗋𝗏𝗂𝖼𝖾 is 𝖻𝖾𝗂𝗇𝗀 𝖽𝖾𝖿𝗂𝗇𝖾𝖽
     # t𝗁𝗂𝗌 𝗇𝖺𝗆𝖾 𝗂𝗌 𝗎𝗌𝖾𝖽 𝗂𝗇𝗍𝖾𝗋𝗇𝖺𝗅𝗅𝗒 𝖻𝗒 𝖣𝗈𝖼𝗄𝖾𝗋 𝖢𝗈𝗆𝗉𝗈𝗌𝖾 𝗍𝗈 𝗋𝖾𝖿𝖾𝗋 𝗍𝗈 𝗍𝗁𝗂𝗌 𝗉𝖺𝗋𝗍𝗂𝖼𝗎𝗅𝖺𝗋 𝖼𝗈𝗇𝖿𝗂𝗀𝗎𝗋𝖺𝗍𝗂𝗈𝗇
     𝗆𝗒-𝖺𝗉𝗉:
       # 𝗌𝗉𝖾𝖼𝗂𝖿𝗂𝖾𝗌 𝗍𝗁𝖾 𝖣𝗈𝖼𝗄𝖾𝗋 𝗂𝗆𝖺𝗀𝖾 𝖿𝗋𝗈𝗆 𝗐𝗁𝗂𝖼𝗁 𝗍𝗁𝖾 𝗌𝖾𝗋𝗏𝗂𝖼𝖾'𝗌 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗌𝗁𝗈𝗎𝗅𝖽 𝖻𝖾 𝖼𝗋𝖾𝖺𝗍𝖾𝖽
       𝗂𝗆𝖺𝗀𝖾: 𝗆𝗒-image
       # 𝖾𝗑𝗉𝗅𝗂𝖼𝗂𝗍𝗅𝗒 𝗌𝖾𝗍𝗌 𝗍𝗁𝖾 𝗇𝖺𝗆𝖾 𝗈𝖿 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗍𝗁𝖺𝗍 𝗐𝗂𝗅𝗅 𝖻𝖾 𝖼𝗋𝖾𝖺𝗍𝖾𝖽 𝖿𝗋𝗈𝗆 𝗍𝗁𝗂𝗌 𝗌𝖾𝗋𝗏𝗂𝖼𝖾
       𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋_𝗇𝖺𝗆𝖾: 𝗆𝗒-container
   ```
 - Add configuration options (𝖿𝗈𝗋 𝖾𝗑𝖺𝗆𝗉𝗅𝖾 𝖾𝗇𝗏𝗂𝗋𝗈𝗇𝗆𝖾𝗇𝗍 𝗏𝖺𝗋𝗂𝖺𝖻𝗅𝖾𝗌)
   ```yaml
   𝗏𝖾𝗋𝗌𝗂𝗈𝗇: "𝟥.𝟪"

   𝗌𝖾𝗋𝗏𝗂𝖼𝖾𝗌:
     𝗆𝗒-𝖺𝗉𝗉:
       𝗂𝗆𝖺𝗀𝖾: 𝗆𝗒-image
       𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋_𝗇𝖺𝗆𝖾: 𝗆𝗒-container
       # 𝗂𝗌 𝖺 𝗄𝖾𝗒 𝗍𝗁𝖺𝗍 𝗌𝗉𝖾𝖼𝗂𝖿𝗂𝖾𝗌 𝖺 𝖻𝗅𝗈𝖼𝗄 𝗈𝖿 𝖾𝗇𝗏𝗂𝗋𝗈𝗇𝗆𝖾𝗇𝗍 𝗏𝖺𝗋𝗂𝖺𝖻𝗅𝖾𝗌 𝗍𝗈 𝖻𝖾 𝗌𝖾𝗍 𝗐𝗂𝗍𝗁𝗂𝗇 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋
       𝖾𝗇𝗏𝗂𝗋𝗈𝗇𝗆𝖾𝗇𝗍:
         # 𝖽𝖾𝖿𝗂𝗇𝖾𝗌 𝖺𝗇 𝖾𝗇𝗏𝗂𝗋𝗈𝗇𝗆𝖾𝗇𝗍 𝗏𝖺𝗋𝗂𝖺𝖻𝗅𝖾 𝗇𝖺𝗆𝖾𝖽 𝖤𝖷𝖠𝖬𝖯𝖫𝖤_𝖵𝖠𝖱 𝗐𝗂𝗍𝗁 𝖺 𝗏𝖺𝗅𝗎𝖾 𝗈𝖿 "𝖾𝗑𝖺𝗆𝗉𝗅𝖾"
         𝖤𝖷𝖠𝖬𝖯𝖫𝖤_𝖵𝖠𝖱: "𝖾𝗑𝖺𝗆𝗉𝗅𝖾"
   ```
 - 𝖠𝖽𝖽 𝗏𝗈𝗅𝗎𝗆𝖾𝗌
   ```yaml
   𝗏𝖾𝗋𝗌𝗂𝗈𝗇: "𝟥.𝟪"

   𝗌𝖾𝗋𝗏𝗂𝖼𝖾𝗌:
     𝗆𝗒-𝖺𝗉𝗉:
       𝗂𝗆𝖺𝗀𝖾: 𝗆𝗒-image
       𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋_𝗇𝖺𝗆𝖾: 𝗆𝗒-container
       𝖾𝗇𝗏𝗂𝗋𝗈𝗇𝗆𝖾𝗇𝗍:
         𝖤𝖷𝖠𝖬𝖯𝖫𝖤_𝖵𝖠𝖱: "𝖾𝗑𝖺𝗆𝗉𝗅𝖾"
       # 𝗍𝗁𝗂𝗌 𝗄𝖾𝗒 𝗂𝗇𝖽𝗂𝖼𝖺𝗍𝖾𝗌 𝗍𝗁𝖾 𝗌𝗍𝖺𝗋𝗍 𝗈𝖿 𝗍𝗁𝖾 𝗏𝗈𝗅𝗎𝗆𝖾 𝖽𝖾𝖿𝗂𝗇𝗂𝗍𝗂𝗈𝗇𝗌 𝖿𝗈𝗋 𝗍𝗁𝖾 𝗌𝖾𝗋𝗏𝗂𝖼𝖾 𝗆𝗒-𝖺𝗉𝗉
       𝗏𝗈𝗅𝗎𝗆𝖾𝗌:
         # 𝗍𝗁𝖾 𝗇𝖺𝗆𝖾 𝗈𝖿 𝗍𝗁𝖾 𝗏𝗈𝗅𝗎𝗆𝖾
         # 𝖣𝗈𝖼𝗄𝖾𝗋 𝖢𝗈𝗆𝗉𝗈𝗌𝖾 𝗅𝗈𝗈𝗄𝗌 𝖿𝗈𝗋 𝖺 𝗏𝗈𝗅𝗎𝗆𝖾 𝗐𝗂𝗍𝗁 𝗍𝗁𝗂𝗌 𝗇𝖺𝗆𝖾
         # i𝖿 𝗂𝗍 𝖽𝗈𝖾𝗌𝗇'𝗍 𝖿𝗂𝗇𝖽 𝗈𝗇𝖾, 𝗂𝗍 𝖼𝗋𝖾𝖺𝗍𝖾𝗌 𝖺 𝗇𝖾𝗐 𝗇𝖺𝗆𝖾𝖽 𝗏𝗈𝗅𝗎𝗆𝖾 𝗐𝗂𝗍𝗁 𝗍𝗁𝗂𝗌 𝗇𝖺𝗆𝖾
         - 𝗆𝗒-𝗇𝖺𝗆𝖾𝖽-𝗏𝗈𝗅𝗎𝗆𝖾:/𝖽𝖺𝗍𝖺 
   ```

 #### 𝖬𝖺𝗄𝖾 𝖲𝖾𝗏𝖾𝗋𝖺𝗅 𝖢𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 𝖶𝗈𝗋𝗄 𝖶𝗂𝗍𝗁 𝖤𝖺𝖼𝗁 𝖮𝗍𝗁𝖾𝗋
   𝖳𝗁𝖾 𝗋𝖾𝖺𝗅 𝗌𝗍𝗋𝖾𝗇𝗀𝗍𝗁 𝗅𝗂𝖾𝗌 𝗂𝗇 𝗂𝗍𝗌 𝖺𝖻𝗂𝗅𝗂𝗍𝗒 𝗍𝗈 𝖾𝖺𝗌𝗂𝗅𝗒 𝗆𝖺𝗇𝖺𝗀𝖾 𝗆𝗎𝗅𝗍𝗂𝗉𝗅𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 𝖺𝗇𝖽 𝗆𝖺𝗄𝖾 𝗍𝗁𝖾𝗆 𝖼𝗈𝗆𝗆𝗎𝗇𝗂𝖼𝖺𝗍𝖾 𝗐𝗂𝗍𝗁 𝖾𝖺𝖼𝗁 𝗈𝗍𝗁𝖾𝗋.
   𝖫𝖾𝗍𝗌 𝖼𝗈𝗇𝗌𝗂𝖽𝖾𝗋 𝗍𝗁𝖾 𝗉𝗋𝖾𝗏𝗂𝗈𝗎𝗌 𝗌𝖾𝖼𝗍𝗂𝗈𝗇 𝖾𝗑𝖺𝗆𝗉𝗅𝖾 𝗂𝗇 𝗐𝗁𝗂𝖼𝗁 𝗐𝖾 𝗁𝖺𝗏𝖾 𝖺 𝗐𝖾𝖻𝖠𝗉𝗉 𝖺𝗇𝖽 𝗉𝗈𝗌𝗍𝗀𝗋𝖾𝗌 𝖽𝖺𝗍𝖺𝖻𝖺𝗌𝖾 𝗂𝗇 𝗍𝗁𝖾 𝗌𝖺𝗆𝖾 𝗇𝖾𝗍𝗐𝗈𝗋𝗄.
   - 𝖳𝗈 𝖻𝗎𝗂𝗅𝖽 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 𝗐𝗂𝗍𝗁 𝖽𝗈𝖼𝗄𝖾𝗋 𝖼𝗈𝗆𝗉𝗈𝗌𝖾 𝖿𝗂𝗋𝗌𝗍 𝗐𝖾 𝗇𝖾𝖾𝖽 𝗍𝗈 𝖺𝖽𝖽 𝗂𝗇 𝖽𝗈𝖼𝗄𝖾𝗋-𝖼𝗈𝗆𝗉𝗈𝗌𝖾.𝗒𝖺𝗆𝗅 𝖿𝗈𝗅𝗅𝗈𝗐𝗂𝗇𝗀 𝖼𝗈𝗆𝗉𝗈𝗇𝖾𝗇𝗍𝗌:
     - postgres database
       ```yaml
       postgres-db: # defines service for a PostgreSQL database
         image: postgres # specifies the Docker image to use for the service (latest)
         container_name: postgres-db # sets a custom name for the created container
         environment: # sets environment variables within the container
           POSTGRES_USER: postgres # username
           POSTGRES_PASSWORD: 12345678 # password
           POSTGRES_DB: postgres_db # database name
       ```
     - webApp
       ```yaml
       webapp: # defines service for webApp
         image: webapp-img # specifies the Docker image to use for the service (latest)
         build:
           # Specifies the build context - the starting point for the build.
           # The dot '.' represents the current directory
           # relative to the location of the docker-compose.yml file
           context: .
           # Indicates the path to the Dockerfile relative to the build context.
           # This path is used by Docker to find the Dockerfile
           # that contains the set of instructions for building the image
           dockerfile: path/to/Dockerfile
         container_name: webApp-container # sets environment variables within the container
       depends_on:
         - postgres-db # ensures webapp starts after the postgres-db service
       ports:
         - "5000:5000" # maps port 5000 inside the container to port 5000 on the host
       ```
     - network
       ```yaml
       networks: # defines the networks used by the services
         user-net: # creates a custom network named user-net
           driver: bridge # use the bridge driver for the network
           ipam: # Ip Address Management configuration
             config:
               - subnet: 192.168.0.0/24 # sets a custom subnet for the network
       ```
     - volume
       ```yaml
       volumes: # defines the volumes used by the services
         postgres-db-volume: # declares a named volume for the PostgreSQL data
       ```
   - Not we need to add `volume` for *postgres-db* and `network` for both *postgres-db* and *webApp*
       ```yaml
       volumes:
         - postgres-db-volume:/var/lib/postgresql/data # Mounts a named volume for data persistence
       ```
       ```yaml
       networks:
         - user-net # connects the service to a custom network
       ```
   - The final `docker-compose.yaml` file should look like this:
     ```yaml
     version: '3.8'

     services:
       postgres-db:
         image: postgres
         container_name: postgres-db
         environment:
           POSTGRES_USER: postgres
           POSTGRES_PASSWORD: 12345678
           POSTGRES_DB: postgres_db
         volumes:
           - postgres-db-volume:/var/lib/postgresql/data
         networks:
           - user-net

       webapp:
         image: webapp-img
         build: .
         container_name: webApp-container
         depends_on:
      - postgres-db
         ports:
           - "5000:5000"
         networks:
           - user-net

     volumes:
       postgres-db-volume:

     networks:
       user-net:
         driver: bridge
         ipam:
           config:
             - subnet: 192.168.0.0/24
     ```
<br>

# Kubernetes

### 𝖶𝗁𝖺𝗍 𝗂𝗌 Kubernetes?
𝖪𝗎𝖻𝖾𝗋𝗇𝖾𝗍𝖾𝗌 𝗂𝗌 𝖺𝗇 𝗈𝗉𝖾𝗇-𝗌𝗈𝗎𝗋𝖼𝖾 𝗉𝗅𝖺𝗍𝖿𝗈𝗋𝗆 𝖽𝖾𝗌𝗂𝗀𝗇𝖾𝖽 𝗍𝗈 𝖺𝗎𝗍𝗈𝗆𝖺𝗍𝖾 𝖽𝖾𝗉𝗅𝗈𝗒𝗂𝗇𝗀, 𝗌𝖼𝖺𝗅𝗂𝗇𝗀, 𝖺𝗇𝖽 𝗈𝗉𝖾𝗋𝖺𝗍𝗂𝗇𝗀 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌. <br>
𝖪𝗎𝖻𝖾𝗋𝗇𝖾𝗍𝖾𝗌 𝖺𝗂𝗆𝗌 𝗍𝗈 𝗉𝗋𝗈𝗏𝗂𝖽𝖾 𝖺 𝖿𝗋𝖺𝗆𝖾𝗐𝗈𝗋𝗄 𝖿𝗈𝗋 𝗋𝗎𝗇𝗇𝗂𝗇𝗀 𝖽𝗂𝗌𝗍𝗋𝗂𝖻𝗎𝗍𝖾𝖽 𝗌𝗒𝗌𝗍𝖾𝗆𝗌 𝗋𝖾𝗌𝗂𝗅𝗂𝖾𝗇𝗍𝗅𝗒
𝖪𝗎𝖻𝖾𝗋𝗇𝖾𝗍𝖾𝗌 𝗈𝗉𝖾𝗋𝖺𝗍𝖾𝗌 𝖻𝖺𝗌𝖾𝖽 𝗈𝗇 𝖺 𝖼𝗅𝗎𝗌𝗍𝖾𝗋 𝖺𝗋𝖼𝗁𝗂𝗍𝖾𝖼𝗍𝗎𝗋𝖾. <br>
𝖠 𝖼𝗅𝗎𝗌𝗍𝖾𝗋 𝖼𝗈𝗇𝗌𝗂𝗌𝗍𝗌 𝗈𝖿 𝖺𝗍 𝗅𝖾𝖺𝗌𝗍 𝗈𝗇𝖾 𝗆𝖺𝗌𝗍𝖾𝗋 𝗇𝗈𝖽𝖾 𝖺𝗇𝖽 𝗆𝗎𝗅𝗍𝗂𝗉𝗅𝖾 𝗐𝗈𝗋𝗄𝖾𝗋 𝗇𝗈𝖽𝖾𝗌. 𝖳𝗁𝖾 𝗆𝖺𝗌𝗍𝖾𝗋 𝗇𝗈𝖽𝖾 𝗂𝗌 𝗋𝖾𝗌𝗉𝗈𝗇𝗌𝗂𝖻𝗅𝖾 𝖿𝗈𝗋 𝗆𝖺𝗇𝖺𝗀𝗂𝗇𝗀 𝗍𝗁𝖾 𝗌𝗍𝖺𝗍𝖾 𝗈𝖿 𝗍𝗁𝖾 𝖼𝗅𝗎𝗌𝗍𝖾𝗋, 𝗂𝗇𝖼𝗅𝗎𝖽𝗂𝗇𝗀 𝗌𝖼𝗁𝖾𝖽𝗎𝗅𝗂𝗇𝗀 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇𝗌, 𝗌𝖼𝖺𝗅𝗂𝗇𝗀 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇𝗌, 𝖺𝗇𝖽 𝗋𝗈𝗅𝗅𝗂𝗇𝗀 𝗈𝗎𝗍 𝗇𝖾𝗐 𝗎𝗉𝖽𝖺𝗍𝖾𝗌.
- 𝖬𝖺𝗌𝗍𝖾𝗋 𝖭𝗈𝖽𝖾: 𝖳𝗁𝖾 𝖼𝗈𝗇𝗍𝗋𝗈𝗅 𝗉𝗅𝖺𝗇𝖾 𝗈𝖿 𝖺 𝖪𝗎𝖻𝖾𝗋𝗇𝖾𝗍𝖾𝗌 𝖼𝗅𝗎𝗌𝗍𝖾𝗋. 𝖨𝗍 𝗆𝖺𝗄𝖾𝗌 𝗀𝗅𝗈𝖻𝖺𝗅 𝖽𝖾𝖼𝗂𝗌𝗂𝗈𝗇𝗌 𝖺𝖻𝗈𝗎𝗍 𝗍𝗁𝖾 𝖼𝗅𝗎𝗌𝗍𝖾𝗋 (𝖿𝗈𝗋 𝖾𝗑𝖺𝗆𝗉𝗅𝖾, 𝗌𝖼𝗁𝖾𝖽𝗎𝗅𝗂𝗇𝗀), 𝖺𝗇𝖽 𝖽𝖾𝗍𝖾𝖼𝗍𝗌 𝖺𝗇𝖽 𝗋𝖾𝗌𝗉𝗈𝗇𝖽𝗌 𝗍𝗈 𝖼𝗅𝗎𝗌𝗍𝖾𝗋 𝖾𝗏𝖾𝗇𝗍𝗌
- 𝖶𝗈𝗋𝗄𝖾𝗋 𝖭𝗈𝖽𝖾𝗌: 𝖳𝗁𝖾𝗌𝖾 𝗇𝗈𝖽𝖾𝗌 𝖺𝖼𝗍𝗎𝖺𝗅𝗅𝗒 𝗋𝗎𝗇 𝗍𝗁𝖾 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇𝗌 𝖺𝗇𝖽 𝗐𝗈𝗋𝗄𝗅𝗈𝖺𝖽𝗌. 𝖤𝖺𝖼𝗁 𝗐𝗈𝗋𝗄𝖾𝗋 𝗇𝗈𝖽𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝗌 𝖺𝗅𝗅 𝗍𝗁𝖾 𝗌𝖾𝗋𝗏𝗂𝖼𝖾𝗌 𝗇𝖾𝖼𝖾𝗌𝗌𝖺𝗋𝗒 𝗍𝗈 𝗋𝗎𝗇 𝗉𝗈𝖽𝗌, 𝗆𝖺𝗇𝖺𝗀𝖾𝖽 𝖻𝗒 𝗍𝗁𝖾 𝗆𝖺𝗌𝗍𝖾𝗋 𝗇𝗈𝖽𝖾. 𝖳𝗁𝖾 𝗌𝖾𝗋𝗏𝗂𝖼𝖾𝗌 𝗂𝗇𝖼𝗅𝗎𝖽𝖾 𝗍𝗁𝖾 𝖣𝗈𝖼𝗄𝖾𝗋 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗋𝗎𝗇𝗍𝗂𝗆𝖾, 𝗄𝗎𝖻𝖾𝗅𝖾𝗍 (𝗐𝗁𝗂𝖼𝗁 𝖼𝗈𝗆𝗆𝗎𝗇𝗂𝖼𝖺𝗍𝖾𝗌 𝗐𝗂𝗍𝗁 𝗍𝗁𝖾 𝗆𝖺𝗌𝗍𝖾𝗋 𝗇𝗈𝖽𝖾), 𝖺𝗇𝖽 𝗄𝗎𝖻𝖾-𝗉𝗋𝗈𝗑𝗒 (𝖺 𝗇𝖾𝗍𝗐𝗈𝗋𝗄 𝗉𝗋𝗈𝗑𝗒 𝗋𝖾𝖿𝗅𝖾𝖼𝗍𝗂𝗇𝗀 𝗌𝖾𝗋𝗏𝗂𝖼𝖾𝗌 𝖺𝗌 𝖽𝖾𝖿𝗂𝗇𝖾𝖽 𝗂𝗇 𝖪𝗎𝖻𝖾𝗋𝗇𝖾𝗍𝖾𝗌 𝗈𝗇 𝖾𝖺𝖼𝗁 𝗇𝗈𝖽𝖾).


### Kubernetes Basic Architecture

𝖪𝗎𝖻𝖾𝗋𝗇𝖾𝗍𝖾𝗌 𝗆𝖺𝗇𝖺𝗀𝖾𝗌 𝖺𝗇𝖽 𝗈𝗋𝗀𝖺𝗇𝗂𝗓𝖾𝗌 𝖺𝗉𝗉𝗌 𝗍𝗁𝖺𝗍 𝖺𝗋𝖾 𝗉𝖺𝖼𝗄𝖾𝖽 𝗂𝗇 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 𝖻𝗒 𝗎𝗌𝗂𝗇𝗀 𝖺 𝖼𝗅𝗎𝗌𝗍𝖾𝗋. <br>
𝖠 𝖼𝗅𝗎𝗌𝗍𝖾𝗋 𝗂𝗌 𝖺 𝖼𝗈𝗅𝗅𝖾𝖼𝗍𝗂𝗈𝗇 𝗈𝖿 𝗆𝖺𝖼𝗁𝗂𝗇𝖾𝗌 𝗍𝗁𝖺𝗍 𝗐𝗈𝗋𝗄 𝗍𝗈𝗀𝖾𝗍𝗁𝖾𝗋 𝖺𝗌 𝖺 𝗌𝗂𝗇𝗀𝗅𝖾 𝗎𝗇𝗂𝗍 𝗍𝗈 𝖾𝗇𝗌𝗎𝗋𝖾 𝗍𝗁𝖺𝗍 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇𝗌 𝗋𝗎𝗇 𝗌𝗆𝗈𝗈𝗍𝗁𝗅𝗒 𝖺𝗇𝖽 𝖾𝖿𝖿𝗂𝖼𝗂𝖾𝗇𝗍𝗅𝗒. <br>
𝖳𝗁𝖾 𝖪𝗎𝖻𝖾𝗋𝗇𝖾𝗍𝖾𝗌 𝖼𝗅𝗎𝗌𝗍𝖾𝗋 𝗂𝗌 𝗆𝖺𝖽𝖾 𝖻𝗒 𝖺𝗍 𝗅𝖾𝖺𝗌𝗍 𝗈𝗇𝖾 𝗆𝖺𝗌𝗍𝖾𝗋 𝗇𝗈𝖽𝖾 𝖺𝗇𝖽 𝖼𝗈𝗇𝗇𝖾𝖼𝗍𝖾𝖽 𝗍𝗈 𝗂𝗍 𝗒𝗈𝗎 𝗁𝖺𝗏𝖾 𝖼𝗈𝗎𝗉𝗅𝖾 𝗈𝖿 𝗐𝗈𝗋𝗄𝖾𝗋 𝗇𝗈𝖽𝖾𝗌.

#### 𝖢𝗈𝗇𝗍𝗋𝗈𝗅 𝖯𝗅𝖺𝗇𝖾 (𝖬𝖺𝗌𝗍𝖾𝗋)
𝖳𝗁𝖾 𝖼𝗈𝗇𝗍𝗋𝗈𝗅 𝗉𝗅𝖺𝗇𝖾 𝗆𝖺𝗇𝖺𝗀𝖾𝗌 𝗍𝗁𝖾 𝖼𝗅𝗎𝗌𝗍𝖾𝗋 𝖺𝗇𝖽 𝗂𝗌 𝗋𝖾𝗌𝗉𝗈𝗇𝗌𝗂𝖻𝗅𝖾 𝖿𝗈𝗋 𝗆𝖺𝗂𝗇𝗍𝖺𝗂𝗇𝗂𝗇𝗀 𝗍𝗁𝖾 𝖽𝖾𝗌𝗂𝗋𝖾𝖽 𝗌𝗍𝖺𝗍𝖾 𝗈𝖿 𝗍𝗁𝖾 𝖼𝗅𝗎𝗌𝗍𝖾𝗋, 𝗌𝗎𝖼𝗁 𝖺𝗌 𝗐𝗁𝗂𝖼𝗁 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇𝗌 𝖺𝗋𝖾 𝗋𝗎𝗇𝗇𝗂𝗇𝗀 𝖺𝗇𝖽 𝗍𝗁𝖾𝗂𝗋 𝖼𝗈𝗋𝗋𝖾𝗌𝗉𝗈𝗇𝖽𝗂𝗇𝗀 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗂𝗆𝖺𝗀𝖾𝗌. 𝖨𝗍 𝖺𝗅𝗌𝗈 𝗆𝖺𝗇𝖺𝗀𝖾𝗌 𝗇𝖾𝗍𝗐𝗈𝗋𝗄𝗂𝗇𝗀, 𝗌𝖼𝖺𝗅𝗂𝗇𝗀, 𝖺𝗇𝖽 𝖽𝖾𝗉𝗅𝗈𝗒𝗆𝖾𝗇𝗍 𝖼𝗈𝗇𝖿𝗂𝗀𝗎𝗋𝖺𝗍𝗂𝗈𝗇𝗌. <br>
𝖳𝗁𝖾 𝖼𝗈𝗇𝗍𝗋𝗈𝗅 𝗉𝗅𝖺𝗇𝖾 𝖼𝗈𝗇𝗌𝗂𝗌𝗍 𝗈𝖿 𝗌𝖾𝗏𝖾𝗋𝖺𝗅 𝗉𝗋𝗈𝖼𝖾𝗌𝗌𝖾𝗌:
- 𝖠𝗉𝗂 𝖲𝖾𝗋𝗏𝖾𝗋 (`𝗄𝗎𝖻𝖾-𝖺𝗉𝗂𝗌𝖾𝗋𝗏𝖾𝗋`) - 𝖾𝗇𝗍𝗋𝗒𝗉𝗈𝗂𝗇𝗍 𝗍𝗈 𝗍𝗁𝖾 𝖪𝗎𝖻𝖾𝗋𝗇𝖾𝗍𝖾𝗌 𝖼𝗅𝗎𝗌𝗍𝖾𝗋
- 𝖢𝗈𝗇𝗍𝗋𝗈𝗅𝗅𝖾𝗋 𝖬𝖺𝗇𝖺𝗀𝖾𝗋 (`𝗄𝗎𝖻𝖾-𝖼𝗈𝗇𝗍𝗋𝗈𝗅𝗅𝖾𝗋-𝗆𝖺𝗇𝖺𝗀𝖾𝗋`) - 𝗄𝖾𝖾𝗉𝗌 𝗍𝗋𝖺𝖼𝗄 𝗈𝖿 𝗐𝗁𝖺𝗍 𝗁𝖺𝗉𝗉𝖾𝗇𝗂𝗇𝗀 𝗂𝗇 𝗍𝗁𝖾 𝖼𝗅𝗎𝗌𝗍𝖾𝗋
- 𝖲𝖼𝗁𝖾𝖽𝗎𝗅𝖾𝗋 (`𝗄𝗎𝖻𝖾-𝗌𝖼𝗁𝖾𝖽𝗎𝗅𝖾𝗋`) - 𝗌𝖼𝗁𝖾𝖽𝗎𝗅𝗂𝗇𝗀 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗈𝗇 𝖽𝗂𝖿𝖿𝖾𝗋𝖾𝗇𝗍 𝗇𝗈𝖽𝖾𝗌 𝖻𝖺𝗌𝖾𝖽 𝗈𝗇 𝗍𝗁𝖾 𝗐𝗈𝗋𝗄𝗅𝗈𝖺𝖽 𝖺𝗇𝖽 𝖺𝗏𝖺𝗂𝗅𝖺𝖻𝗅𝖾 𝗋𝖾𝗌𝗈𝗎𝗋𝖼𝖾𝗌. 𝖡𝖺𝗌𝗂𝖼𝖺𝗅𝗅𝗒 𝗂𝗍 𝖽𝖾𝖼𝗂𝖽𝖾𝗌 𝗈𝗇 𝗐𝗁𝗂𝖼𝗁 𝗐𝗈𝗋𝗄𝖾𝗋 𝗇𝗈𝖽𝖾 𝗍𝗁𝖾 𝗇𝖾𝗑𝗍 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗌𝗁𝗈𝗎𝗅𝖽 𝖻𝖾 𝗌𝖼𝗁𝖾𝖽𝗎𝗅𝖾𝖽.
- `𝖾𝗍𝖼𝖽` - 𝖪𝗎𝖻𝖾𝗋𝗇𝖾𝗍𝖾𝗌 𝖻𝖺𝖼𝗄𝗂𝗇𝗀 𝗄𝖾𝗒-𝗏𝖺𝗅𝗎𝖾 𝗌𝗍𝗈𝗋𝖾. 𝖧𝗈𝗅𝖽𝗌 𝖺𝗍 𝖺𝗇𝗒 𝗍𝗂𝗆𝖾 𝗍𝗁𝖾 𝖼𝗎𝗋𝗋𝖾𝗇𝗍 𝗌𝗍𝖺𝗍𝖾 𝗈𝖿 𝗍𝗁𝖾 𝖪𝗎𝖻𝖾𝗋𝗇𝖾𝗍𝖾𝗌 𝖼𝗅𝗎𝗌𝗍𝖾𝗋.

#### 𝖶𝗈𝗋𝗄𝖾𝗋 𝖭𝗈𝖽𝖾
𝖶𝗈𝗋𝗄𝖾𝗋𝗌 (𝗈𝗋 𝗐𝗈𝗋𝗄𝖾𝗋 𝗇𝗈𝖽𝖾𝗌) 𝖺𝗋𝖾 𝗍𝗁𝖾 𝗆𝖺𝖼𝗁𝗂𝗇𝖾𝗌 𝗂𝗇 𝗍𝗁𝖾 𝖼𝗅𝗎𝗌𝗍𝖾𝗋 𝗍𝗁𝖺𝗍 𝖺𝖼𝗍𝗎𝖺𝗅𝗅𝗒 𝗋𝗎𝗇 𝗍𝗁𝖾 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇𝗌 𝖺𝗇𝖽 𝗐𝗈𝗋𝗄𝗅𝗈𝖺𝖽𝗌. 𝖤𝖺𝖼𝗁 𝗐𝗈𝗋𝗄𝖾𝗋 𝗁𝖺𝗌 𝖺 𝗌𝖾𝗍 𝗈𝖿 𝖼𝗈𝗆𝗉𝗈𝗇𝖾𝗇𝗍𝗌 𝗇𝖾𝖼𝖾𝗌𝗌𝖺𝗋𝗒 𝖿𝗈𝗋 𝗍𝗁𝗂𝗌 𝗍𝖺𝗌𝗄, 𝗂𝗇𝖼𝗅𝗎𝖽𝗂𝗇𝗀 𝖺 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗋𝗎𝗇𝗍𝗂𝗆𝖾 𝖿𝗈𝗋 𝗋𝗎𝗇𝗇𝗂𝗇𝗀 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 𝖺𝗇𝖽 𝖺𝗀𝖾𝗇𝗍𝗌 (𝗅𝗂𝗄𝖾 𝗄𝗎𝖻𝖾𝗅𝖾𝗍 𝖺𝗇𝖽 𝗄𝗎𝖻𝖾-𝗉𝗋𝗈𝗑𝗒) 𝗍𝗁𝖺𝗍 𝖼𝗈𝗆𝗆𝗎𝗇𝗂𝖼𝖺𝗍𝖾 𝗐𝗂𝗍𝗁 𝗍𝗁𝖾 𝗆𝖺𝗌𝗍𝖾𝗋 𝗍𝗈 𝗋𝖾𝖼𝖾𝗂𝗏𝖾 𝗂𝗇𝗌𝗍𝗋𝗎𝖼𝗍𝗂𝗈𝗇𝗌 𝖺𝗇𝖽 𝗆𝖺𝗇𝖺𝗀𝖾 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 𝖺𝗇𝖽 𝗇𝖾𝗍𝗐𝗈𝗋𝗄𝗂𝗇𝗀 𝗈𝗇 𝗍𝗁𝖾 𝗇𝗈𝖽𝖾.
- 𝖭𝗈𝖽𝖾 𝖺𝗋𝖼𝗁𝗂𝗍𝖾𝖼𝗍𝗎𝗋𝖾:
- 𝖯𝗈𝖽: 𝖳𝗁𝖾 𝗌𝗆𝖺𝗅𝗅𝖾𝗌𝗍 𝖽𝖾𝗉𝗅𝗈𝗒𝖺𝖻𝗅𝖾 𝗎𝗇𝗂𝗍𝗌 𝗂𝗇 𝖪𝗎𝖻𝖾𝗋𝗇𝖾𝗍𝖾𝗌, 𝖾𝖺𝖼𝗁 𝖯𝗈𝖽 𝖾𝗇𝖼𝖺𝗉𝗌𝗎𝗅𝖺𝗍𝖾𝗌 𝗈𝗇𝖾 𝗈𝗋 𝗆𝗈𝗋𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌, 𝗉𝗋𝗈𝗏𝗂𝖽𝗂𝗇𝗀 𝗍𝗁𝖾𝗆 𝗐𝗂𝗍𝗁 𝖺 𝗎𝗇𝗂𝗊𝗎𝖾 𝖨𝖯 𝖺𝖽𝖽𝗋𝖾𝗌𝗌 𝖺𝗇𝖽 𝗌𝗍𝗈𝗋𝖺𝗀𝖾 𝗋𝖾𝗌𝗈𝗎𝗋𝖼𝖾𝗌.
- 𝖢𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝖱𝗎𝗇𝗍𝗂𝗆𝖾: 𝖳𝗁𝖾 𝗎𝗇𝖽𝖾𝗋𝗅𝗒𝗂𝗇𝗀 𝗌𝗈𝖿𝗍𝗐𝖺𝗋𝖾 𝗎𝗌𝖾𝖽 𝗍𝗈 𝗋𝗎𝗇 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 (𝖾.𝗀., 𝖣𝗈𝖼𝗄𝖾𝗋, 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝖽).
- 𝗄𝗎𝖻𝖾𝗅𝖾𝗍: 𝖠𝗇 𝖺𝗀𝖾𝗇𝗍 𝗋𝗎𝗇𝗇𝗂𝗇𝗀 𝗈𝗇 𝖾𝖺𝖼𝗁 𝗇𝗈𝖽𝖾, 𝖾𝗇𝗌𝗎𝗋𝗂𝗇𝗀 𝗍𝗁𝖺𝗍 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 𝖺𝗋𝖾 𝗋𝗎𝗇𝗇𝗂𝗇𝗀 𝗂𝗇 𝖺 𝖯𝗈𝖽.
- 𝗄𝗎𝖻𝖾-𝗉𝗋𝗈𝗑𝗒: 𝖬𝖺𝗇𝖺𝗀𝖾𝗌 𝗇𝖾𝗍𝗐𝗈𝗋𝗄𝗂𝗇𝗀 𝗈𝗇 𝖾𝖺𝖼𝗁 𝗇𝗈𝖽𝖾, 𝖺𝗅𝗅𝗈𝗐𝗂𝗇𝗀 𝗍𝗁𝖾 𝖯𝗈𝖽𝗌 𝗍𝗈 𝖼𝗈𝗆𝗆𝗎𝗇𝗂𝖼𝖺𝗍𝖾 𝗐𝗂𝗍𝗁 𝖾𝖺𝖼𝗁 𝗈𝗍𝗁𝖾𝗋 𝖺𝗇𝖽 𝗍𝗁𝖾 𝗈𝗎𝗍𝗌𝗂𝖽𝖾 𝗐𝗈𝗋𝗅𝖽.

#### 𝖯𝗈𝖽𝗌
𝖨𝗍`𝗌 𝖻𝖺𝗌𝗂𝖼𝖺𝗅𝗅𝗒 𝖺𝗇 𝖺𝖻𝗌𝗍𝗋𝖺𝖼𝗍𝗂𝗈𝗇 𝗈𝗏𝖾𝗋 𝖺 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋. 𝖨𝗍 𝖼𝗋𝖾𝖺𝗍𝖾𝖽 𝖺 𝗋𝗎𝗇𝗇𝗂𝗇𝗀 𝖾𝗇𝗏𝗂𝗋𝗈𝗇𝗆𝖾𝗇𝗍 𝗈𝗋 𝖺 𝗅𝖺𝗒𝖾𝗋 𝗈𝗇 𝗍𝗈𝗉 𝗈𝖿 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝖻𝖾𝖼𝖺𝗎𝗌𝖾 𝖪𝗎𝖻𝖾𝗋𝗇𝖾𝗍𝖾𝗌 𝖺𝖻𝗌𝗍𝗋𝖺𝖼𝗍 𝗍𝗁𝖾 𝗋𝗎𝗇𝗍𝗂𝗆𝖾 𝗈𝖿 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋.
- 𝖠 𝖯𝗈𝖽 𝖼𝗈𝗇𝗌𝗂𝗌𝗍𝗌 𝗈𝖿 𝗈𝗇𝖾 𝗈𝗋 𝗆𝗈𝗋𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 𝗍𝗁𝖺𝗍 𝗌𝗁𝖺𝗋𝖾 𝗋𝖾𝗌𝗈𝗎𝗋𝖼𝖾𝗌 𝖺𝗇𝖽 𝖺𝗋𝖾 𝖼𝗈𝗅𝗈𝖼𝖺𝗍𝖾𝖽 𝗈𝗇 𝗍𝗁𝖾 𝗁𝗈𝗌𝗍 𝗆𝖺𝖼𝗁𝗂𝗇𝖾.
- 𝖠𝗅𝗅 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 𝗐𝗂𝗅𝗅 𝗋𝗎𝗇 𝗂𝗇 𝖺 𝗉𝗈𝖽. 𝖯𝗈𝖽𝗌 𝖺𝖻𝗌𝗍𝗋𝖺𝖼𝗍 𝗍𝗁𝖾 𝗇𝖾𝗍𝗐𝗈𝗋𝗄 𝖺𝗇𝖽 𝗌𝗍𝗈𝗋𝖺𝗀𝖾 𝖺𝗐𝖺𝗒 𝖿𝗋𝗈𝗆 𝗍𝗁𝖾 𝗎𝗇𝖽𝖾𝗋𝗅𝗒𝗂𝗇𝗀 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌.
- 𝖤𝖺𝖼𝗁 𝗉𝗈𝖽 𝗁𝖺𝗌 𝗈𝗇𝖾 𝗎𝗇𝗂𝗊𝗎𝖾 𝖨𝖯 𝖺𝖽𝖽𝗋𝖾𝗌𝗌 𝖺𝗌𝗌𝗂𝗀𝗇𝖾𝖽.

#### Services
𝖤𝖺𝖼𝗁 𝖯𝗈𝖽 𝗂𝗌 𝖺𝗌𝗌𝗂𝗀𝗇𝖾𝖽 𝖺 𝗎𝗇𝗂𝗊𝗎𝖾 𝖨𝖯 𝖺𝖽𝖽𝗋𝖾𝗌𝗌 𝗐𝗂𝗍𝗁𝗂𝗇 𝗍𝗁𝖾 𝖪𝗎𝖻𝖾𝗋𝗇𝖾𝗍𝖾𝗌 𝖼𝗅𝗎𝗌𝗍𝖾𝗋, 𝗐𝗁𝗂𝖼𝗁 𝖺𝗅𝗅𝗈𝗐𝗌 𝖿𝗈𝗋 𝖽𝗂𝗋𝖾𝖼𝗍 𝗉𝗈𝖽-𝗍𝗈-𝗉𝗈𝖽 𝖼𝗈𝗆𝗆𝗎𝗇𝗂𝖼𝖺𝗍𝗂𝗈𝗇. <br>
𝖧𝗈𝗐𝖾𝗏𝖾𝗋, 𝖯𝗈𝖽𝗌 𝖺𝗋𝖾 𝖾𝗉𝗁𝖾𝗆𝖾𝗋𝖺𝗅; 𝗍𝗁𝖾𝗒 𝖼𝖺𝗇 𝖻𝖾 𝖼𝗋𝖾𝖺𝗍𝖾𝖽, 𝖽𝖾𝗌𝗍𝗋𝗈𝗒𝖾𝖽, 𝖺𝗇𝖽 𝗋𝖾𝗉𝗅𝖺𝖼𝖾𝖽 𝖻𝗒 𝖪𝗎𝖻𝖾𝗋𝗇𝖾𝗍𝖾𝗌 𝗍𝗈 𝗆𝖺𝗇𝖺𝗀𝖾 𝗍𝗁𝖾 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇'𝗌 𝗌𝗍𝖺𝗍𝖾. <br>
𝖳𝗁𝗂𝗌 𝗆𝖾𝖺𝗇𝗌 𝗍𝗁𝖾𝗂𝗋 𝖨𝖯 𝖺𝖽𝖽𝗋𝖾𝗌𝗌𝖾𝗌 𝖼𝖺𝗇 𝖼𝗁𝖺𝗇𝗀𝖾 𝗈𝗏𝖾𝗋 𝗍𝗂𝗆𝖾, 𝖾𝗌𝗉𝖾𝖼𝗂𝖺𝗅𝗅𝗒 𝗐𝗁𝖾𝗇 𝖺 𝖯𝗈𝖽 𝖼𝗋𝖺𝗌𝗁𝖾𝗌 𝖺𝗇𝖽 𝖺 𝗇𝖾𝗐 𝗈𝗇𝖾 𝗂𝗌 𝖼𝗋𝖾𝖺𝗍𝖾𝖽 𝗍𝗈 𝗋𝖾𝗉𝗅𝖺𝖼𝖾 𝗂𝗍.

𝖳𝗁𝗂𝗌 𝗂𝗌 𝗐𝗁𝖾𝗋𝖾 𝖲𝖾𝗋𝗏𝗂𝖼𝖾𝗌 𝖼𝗈𝗆𝖾 𝗂𝗇. 𝖠 𝖲𝖾𝗋𝗏𝗂𝖼𝖾 𝗂𝗇 𝖪𝗎𝖻𝖾𝗋𝗇𝖾𝗍𝖾𝗌 𝗂𝗌 𝖺𝗇 𝖺𝖻𝗌𝗍𝗋𝖺𝖼𝗍𝗂𝗈𝗇 𝗐𝗁𝗂𝖼𝗁 𝖽𝖾𝖿𝗂𝗇𝖾𝗌 𝖺 𝗅𝗈𝗀𝗂𝖼𝖺𝗅 𝗌𝖾𝗍 𝗈𝖿 𝖯𝗈𝖽𝗌 𝖺𝗇𝖽 𝖺 𝗉𝗈𝗅𝗂𝖼𝗒 𝖻𝗒 𝗐𝗁𝗂𝖼𝗁 𝗍𝗈 𝖺𝖼𝖼𝖾𝗌𝗌 𝗍𝗁𝖾𝗆. <br>
𝖳𝗁𝖾 𝗄𝖾𝗒 𝖻𝖾𝗇𝖾𝖿𝗂𝗍𝗌 𝗈𝖿 𝖲𝖾𝗋𝗏𝗂𝖼𝖾𝗌 𝗂𝗇𝖼𝗅𝗎𝖽𝖾:
- 𝖲𝗍𝖺𝖻𝗅𝖾 𝖨𝖯 𝖺𝖽𝖽𝗋𝖾𝗌𝗌: 𝖲𝖾𝗋𝗏𝗂𝖼𝖾𝗌 𝗉𝗋𝗈𝗏𝗂𝖽𝖾 𝖺 𝗌𝗂𝗇𝗀𝗅𝖾, 𝗌𝗍𝖺𝖻𝗅𝖾 𝖨𝖯 𝖺𝖽𝖽𝗋𝖾𝗌𝗌 𝗍𝗁𝖺𝗍 𝖼𝗅𝗂𝖾𝗇𝗍𝗌 𝖼𝖺𝗇 𝗎𝗌𝖾 𝗍𝗈 𝖼𝗈𝗆𝗆𝗎𝗇𝗂𝖼𝖺𝗍𝖾 𝗐𝗂𝗍𝗁 𝗍𝗁𝖾 𝖯𝗈𝖽𝗌 𝗂𝗇 𝗍𝗁𝖾 𝖲𝖾𝗋𝗏𝗂𝖼𝖾, 𝗋𝖾𝗀𝖺𝗋𝖽𝗅𝖾𝗌𝗌 𝗈𝖿 𝗍𝗁𝖾 𝗂𝗇𝖽𝗂𝗏𝗂𝖽𝗎𝖺𝗅 𝖯𝗈𝖽'𝗌 𝗅𝗂𝖿𝖾 𝖼𝗒𝖼𝗅𝖾. 𝖳𝗁𝗂𝗌 𝗆𝖾𝖺𝗇𝗌 𝗒𝗈𝗎 𝖽𝗈𝗇'𝗍 𝗁𝖺𝗏𝖾 𝗍𝗈 𝗋𝖾𝖼𝗈𝗇𝖿𝗂𝗀𝗎𝗋𝖾 𝗒𝗈𝗎𝗋 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇𝗌 𝖾𝗏𝖾𝗋𝗒 𝗍𝗂𝗆𝖾 𝖺 𝖯𝗈𝖽 𝗂𝗌 𝗋𝖾𝗉𝗅𝖺𝖼𝖾𝖽.
- 𝖫𝗈𝖺𝖽 𝖻𝖺𝗅𝖺𝗇𝖼𝗂𝗇𝗀: 𝖶𝗁𝖾𝗇 𝗆𝗎𝗅𝗍𝗂𝗉𝗅𝖾 𝖯𝗈𝖽𝗌 𝗆𝖺𝗍𝖼𝗁 𝗍𝗁𝖾 𝖲𝖾𝗋𝗏𝗂𝖼𝖾'𝗌 𝗌𝖾𝗅𝖾𝖼𝗍𝗈𝗋, 𝗍𝗁𝖾 𝖲𝖾𝗋𝗏𝗂𝖼𝖾 𝗅𝗈𝖺𝖽 𝖻𝖺𝗅𝖺𝗇𝖼𝖾𝗌 𝗍𝗁𝖾 𝗍𝗋𝖺𝖿𝖿𝗂𝖼 𝖺𝗆𝗈𝗇𝗀 𝗍𝗁𝖾𝗆, 𝗉𝗋𝗈𝗏𝗂𝖽𝗂𝗇𝗀 𝗋𝖾𝗅𝗂𝖺𝖻𝗂𝗅𝗂𝗍𝗒 𝖺𝗇𝖽 𝗁𝗂𝗀𝗁 𝖺𝗏𝖺𝗂𝗅𝖺𝖻𝗂𝗅𝗂𝗍𝗒.

> [!NOTE]
> 𝖶𝗁𝖾𝗇 𝗒𝗈𝗎 𝖼𝗋𝖾𝖺𝗍𝖾 𝖺 𝖲𝖾𝗋𝗏𝗂𝖼𝖾, 𝗂𝗍 𝗀𝖾𝗍𝗌 𝖺 𝗌𝗍𝖺𝗍𝗂𝖼 𝖨𝖯 𝖺𝖽𝖽𝗋𝖾𝗌𝗌 𝗍𝗁𝖺𝗍 𝖽𝗈𝖾𝗌𝗇'𝗍 𝖼𝗁𝖺𝗇𝗀𝖾. 𝖳𝗁𝖾 𝖲𝖾𝗋𝗏𝗂𝖼𝖾 𝗄𝖾𝖾𝗉𝗌 𝗍𝗋𝖺𝖼𝗄 𝗈𝖿 𝗍𝗁𝖾 𝖯𝗈𝖽𝗌 𝗍𝗁𝖺𝗍 𝗆𝖺𝗍𝖼𝗁 𝗂𝗍𝗌 𝗌𝖾𝗅𝖾𝖼𝗍𝗈𝗋, 𝖾𝗏𝖾𝗇 𝖺𝗌 𝗍𝗁𝖾𝗒 𝖺𝗋𝖾 𝗋𝖾𝗉𝗅𝖺𝖼𝖾𝖽 𝗈𝗋 𝖼𝗁𝖺𝗇𝗀𝖾 𝖨𝖯 𝖺𝖽𝖽𝗋𝖾𝗌𝗌𝖾𝗌. <br>
> 𝖶𝗁𝖾𝗇 𝗍𝗋𝖺𝖿𝖿𝗂𝖼 𝗂𝗌 𝖽𝗂𝗋𝖾𝖼𝗍𝖾𝖽 𝗍𝗈 𝗍𝗁𝖾 𝖲𝖾𝗋𝗏𝗂𝖼𝖾'𝗌 𝗌𝗍𝖺𝖻𝗅𝖾 𝖨𝖯, 𝗍𝗁𝖾 𝖲𝖾𝗋𝗏𝗂𝖼𝖾 𝗍𝗁𝖾𝗇 𝗋𝗈𝗎𝗍𝖾𝗌 𝗍𝗁𝖾 𝗍𝗋𝖺𝖿𝖿𝗂𝖼 𝗍𝗈 𝗈𝗇𝖾 𝗈𝖿 𝗍𝗁𝖾 𝗎𝗇𝖽𝖾𝗋𝗅𝗒𝗂𝗇𝗀 𝖯𝗈d𝗌. <br>
> 𝖳𝗁𝗂𝗌 𝗐𝖺𝗒, 𝖾𝗏𝖾𝗇 𝗍𝗁𝗈𝗎𝗀𝗁 𝖺 𝖯𝗈𝖽 𝗆𝗂𝗀𝗁𝗍 𝗀𝖾𝗍 𝗋𝖾𝗉𝗅𝖺𝖼𝖾𝖽 𝖺𝗇𝖽 𝗋𝖾𝖼𝖾𝗂𝗏𝖾 𝖺 𝗇𝖾𝗐 𝖨𝖯 𝖺𝖽𝖽𝗋𝖾𝗌𝗌, 𝗍𝗁𝖾 𝖲𝖾𝗋𝗏𝗂𝖼𝖾'𝗌 𝖨𝖯 𝖺𝖽𝖽𝗋𝖾𝗌𝗌 𝗋𝖾𝗆𝖺𝗂𝗇𝗌 𝗍𝗁𝖾 𝗌𝖺𝗆𝖾, 𝗉𝗋𝗈𝗏𝗂𝖽𝗂𝗇𝗀 𝖺 𝖼𝗈𝗇𝗌𝗂𝗌𝗍𝖾𝗇𝗍 𝖾𝗇𝖽𝗉𝗈𝗂𝗇𝗍 𝖿𝗈𝗋 𝗈𝗍𝗁𝖾𝗋 𝖼𝗈𝗆𝗉𝗈𝗇𝖾𝗇𝗍𝗌 𝗈𝗋 𝖾𝗑𝗍𝖾𝗋𝗇𝖺𝗅 𝖼𝗅𝗂𝖾𝗇𝗍𝗌 𝗍𝗈 𝖼𝗈𝗇𝗇𝖾𝖼𝗍 𝗍𝗈.

𝖲𝖾𝗋𝗏𝗂𝖼𝖾𝗌 𝖾𝗇𝗌𝗎𝗋𝖾 𝗍𝗁𝖺𝗍 𝗍𝗋𝖺𝖿𝖿𝗂𝖼 𝗋𝖾𝖺𝖼𝗁𝖾𝗌 𝗍𝗁𝖾 𝖼𝗈𝗋𝗋𝖾𝖼𝗍 𝖯𝗈𝖽𝗌 𝗐𝗂𝗍𝗁𝗂𝗇 𝗍𝗁𝖾 𝖪𝗎𝖻𝖾𝗋𝗇𝖾𝗍𝖾𝗌 𝖼𝗅𝗎𝗌𝗍𝖾𝗋, 𝖾𝗏𝖾𝗇 𝖺𝗌 𝖯𝗈𝖽𝗌 𝖺𝗋𝖾 𝖼𝗋𝖾𝖺𝗍𝖾𝖽 𝗈𝗋 𝖽𝖾𝗌𝗍𝗋𝗈𝗒𝖾𝖽. 𝖳𝗁𝗂𝗌 𝗂𝗌 𝖼𝗋𝗂𝗍𝗂𝖼𝖺𝗅 𝖿𝗈𝗋 𝗍𝗁𝖾 𝗂𝗇𝗍𝖾𝗋𝗇𝖺𝗅 𝗐𝗈𝗋𝗄𝗂𝗇𝗀𝗌 𝗈𝖿 𝗍𝗁𝖾 𝖼𝗅𝗎𝗌𝗍𝖾𝗋. 𝖧𝗈𝗐𝖾𝗏𝖾𝗋, 𝗐𝖾 𝗈𝖿𝗍𝖾𝗇 𝗇𝖾𝖾𝖽 𝖺 𝗐𝖺𝗒 𝗍𝗈 𝖼𝗈𝗇𝗇𝖾𝖼𝗍 𝗍𝗁𝖾 𝗈𝗎𝗍𝗌𝗂𝖽𝖾 𝗐𝗈𝗋𝗅𝖽 𝗍𝗈 𝗈𝗎𝗋 𝗂𝗇𝗍𝖾𝗋𝗇𝖺𝗅 𝗌𝖾𝗋𝗏𝗂𝖼𝖾𝗌 𝗂𝗇 𝖺 𝖼𝗈𝗇𝗍𝗋𝗈𝗅𝗅𝖾𝖽 𝖺𝗇𝖽 𝖾𝖿𝖿𝗂𝖼𝗂𝖾𝗇𝗍 𝗆𝖺𝗇𝗇𝖾𝗋. <br>
𝖳𝗁𝗂𝗌 𝗂𝗌 𝗐𝗁𝖾𝗋𝖾 𝖨𝗇𝗀𝗋𝖾𝗌𝗌 𝖾𝗇𝗍𝖾𝗋𝗌 𝗍𝗁𝖾 𝗉𝗂𝖼𝗍𝗎𝗋𝖾.

#### 𝖨𝗇𝗀𝗋𝖾𝗌𝗌
𝖠𝖿𝗍𝖾𝗋 𝖾𝗌𝗍𝖺𝖻𝗅𝗂𝗌𝗁𝗂𝗇𝗀 𝗌𝗍𝖺𝖻𝗅𝖾 𝖼𝗈𝗆𝗆𝗎𝗇𝗂𝖼𝖺𝗍𝗂𝗈𝗇 𝗐𝗂𝗍𝗁𝗂𝗇 𝗍𝗁𝖾 𝖼𝗅𝗎𝗌𝗍𝖾𝗋 𝗎𝗌𝗂𝗇𝗀 𝖲𝖾𝗋𝗏𝗂𝖼𝖾𝗌, 𝗐𝖾 𝗈𝖿𝗍𝖾𝗇 𝗋𝖾𝗊𝗎𝗂𝗋𝖾 𝖾𝗑𝗍𝖾𝗋𝗇𝖺𝗅 𝗎𝗌𝖾𝗋𝗌 𝗈𝗋 𝗌𝗒𝗌𝗍𝖾𝗆𝗌 𝗍𝗈 𝖺𝖼𝖼𝖾𝗌𝗌 𝗍𝗁𝖾𝗌𝖾 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇𝗌. 𝖨𝗇𝗌𝗍𝖾𝖺𝖽 𝗈𝖿 𝖾𝗑𝗉𝗈𝗌𝗂𝗇𝗀 𝖾𝖺𝖼𝗁 𝗌𝖾𝗋𝗏𝗂𝖼𝖾 𝖽𝗂𝗋𝖾𝖼𝗍𝗅𝗒 𝗍𝗈 𝗍𝗁𝖾 𝗈𝗎𝗍𝗌𝗂𝖽𝖾 (𝗐𝗁𝗂𝖼𝗁 𝖼𝖺𝗇 𝖻𝖾 𝖼𝗈𝗆𝗉𝗅𝖾𝗑 𝖺𝗇𝖽 𝗂𝗇𝗌𝖾𝖼𝗎𝗋𝖾), 𝗐𝖾 𝗎𝗌𝖾 𝖨𝗇𝗀𝗋𝖾𝗌𝗌.

𝖪𝖾𝗒 𝖥𝗎𝗇𝖼𝗍𝗂𝗈𝗇𝗌 𝗈𝖿 𝖨𝗇𝗀𝗋𝖾𝗌𝗌:
- 𝖤𝗑𝗍𝖾𝗋𝗇𝖺𝗅 𝖠𝖼𝖼𝖾𝗌𝗌: 𝖨𝗇𝗀𝗋𝖾𝗌𝗌 𝖺𝖼𝗍𝗌 𝖺𝗌 𝖺 𝗌𝗆𝖺𝗋𝗍 𝗋𝗈𝗎𝗍𝖾𝗋 𝗈𝗋 𝖾𝗇𝗍𝗋𝗒 𝗉𝗈𝗂𝗇𝗍 𝗍𝗈 𝗍𝗁𝖾 𝖼𝗅𝗎𝗌𝗍𝖾𝗋, 𝖽𝗂𝗋𝖾𝖼𝗍𝗂𝗇𝗀 𝖾𝗑𝗍𝖾𝗋𝗇𝖺𝗅 𝖧𝖳𝖳𝖯(𝖲) 𝗍𝗋𝖺𝖿𝖿𝗂𝖼 𝗍𝗈 𝗍𝗁𝖾 𝖺𝗉𝗉𝗋𝗈𝗉𝗋𝗂𝖺𝗍𝖾 𝗂𝗇𝗍𝖾𝗋𝗇𝖺𝗅 𝖲𝖾𝗋𝗏𝗂𝖼𝖾𝗌 𝖻𝖺𝗌𝖾𝖽 𝗈𝗇 𝗉𝗋𝖾𝖽𝖾𝖿𝗂𝗇𝖾𝖽 𝗋𝗎𝗅𝖾𝗌.
- 𝖴𝗇𝗂𝖿𝗂𝖾𝖽 𝖤𝗇𝗍𝗋𝗒 𝖯𝗈𝗂𝗇𝗍: 𝖨𝗍 𝗉𝗋𝗈𝗏𝗂𝖽𝖾𝗌 𝖺 𝗌𝗂𝗇𝗀𝗅𝖾 𝖾𝗇𝗍𝗋𝗒 𝗉𝗈𝗂𝗇𝗍 𝗍𝗈 𝗆𝖺𝗇𝖺𝗀𝖾 𝖺𝖼𝖼𝖾𝗌𝗌 𝗍𝗈 𝗆𝗎𝗅𝗍𝗂𝗉𝗅𝖾 𝗌𝖾𝗋𝗏𝗂𝖼𝖾𝗌 𝗂𝗇 𝗍𝗁𝖾 𝖼𝗅𝗎𝗌𝗍𝖾𝗋, 𝗋𝖾𝖽𝗎𝖼𝗂𝗇𝗀 𝗍𝗁𝖾 𝗇𝖾𝖾𝖽 𝖿𝗈𝗋 𝗆𝗎𝗅𝗍𝗂𝗉𝗅𝖾 𝗉𝗎𝖻𝗅𝗂𝖼 𝖨𝖯 𝖺𝖽𝖽𝗋𝖾𝗌𝗌𝖾𝗌.
- 𝖲𝖾𝖼𝗎𝗋𝗂𝗍𝗒 𝖺𝗇𝖽 𝖢𝗈𝗆𝗉𝗅𝗂𝖺𝗇𝖼𝖾: 𝖡𝗒 𝗁𝖺𝗇𝖽𝗅𝗂𝗇𝗀 𝖲𝖲𝖫/𝖳𝖫𝖲 𝗍𝖾𝗋𝗆𝗂𝗇𝖺𝗍𝗂𝗈𝗇 𝖺𝗍 𝗍𝗁𝖾 𝖨𝗇𝗀𝗋𝖾𝗌𝗌 𝗅𝖾𝗏𝖾𝗅, 𝗐𝖾 𝖼𝖾𝗇𝗍𝗋𝖺𝗅𝗂𝗓𝖾 𝗍𝗁𝖾 𝗌𝖾𝖼𝗎𝗋𝗂𝗍𝗒 𝖺𝗌𝗉𝖾𝖼𝗍, 𝗆𝖺𝗄𝗂𝗇𝗀 𝗂𝗍 𝖾𝖺𝗌𝗂𝖾𝗋 𝗍𝗈 𝗆𝖺𝗇𝖺𝗀𝖾 𝖼𝖾𝗋𝗍𝗂𝖿𝗂𝖼𝖺𝗍𝖾𝗌 𝖺𝗇𝖽 𝖼𝗈𝗆𝗉𝗅𝗂𝖺𝗇𝖼𝖾.
- 𝖯𝖺𝗍𝗁-𝖡𝖺𝗌𝖾𝖽 𝖱𝗈𝗎𝗍𝗂𝗇𝗀: 𝖨𝗇𝗀𝗋𝖾𝗌𝗌 𝖼𝗈𝗇𝗍𝗋𝗈𝗅𝗅𝖾𝗋𝗌 𝖼𝖺𝗇 𝗋𝗈𝗎𝗍𝖾 𝗍𝗋𝖺𝖿𝖿𝗂𝖼 𝗍𝗈 𝖽𝗂𝖿𝖿𝖾𝗋𝖾𝗇𝗍 𝗌𝖾𝗋𝗏𝗂𝖼𝖾𝗌 𝖻𝖺𝗌𝖾𝖽 𝗈𝗇 𝗍𝗁𝖾 𝖴𝖱𝖫 𝗉𝖺𝗍𝗁. 𝖥𝗈𝗋 𝖾𝗑𝖺𝗆𝗉𝗅𝖾, 𝗍𝗋𝖺𝖿𝖿𝗂𝖼 𝗍𝗈 𝖾𝗑𝖺𝗆𝗉𝗅𝖾.𝖼𝗈𝗆/𝗏𝗂𝖽𝖾𝗈 𝗀𝗈𝖾𝗌 𝗍𝗈 𝗈𝗇𝖾 𝗌𝖾𝗋𝗏𝗂𝖼𝖾, 𝗐𝗁𝗂𝗅𝖾 𝖾𝗑𝖺𝗆𝗉𝗅𝖾.𝖼𝗈𝗆/𝖺𝗎𝖽𝗂𝗈 𝗀𝗈𝖾𝗌 𝗍𝗈 𝖺𝗇𝗈𝗍𝗁𝖾𝗋.












