# elkctl
A simple "elkctl" (like apachectl) script for the Elasticsearch, Logstash and Kibana stack.

## My current versions
I'm currently using this with:
* Elasticsearch 2.1.0
* Logstash 2.0.0
* Kibana 4.3.0

## Pre-requisites
Elasticsearch, Logstash and Kibana are installed and have init scripts.
i.e. you can start them with "sudo service start kibana"

If you haven't configured your ELK stack yet then this won't work.
I used [this digital ocean guide](https://www.digitalocean.com/community/tutorials/how-to-install-elasticsearch-logstash-and-kibana-elk-stack-on-ubuntu-14-04) to build a single instance stack and get started.

## Install
This is just a shell script so you can download it and put it anywhere in your PATH and give it executable permissions to install.
Example install:
1. `cd ~`
2. `mkdir src`
3. `cd src`
4. `wget https://github.com/BasiliusCarver/elkctl/archive/master.tar.gz`
5. `tar -xvf master.tar.gz`
6. `cd elkctl-master/`
7. `sudo cp elkctl.sh /usr/bin/`
8. `sudo chmod a+x /usr/bin/elkctl.sh`

First run:
1. `sudo elkctl status`
