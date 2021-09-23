# Cluster Docker: Apache Ranger


## Background

Docker cluster with Apache Ranger and a minimal Hadoop ecosystem to perform some basic experiments. This branch is forked from [kadensungbincho/apache-ranger-docker-poc](https://github.com/kadensungbincho/apache-ranger-docker-poc) and I'm only reorganized and updated the docker-compose file, trying to make the start process in one step. This cluster provides:

- Apache Ranger (with ElasticSearch to store and retrieve audit logs);
- HDFS;
- Yarn;
- Hive.


All credits go to [@kadensungbincho](https://github.com/kadensungbincho). It's highly recommended read his [article](https://kadencho.medium.com/hands-on-apache-ranger-docker-poc-with-hadoop-hdfs-hive-presto-814344a03a17) on Medium platform.

## Quickstart

1. Run the command: `docker-composes up`
2. The process will starts (the first execution requires some time since it needs to download all images);
3. Waits until the Ranger Web UI is ready in `localhost:6080` (when is started, a log in ranger-admin component like `Starting Apache Ranger Admin Service` will appears)

## NOTE:

 - Starting all components can take some time, and in my machine, all processes used approximately 4GB RAM.
