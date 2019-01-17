FROM openjdk:11-jdk

RUN apt-get update && apt-get -y install libapache2-mod-svn git-svn vim

WORKDIR /svn-migration

RUN wget https://bitbucket.org/atlassian/svn-migration-scripts/downloads/svn-migration-scripts.jar && \
    java -jar svn-migration-scripts.jar verify