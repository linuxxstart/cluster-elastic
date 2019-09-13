# cluster_elastic
Subindo cluster elastic com autenticação e controle de acesso de usuários
# Instalando docker, docker-compose e aumentando o mapeamento de arquivo em memória
```
# curl -fsSL https://get.docker.com | sh
# curl -L "https://github.com/docker/compose/releases/download/1.24.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
# chmod +x /usr/local/bin/docker-compose
# ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose
# echo vm.max_map_count=262144 >> /etc/sysctl.conf && sysctl -p
```
# Arquivo .ENV
O arquivo .env contém a senha do usuário elastic (para logar no kibana) e nome do projeto compose.
# Subindo o cluster
```
# docker-compose -f create-certs.yml run --rm create_certs
# docker-compose up -d
```
![kibana](https://user-images.githubusercontent.com/55243431/64805565-bf56df00-d567-11e9-87e8-116eb3f299e6.png)
![cluster_elastic](https://user-images.githubusercontent.com/55243431/64883926-d0225600-d636-11e9-80fd-dd81439435e4.png)
