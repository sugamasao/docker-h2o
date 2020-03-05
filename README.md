# Docker image for h2o with HTTPS

- create Self certificate.
- revese proxy to internal:3000

## How to use

docker image build.

```sh
% git clone
% docker build -t h2o-https:1 .
% docker run -it -p 9090:9090 h2o-https:1
```

h2o waiting `https://localhost:9090`.

next. wake up App Server

```sh
% ./bin/rails s -p 3000
```

acess to `https://localhost:9090` !

