FROM            redhat/ubi9
COPY            mongo.repo /etc/yum.repos.d
RUN             dnf install mongodb-mongosh git -y
RUN             mkdir /tmp
WORKDIR         /tmp
COPY            *.js run.sh /tmp/
ENTRYPOINT      ["bash", "run.sh"]

