# kafka-docker-setup


```
docker compose up -d

```

Now once the container is up use the below command to enter into the kakfa-shell

```
docker exec -it -w /opt/kafka/bin broker sh

```

If you are working with let suppose Node or Sprint or Python then you will use the dedicated pacakges to work with kafka to create topics n all but if you are doing it through shell the use the below commands


Create Topic using Shell

```
 ./kafka-topics.sh --create --topic <topic_name> --bootstrap-server broker:<PORT_NUMBER>
 
```

List down all the topics


```
 ./kafka-topics.sh --bootstrap-server broker:<PORT_NUMBER>
 
```

Consume a Topic

```
./kafka-console-consumer.sh -- topic <topic_name> --from-beginning --bootstrap-server broker:29092

```
