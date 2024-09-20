### kafka - Curso na Udemy
#### 18/09/2024

Kafka CLI

#### Criar um tópico
- kafka-topics --bootstrap-server localhost:9092 --create --topic nome-do-tópico --partitions 1 --replication-factor 1

#### Listar o(s) tópico(s)
- kafka-topics --bootstrap-server localhost:9092 --list

#### Listar o(s) grupo(s)
- kafka-consumer-groups --bootstrap-server localhost:9092 --list

#### Producer - Enviar mensagem para o tópico
- kafka-console-producer --broker-list localhost:9092 --topic nome-do-tópico

#### Consumer - Receber mensagem Kafka
- kafka-console-consumer --bootstrap-server localhost:9092 --topic nome-do-tópico --group nome-do-grupo

#### Exibir as mensagens do Kafka
- kafka-console-consumer --bootstrap-server localhost:9092 --topic nome-do-tópico --from-beginning

#### Excluir um tópico
- kafka-topics --bootstrap-server localhost:9092 --delete --topic nome-do-tópico

#### Excluir um grupo
- kafka-consumer-groups --bootstrap-server localhost:9092 --delete --group nome-do-grupo