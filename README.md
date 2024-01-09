# installKafka
# feature 0001

пример раздачи ACL

./kafka-acls.sh --bootstrap-server 192.168.0.137:9092 \
  --command-config /home/alex/kafka.prop \
  --add \
  --allow-principal User:qqq \
  --allow-principal Group:qqq \
  --operation All \
  --topic qwe001


почему-то работает не * как минимум для групп

после этой команды (kafka-acls.hs) должна сработать вот эта
root@kafka002:/u01/kafka/current/bin# ./kafka-console-consumer.sh --bootstrap-server=192.168.0.137:9092 --topic=qwe001 --from-beginning --consumer.config=/home/alex/qqq.prop --group qqq

sgsd
gs
dg
sg
s
gs
