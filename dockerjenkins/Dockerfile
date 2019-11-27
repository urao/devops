FROM jenkins/jenkins:2.112
LABEL maintainer="urao@juniper.net"

USER root
RUN mkdir /var/log/jenkins
RUN chown -R jenkins:jenkins /var/log/jenkins
USER jenkins


ENV JAVA_OPTS="-Xmx8192m"
ENV JENKINS_OPTS="--handlerCountMax=10 --logfile=/var/log/jenkins/jenkins.log"
