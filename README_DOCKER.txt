1. Clone this repository to local
2. Edit gdanmaku/settings.py
3. Build it! (docker build -t gdanmaku-server .)
4. Fire up an redis container (docker run --name gdanmaku-redis -d redis)
5. Fire up the app (docker run -id --name gdanmaku-server -p 50001:5000 --restart=always --link gdanmaku-redis:redis gdanmaku-server)
6. Now your app up at 0.0.0.0:50001 Enjoy :)
