# focalboard
personal docker image build for focalboard


## Usage

```
docker build --build-arg focalboard_version=0.9.4 -t focalboard .
docker run -it -p 8000:8000 focalboard
```

### Using docker-compose

```
docker-compose up -d
``` 

