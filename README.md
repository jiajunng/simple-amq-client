## RECV
mvn exec:java -Dexec.mainClass="com.redhat.demo.App" -D broker.url="failover://(amqp://192.168.0.110:5672)" -Dsend.queue=queue2 -Dsend.mode=RECV

## SEND

mvn exec:java -Dexec.mainClass="com.redhat.demo.App" -D broker.url="failover://(amqp://192.168.0.110:5672)" -Dsend.queue=queue2 -Dsend.msg=helloworld! -Dsend.mode=SEND
