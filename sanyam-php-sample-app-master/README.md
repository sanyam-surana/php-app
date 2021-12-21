# Sanyam PHP Sample app

Tech stack:

- PHP
- Docker
- Kubernetes

## Steps to deploy the app on kubernetes

- Clone the repo

```sh
git clone https://github.com/sanyam-surana/php-app/tree/main/sanyam-php-sample-app-master
cd sanyam-php-sample-app
```

- Build the image and push it to your docker registry

```sh
docker build -t <docker_repo/your_image_name>:<tag> .
docker image push <docker_repo/your_image_name>:<tag>
```

- Deploy the components in k8s/ folder to your kubernetes cluster

```sh
kubectl apply -f ./k8s/
```
