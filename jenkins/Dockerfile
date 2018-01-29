FROM jenkins/jenkins:lts
USER root
RUN apt-get update \
      && apt-get install -y git maven sudo libltdl7 \
      && rm -rf /var/lib/apt/lists/*
RUN echo "jenkins ALL=NOPASSWD: ALL" >> /etc/sudoers
USER jenkins
ADD jdk8.tar.gz /usr/local/
ADD jenkins.sh /etc/profile.d
