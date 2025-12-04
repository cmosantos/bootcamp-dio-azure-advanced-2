# Módulo 3 – Criando Containers com Docker

## 1. Conceitos essenciais

- Diferença entre máquina virtual e container
- **Imagem** x **container**
- Dockerfile, volumes, networks e Docker Hub

## 2. Instalação e primeiros comandos

- Instalação do Docker Desktop/engine
- Comandos básicos:
  - `docker pull`
  - `docker run`
  - `docker ps` / `docker ps -a`
  - `docker stop` / `docker rm`
  - `docker images`

## 3. Armazenamento com volumes

- Volumes para persistir dados mesmo após remover containers
- Bind mounts x volumes gerenciados
- Uso de volumes para bancos de dados e logs

## 4. Logs, rede e troubleshooting

- `docker logs` para inspecionar saída da aplicação
- Redes:
  - bridge (padrão)
  - comunicação entre containers no mesmo network
- Exposição de portas (`-p host:container`)

## 5. Dockerfile e Docker Compose

- Estrutura típica de um Dockerfile:
  - `FROM`, `WORKDIR`, `COPY`, `RUN`, `CMD` / `ENTRYPOINT`
- Docker Compose:
  - definir vários serviços em `docker-compose.yml`
  - subir e derrubar stack completa (`docker compose up/down`)

## 6. Desafios práticos

- Projetos com simulação de microsserviços
- Desafios de lógica usando comandos Docker para:
  - criar, parar, remover e inspecionar containers

## 7. Conclusão

Esse módulo mostrou como:
- empacotar aplicações em imagens
- rodar ambientes completos com poucos comandos
- preparar o terreno para orquestração com Kubernetes
