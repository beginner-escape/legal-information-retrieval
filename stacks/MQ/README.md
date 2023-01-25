## Message Queue

### Only one container
---
1. Download confluent-kafka

```sh
$ sh download
```

2. Build image
```sh
$ docker build -t {container_name}:{version} .
```

3. (Optional) Run the container
```sh
$ docker run -{flags} {container_name}:{version}
```
