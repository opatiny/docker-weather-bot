FROM nodered/node-red:1.0.6

# copy node-red project files into place
COPY weather-bot/flow.json /data/flows.json
COPY weather-bot/flow_cred.json /data/flows_cred.json
COPY weather-bot/package.json /data/package.json
COPY settings.js /data/settings.js

RUN npm i node-red-contrib-telegrambot@8.1.0
