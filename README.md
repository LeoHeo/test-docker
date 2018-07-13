## Docker build

```
$ docker build -t test-docker/node .
```

## Docker run
- NODE_ENV 바꾸고 싶은걸로

```
$ docker run -p 4999:3000 -e NODE_ENV=test -d test-docker/node
```

## Test

```
$ curl localhost:4999
<!DOCTYPE html><html><head><title>test</title><link rel="stylesheet" href="/stylesheets/style.css"></head><body><h1>test</h1><p>Welcome to test</p></body></html>%
```
