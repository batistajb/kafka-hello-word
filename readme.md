
### Criar tópico 
``` kafka-topics --create --topic=topico1 --bootstrap-server=localhost:9092 --partitions=3 ``` 

### Listar tópicos 
```kafka-topics --list --bootstrap-server=localhost:9092 ```

### Detalhes do tópico 
``` kafka-topics --bootstrap-server=localhost:9092 --topic=topico1 --describe ```
 
### Consumir 
``` kafka-console-consumer --bootstrap-server=localhost:9092 --topic=topico1 ```
- --from-beginning (todas ocorrências)
- --group=x (agrupar consumers/partições distribuídas)

### Produzir
```kafka-console-producer --bootstrap-server=localhost:9092 --topic=topico1```

### Detalhes do grupo
``` kafka-consumer-groups --bootstrap-server=localhost:9092 --group=x --describe ```
