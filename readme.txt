docker steps

docker build -t img-static-site-example .

docker run -it -d -p 80:80 img-static-site-example

also you can push that image artifact registry with help of below command
===============================================================================
1- gcloud auth login
2- gcloud auth configure-docker \
    asia-south1-docker.pkg.dev

3- docker images

4- docker push asia-south1-docker.pkg.dev/projectname/repositoryname/te-api-gateway:v1
