# Framer

## Description
- Framer is a wab app which calls an API to retrieve a video. However, the API that should be containing the video is actually containing images where each image is a frame of the video! This is intentional; Framer stitches the frames together and mimics a 30fps video.
---

## Prerequisits
- Docker v19.03.13 or higher
- Docker-compose v1.27.4 or higher
- Node.js v16.15.1 or higher
- npm v6.14.9 or higher
- yarn v1.22.5 or higher

## How to Run

### Option 1: Deploying Client and Server into a docker container
1. Deploy Client & Server (Using Docker) ➡ `$ docker-compose up`
- or Server ONLY ➡ `$ cd Framer/server; yarn run dev`
- or Client ONLY ➡ `$ cd Framer/client; yarn start`compose up

### Option 2: Deploying Client + _API_ into a docker container (<ins>_`EC2 Linux Instance`_<ins>)
1. AWS Management Console
2. Create _EC2 Linux Instance_
3. Install the following within _EC2 Linux Instance_:
  - `Node.js` + `npm` + `yarn`
  - <a href="https://gist.github.com/npearce/6f3c7826c7499587f00957fee62f8ee9" target="_top"><b>`Docker + Docker-Compose`</b></a>
  - clone project repository

5. Deploy Client & Server (Using Docker) ➡ `$ docker-compose up`
- or Server ONLY ➡ `$ cd Framer/server; yarn run dev`
- or Client ONLY ➡ `$ cd Framer/client; yarn start`
