# docker-artifactory-jcr
dockerized artifactory-jcr install

# Installation of artifactory with docker

```
docker pull docker.bintray.io/jfrog/artifactory-jcr:latest

```
# Creating folder for data persistance

```
mkdir -p /var/opt/jfrog/artifactory
chown -R 1030:1030 /var/opt/jfrog

```

# Running artifactory image

```
docker run --name artifactory -d -p 8808:8081 -v /var/opt/jfrog/artifactory:/var/opt/jfrog/artifactory docker.bintray.io/jfrog/artifactory-jcr:latest

```

# URL
http://server_name:8808
