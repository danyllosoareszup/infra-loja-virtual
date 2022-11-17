# terraform ec2 cloudwatch

## Como usar?

1. Ajuste variables.tf de acordo com o seu ambiente

2. Para criar o ambiente:

```bash
make start
```

*Pode levar até 5min para a instância se tornar operacional*

3. Acesse a instância e execute:

```bash
sudo su - 
bash -c 'cd /opt/lojavirtual && git checkout main'
docker-compose -f /opt/lojavirtual/docker/docker-compose.yml up -d
```

4. Para destruir o ambiente:

```bash
make stop
```



# infra-loja-virtual
