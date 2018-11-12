# Labs-Gate-Deploy
Deploy University laboratory network management system

# Deploy with Docker
first clone deploy git on your server

you need `curl git pip docker docker-compose`

## install dependencies
in ubuntu

`sudo apt-get update`

`sudo apt-get -y install apt-transport-https ca-certificates curl software-properties-common git`

in centos

`sudo yum install -y yum-utils device-mapper-persistent-data lvm2 curl git`

## install docker 

in ubuntu


`curl -fsSL http://mirrors.aliyun.com/docker-ce/linux/ubuntu/gpg | sudo apt-key add -`

`sudo add-apt-repository "deb [arch=amd64] http://mirrors.aliyun.com/docker-ce/linux/ubuntu $(lsb_release -cs) stable"`

`sudo apt-get -y update`

`sudo apt-get -y install docker-ce`

in centos

`sudo yum-config-manager --add-repo http://mirrors.aliyun.com/docker-ce/linux/centos/docker-ce.repo`

`sudo yum makecache fast`

`sudo yum -y install docker-ce`

`sudo service docker start`

## install pip

`curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py`

`python get-pip.py`

## install docker compose

`pip install docker-compose`

## Deploy Project

`git clone https://github.com/shiyunjin/Labs-Gate-Deploy.git`

`cd Labs-Gate-Deploy`

`docker-compose up -d`
