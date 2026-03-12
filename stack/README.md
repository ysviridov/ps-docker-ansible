# 12.12. Домашнее задание - Docker swarm

Установка метки pg на ноду для размещения базы данных.

```bash
docker node update --label-add pg=true <node-name>
```

Деплой стэка:

```bash
   docker stack deploy -c docker-stack.yml mystack
```

Проверки:

```bash
docker stack ps mystack
docker service ls
docker service ps mystack_nginx
docker service ps mystack_postgres
```
