install kafka
https://kafka.apache.org/quickstart

edit config/server.properties:

log.dirs=C:\kafka\kafka-logs

zookeeper.properties

dataDir=C:\kafka\zookeeper-data


start zookeeper:

C:\>cd kafka

C:\kafka>.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties





create topic:
bin\windows\kafka-topics.bat --create ^
--bootstrap-server localhost:9092 ^
--replication-factor 1 --partitions 1 ^
--topic mytopic


list topics:

.\bin\windows\kafka-topics.bat --list --bootstrap-server localhost:9092



https://www.kafkatool.com/download.html
