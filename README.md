# docker-run-rs

Run run-rs in a docker container. run-rs is a zero-config MongoDB runner. Starts a replica set with no non-node dependencies, not even MongoDB.

## Use as a service in GitHub Actions
```yaml
jobs:
  build:
  
    ...

    services:
      mongodb:
        image: docker.pkg.github.com/luca-rand/docker-run-rs/run
        ports:
          - 27017/tcp
          - 27018/tcp
          - 27019/tcp
```
