FROM centos
VOLUME /var/lib/mysql
RUN yum -y install mysql-server
RUN yum -y install java-1.7.0-openjdk.x86_64
RUN wget -O /etc/yum.repos.d/sonar.repo http://downloads.sourceforge.net/project/sonar-pkg/rpm/sonar.repo
RUN yum -y install sonar
EXPOSE 9000
CMD ["/opt/sonar/bin/linux-x86-64/sonar.sh", "console"]
