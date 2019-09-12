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
