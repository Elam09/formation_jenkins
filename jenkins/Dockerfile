FROM jenkins/jenkins
LABEL maintainer="didiertahobeu93@gmail.com"
USER root
RUN mkdir /var/log/jenkins
RUN mkdir /var/cache/jenkins

RUN chown -R jenkins:jenkins /var/log/jenkins
RUN chown -R jenkins:jenkins /var/cache/jenkins
RUN chmod -R 777 /opt
RUN chmod -R 777 /var
RUN chmod -R 777 /etc

USER jenkins




ENV JAVA_OPTS="-Xmx8192m"
ENV JENKINS_OPTS="--handlerCountMax=300 --logfile=/var/log/jenkins/jenkins.log --webroot=/var/cache/jenkins/war"
