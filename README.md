# jenkins-pipeline

docker pull jenkins/jenkins
docker run   -u root --rm -d --network host --dns <dns host> --env http_proxy="http://<proxy>:<port>" --env https_proxy="https://<proxy>:<port>" --env no_proxy="127.0.0.1,localhost" -v jenkins-data:/var/jenkins_home -v /var/run/docker.sock:/var/run/docker.sock jenkins/jenkins:latest

docker exec -it a165f4e59c39  script -q -c "/bin/bash" /dev/null
