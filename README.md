# **kudu**
___

### Description
___

This image runs [*Apache Kudu*](https://kudu.apache.org/) included in the Cloudera CDH distribution.

You can pull it with:

    docker pull comchangs/kudu


You can also find other images based on different Apache Kudu releases, using a different tag in the following form:

    docker pull comchangs/kudu:[kudu-release]-[cdh-release]


Stop with Docker Compose:

    docker-compose -p comchangs up


**IMPORTANT**: You need the **ntpd** daemon running on the host. To install it:

    apt-get install ntp (Debian, Ubuntu)
    yum install ntp     (RedHat, Centos)
    
    sudo service ntp start

Once started you'll be able to access to the following UIs:

| **Kudu Web UIs**           |**URL**                    |
|:----------------------------|:--------------------------|
| *Kudu Master*               | http://localhost:8051     |
| *Kudu Tablet Server*        | http://localhost:8050     |
