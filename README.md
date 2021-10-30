# focalboard
personal docker image build for focalboard


## Usage

```
docker build --build-arg focalboard_version=0.6.5 -t focalboard .
docker run -it -p 8000:8000 focalboard
```

### Using docker-compose

```
docker-compose up -d
``` 

