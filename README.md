# Kunagi Docker
Docker image contains Kunagi - application for managing Scrum project.
See more about Kunagi: http://kunagi.org/

Actual version of Kunagi is 0.26.2.
It is deployed on Apache Tomcat 7.0.70 with Java Runtime 7.

## Running application
```sh
docker run -d -p 8080:8080 --name kunagi -v /home/YOUR_USER/kunagi-data:/usr/local/tomcat/webapps/kunagi-data speedlog/kunagi-docker
```
It exposes port 8080, so application will be avaible on http://localhost:8080/kunagi. Kunagi data will be persist in host folder "/home/YOUR_USER/kunagi-data".

## Configuration
You can run container with another version of Kunagi. There are two environment options:
* KUNAGI_VERSION - version of Kunagi application
* KUNAGI_SHA1 - sha1 of war file
