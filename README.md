
* [Docker](#docker)
  * [Run](#run)
  * [Network](#docker-networking)

# Docker
### 𝖶𝗁𝖺𝗍 𝗂𝗌 𝖣𝗈𝖼𝗄𝖾𝗋?
𝖣𝗈𝖼𝗄𝖾𝗋 𝗂𝗌 𝖺 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗂𝗓𝖺𝗍𝗂𝗈𝗇 𝗉𝗅𝖺𝗍𝖿𝗈𝗋𝗆 𝗍𝗁𝖺𝗍 𝖺𝗅𝗅𝗈𝗐𝗌 𝗍𝗈 𝗉𝗎𝗍 𝖺𝗉𝗉𝗅𝗂𝖼𝖺𝗍𝗂𝗈𝗇𝗌 𝖺𝗇𝖽 𝗍𝗁𝖾𝗂𝗋 𝖽𝖾𝗉𝖾𝗇𝖽𝖾𝗇𝖼𝗂𝖾𝗌 𝗂𝗇𝗍𝗈 𝗂𝗌𝗈𝗅𝖺𝗍𝖾𝖽, 𝗅𝗂𝗀𝗁𝗍𝗐𝖾𝗂𝗀𝗁𝗍 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌.
<𝖻𝗋>
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


- `𝖡𝗋𝗂𝖽𝗀𝖾`: 𝖳𝗁𝖾 𝖡𝗋𝗂𝖽𝗀𝖾 𝗇𝖾𝗍𝗐𝗈𝗋𝗄 𝖺𝗌𝗌𝗂𝗀𝗇𝗌 𝖨𝖯𝗌 𝗂𝗇 𝗍𝗁𝖾 𝗋𝖺𝗇𝗀𝖾 𝗈𝖿 𝟣𝟩𝟤.𝟣𝟩.𝗑.𝗑 𝗍𝗈 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 𝗐𝗂𝗍𝗁𝗂𝗇 𝗂𝗍.<𝖻𝗋>
𝖳𝗈 𝖺𝖼𝖼𝖾𝗌𝗌 𝗍𝗁𝖾𝗌𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 𝖿𝗋𝗈𝗆 𝗈𝗎𝗍𝗌𝗂𝖽𝖾 𝗒𝗈𝗎 𝗇𝖾𝖾𝖽 𝗍𝗈 𝗆𝖺𝗉 𝗍𝗁𝖾 𝗉𝗈𝗋𝗍𝗌 𝗈𝖿 𝗍𝗁𝖾𝗌𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌 𝗍𝗈 𝗍𝗁𝖾 𝗉𝗈𝗋𝗍𝗌 𝗈𝗇 𝗍𝗁𝖾 𝗁𝗈𝗌𝗍.
- `𝖧𝗈𝗌𝗍`: 𝖲𝖾𝗅𝖾𝖼𝗍𝗂𝗇𝗀 𝗍𝗁𝖾 𝖧𝗈𝗌𝗍 𝗇𝖾𝗍𝗐𝗈𝗋𝗄 𝗐𝗂𝗅𝗅 𝗋𝖾𝗆𝗈𝗏𝖾 𝖺𝗇𝗒 𝗇𝖾𝗍𝗐𝗈𝗋𝗄 𝗂𝗌𝗈𝗅𝖺𝗍𝗂𝗈𝗇 𝖻𝖾𝗍𝗐𝖾𝖾𝗇 𝗍𝗁𝖾 𝖽𝗈𝖼𝗄𝖾𝗋 𝗁𝗈𝗌𝗍 𝖺𝗇𝖽 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋𝗌.<𝖻𝗋>
𝖥𝗈𝗋 𝗂𝗇𝗌𝗍𝖺𝗇𝖼𝖾, 𝗂𝖿 𝗒𝗈𝗎 𝗋𝗎𝗇 𝖺 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗈𝗇 𝗉𝗈𝗋𝗍 𝟧𝟢𝟢𝟢, 𝗂𝗍 𝗐𝗂𝗅𝗅 𝖻𝖾 𝖺𝖼𝖼𝖾𝗌𝗌𝗂𝖻𝗅𝖾 𝗈𝗇 𝗍𝗁𝖾 𝗌𝖺𝗆𝖾 𝗉𝗈𝗋𝗍 𝗈𝗇 𝗍𝗁𝖾 𝖽𝗈𝖼𝗄𝖾𝗋 𝗁𝗈𝗌𝗍 𝗐𝗂𝗍𝗁𝗈𝗎𝗍 𝖺𝗇𝗒 𝖾𝗑𝗉𝗅𝗂𝖼𝗂𝗍 𝗉𝗈𝗋𝗍 𝗆𝖺𝗉𝗉𝗂𝗇𝗀. 𝖳𝗁𝖾 𝗈𝗇𝗅𝗒 𝖽𝗈𝗐𝗇𝗌𝗂𝖽𝖾 𝗈𝖿 𝗍𝗁𝗂𝗌 𝖺𝗉𝗉𝗋𝗈𝖺𝖼𝗁 𝗂𝗌 𝗍𝗁𝖺𝗍 𝗒𝗈𝗎 𝖼𝖺𝗇 𝗇𝗈𝗍 𝗎𝗌𝖾 𝗍𝗁𝖾 𝗌𝖺𝗆𝖾 𝗉𝗈𝗋𝗍 𝗍𝗐𝗂𝖼𝖾 𝖿𝗈𝗋 𝖺𝗇𝗒 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋.
- `𝖭𝗈𝗇𝖾`: 𝖳𝗁𝖾 𝖭𝗈𝗇𝖾 𝗇𝖾𝗍𝗐𝗈𝗋𝗄 𝗄𝖾𝖾𝗉𝗌 𝗍𝗁𝖾 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋 𝗂𝗇 𝖼𝗈𝗆𝗉𝗅𝖾𝗍𝖾 𝗂𝗌𝗈𝗅𝖺𝗍𝗂𝗈𝗇, 𝗂.𝖾. 𝗍𝗁𝖾𝗒 𝖺𝗋𝖾 𝗇𝗈𝗍 𝖼𝗈𝗇𝗇𝖾𝖼𝗍𝖾𝖽 𝗍𝗈 𝖺𝗇𝗒 𝗇𝖾𝗍𝗐𝗈𝗋𝗄 𝗈𝗋 𝖼𝗈𝗇𝗍𝖺𝗂𝗇𝖾𝗋.

By default all containers are in `𝖡𝗋𝗂𝖽𝗀𝖾` network.
If we want to run two containers in a separate network,<br>
we can define a custom(user-defined) network for this purpose by using the following command and assigning this network when running the containers.
 - `docker network create <options> <network_name>`

For example, if we want to create a separate network for a webApp with database:

 - Define a network (specifying driver and subnet are optional)
   ```console
   docker network create \
      --driver bridge \
      --subnet 182.18.0.0/16 \
      user-net
   ```
 - Create a Postgres instance
   - Pull latest Postgres image
     ```console
     docker pull postgres
     ```
   - Build postgres container
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
 - Create a webApp instance
   - Build webApp image
     ```console
     docker build --name webApp-img .
     ```
   - Build webApp container
     ```console
     docker run \
        --name webApp-container \
        --network user-net \
        -p 5000:5000 \
        --detach \
        webApp-img
     ```
   
