# Rabbit MQ Sample

Exemple canonique de file d'attente **RabbitMQ** : producteur et consommateur Python
(`pika`) échangés via un conteneur `rabbitmq:3`.

Utilisé comme sous-module dans [`notebook-containers-intro`](https://github.com/ebpro/notebook-containers-intro).

## Usage

```bash
./run.sh
```

Le script :

1. construit l'image client `rabbitmq-client` (Python + pika),
2. crée le réseau Docker `mq-net`,
3. lance le broker `rabbitmq:3`,
4. publie un message (producteur) puis le consomme,
5. arrête le broker.

Prérequis : Docker en fonctionnement.
