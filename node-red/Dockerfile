FROM nodered/node-red:1.0.6

# copy node-red project files into place
COPY weather-bot /data
COPY settings.js /data/settings.js

RUN npm i node-red-contrib-telegrambot@8.1.0
