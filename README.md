### Running rabbitmq examples, send and receive messages

#### How to Run:
Firtly, up the rabbit-mq container, inside third_part/rabbitmq run:
~~~
docker-compose up -d
~~~
Now, we can test, on the root folder, run:
~~~
go run cmd/send/send.go
~~~
This send a hello-world to rabbitmq, now, receive the message:
~~~
go run cmd/receive/receive.go
~~~
the receiving code keeps listening until it exits, press Ctr-c to exit.
