# focalboard
personal docker image build for focalboard


## Usage

```
docker run -it -p 8000:8000 melashri/focalboard
```

### Using docker-compose

The `docker-compose.yml` can be 

```
services:
  focalboard:
    image: nicoulaj/focalboard
    volumes:
    - ./config.json:/opt/focalboard/config.json
    - /var/lib/focalboard:/var/lib/focalboard
```

run the docker-compose

```
docker-compose up -d
``` 


with `config.json`
```
{
    ["serverRoot": "http://focalboard.tld",]
    "port": 8000,
    "dbtype": "sqlite3",
    "dbconfig": "/var/lib/focalboard/focalboard.db",
    "postgres_dbconfig": "dbname=focalboard sslmode=disable",
    "useSSL": false,
    "webpath": "./pack",
    "filespath": "/var/lib/focalboard/files",
    "telemetry": false,
    "session_expire_time": 2592000,
    "session_refresh_time": 18000,
    "localOnly": false,
    "enableLocalMode": true,
    "localModeSocketLocation": "/var/tmp/focalboard_local.socket"
}
```
