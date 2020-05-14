# docker-weather-bot

Dockerization of [weather-bot project](https://github.com/opatiny/weather-bot).

This project uses sub-modules!

## How to use it
### Clone the project
```bash
git clone --recurse-submodules https://github.com/opatiny/docker-weather-bot
```

### Add your environment variables

Copy the `docker-compose.yml.example` file to `docker-compose.yml` and replace the two environment variables with your credentials:
```yml
    environment:
      BOT_TOKEN: <your token here>
      OWM_ID: <your openweathermap appid here>
```

### Start the bot

Run the following command:

```bash
docker-compose up -d --build
```

Or use the script if you have node.js:

```bash
npm start
```

### Stop the bot

Run the following command:

```bash
docker-compose down
```

Or use the script if you have node.js:

```bash
npm run stop
```

## For development only: Updating the submodules

```bash
git submodule update --recursive --remote
```

Or use the script:
```bash
npm run update
```
