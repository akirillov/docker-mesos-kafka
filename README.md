# Apache Kafka Mesos Scheduler
Apache Kafka on Apache Mesos in Docker

## Usage

This project simply encapsulates the `mesos/kafka` project in a Docker container to allow easy scheduling with Marathon. For all configration options please see: https://github.com/mesos/kafka#scheduler-configuration

```
docker pull yagni/mesos-kafka
docker run -p 7000:7000 yagni/mesos-kafka scheduler --master=leader.mesos:5050 --zk=leader.mesos:2181 --api=http://kafka-mesos.marathon.mesos:7000 --storage=zk:/kafka-mesos
```



