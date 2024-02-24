# Basic rtmp nginx server made in docker

Intended for vrchat video players but can be used for anything

Inspired by https://github.com/mekanoe/VRC_HLS

## Setup instuctions
1. Install docker if you dont have it already
2. Edit the docker-compose.yml and maybe line 12 in nginx.conf to your needs, make sure you open the port on your router. In this case ``34200``
3. Run the ``start.bat``, ``start.sh`` or just ``docker compose up``
4. Set your obs to stream to ``rtmp://127.0.0.1/live``, stream key can be anything
5. View your work, you can try it in vlc or vrchat and enter ``http://PUBLIC-IP:34200/hls/THE-STREAM-KEY-YOU-CHOSE-HERE.m3u8``
6. Enjoy... theres probably gonna be noticable latency and i cant help with that sorry! Just try stuff maybe you can get it down.
