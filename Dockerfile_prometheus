FROM centos

RUN yum install wget -y

RUN wget https://github.com/prometheus/prometheus/releases/download/v2.19.0/prometheus-2.19.0.linux-amd64.tar.gz

RUN tar -xzf prometheus-2.19.0.linux-amd64.tar.gz

RUN mkdir /prometheus

CMD ./prometheus-2.19.0.linux-amd64/prometheus --config.file=/prometheus-2.19.0.linux-amd64/prometheus.yml --storage.tsdb.path=/prometheus && tail -f /dev/null
