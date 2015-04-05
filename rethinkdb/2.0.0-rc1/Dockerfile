FROM    erealm/centos6

RUN     rpm -ivh http://download.rethinkdb.com/dev/2.0.0-0RC1/rethinkdb-2.0.0_0RC1.x86_64.rpm

# Define default command.
EXPOSE 8080
EXPOSE 28015
EXPOSE 29015

WORKDIR /data

VOLUME /data

CMD ["/usr/bin/rethinkdb", "--bind", "all", "-d", "/data"]
