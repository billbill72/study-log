### Build docker image with self defined plugins
``` shell
docker build --pull --rm -e JENKINS_VERSION=2.515-jdk21 -f 'jenkins\2.515-jdk21\dockerfile' -t 'jenkins/jenkins:2.515-jdk21-edition' 'jenkins\2.515-jdk21'
```
