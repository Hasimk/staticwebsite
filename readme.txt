docker steps--

1- docker build -t img-static-site-example .

2- docker run -it -d -p 9090:80 img-static-site-example

3- In case the port 80 is occupied by the host machine or any other docker container. You can change the host machine port to something else.
also you can push that image artifact registry with help of below command

4- docker run -it -d -p 8080:80 img-static-site-example

5- Once the container is up and running. All the on port 8080 of host machine will be redirected to container’s port 80.

Access you docker host using IP address (or hostname/domain name) on port 8080 to view application.


======================================================================================================================

how to push image in artifact registry 
1- gcloud auth login
2- gcloud auth configure-docker \
    asia-south1-docker.pkg.dev

3- docker images

4- docker push asia-south1-docker.pkg.dev/projectname/repositoryname/te-api-gateway:v1
