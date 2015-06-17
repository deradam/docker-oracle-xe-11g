docker-oracle-xe-11g
============================

Oracle Express Edition 11g Release 2 on Ubuntu 14.04.1 LTS

This **Dockerfile** is a based on [https://registry.hub.docker.com/u/sath89/oracle-xe-11g/]
It is actually a role back to the changes before June 2015 for local compatibility reasons.

### Installation

    docker pull deradam/oracle-xe-11g

Run with 8080 and 1521 ports opened:

    docker run -d -p 8080:8080 -p 1521:1521 deradam/oracle-xe-11g

Connect database with following setting:

    hostname: localhost
    port: 1521
    sid: xe
    username: system
    password: oracle

Password for SYS & SYSTEM:

    oracle

Connect to Oracle Application Express web management console with following settings:

    http://localhost:8080/apex
    workspace: INTERNAL
    user: ADMIN
    password: oracle