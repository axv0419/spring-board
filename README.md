# spring-board
Sample repo for GCloud install


### Build / Tag / Push image

To push the image to gcr.io


```bash

# docker login to gcr.io
gcloud auth configure-docker
gcloud auth login

#build the image
GCP_PROJECT_NAME=xyz-dev-mx
docker build -t d3x-spring-board
docker tag d3x-spring-board gcr.io/${GCP_PROJECT_NAME}/d3x-spring-board
docker push gcr.io/${GCP_PROJECT_NAME}/d3x-spring-board

```
