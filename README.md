# Commands

```bash
docker login

docker info -f '{{.DriverStatus}}'

docker buildx ls
docker buildx create --name mybuilder
docker buildx use mybuilder
docker buildx ls

docker buildx inspect --bootstrap

docker buildx build -t newimage . --platform linux/amd64,linux/arm64 -o type=oci,dest=- > newimage.tar

docker load < newimage.tar

# docker tag
# docker push
```