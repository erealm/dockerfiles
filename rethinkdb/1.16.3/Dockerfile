FROM    erealm/centos6

RUN     rpm -ivh http://download.rethinkdb.com/centos/6/x86_64/rethinkdb-1.16.3.x86_64.rpm

# Define default command.
EXPOSE 8080
EXPOSE 28015
EXPOSE 29015

WORKDIR /data

VOLUME /data

CMD ["/usr/bin/rethinkdb", "--bind", "all", "-d", "/data"]
