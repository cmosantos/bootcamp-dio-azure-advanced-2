# Lab – Pipeline GitLab, Docker e Kubernetes

## Objetivo

Simular um fluxo moderno de entrega contínua:

1. Código versionado no GitLab
2. Build de imagem Docker
3. Deploy automatizado em Kubernetes

## Componentes

- Repositório GitLab
- Dockerfile da aplicação
- Arquivo `.gitlab-ci.yml`
- Manifests YAML de Deployment e Service

## Fluxo

1. Desenvolvedor faz commit e push
2. Pipeline:
   - compila e testa aplicação (quando configurado)
   - gera imagem Docker
   - envia a imagem para registry
   - aplica manifests no cluster Kubernetes
3. Nova versão sobe automaticamente no cluster

## Aprendizados

- Entendimento de CI/CD na prática
- Importância de padronizar build e deploy
- Integração entre Git, Docker e Kubernetes
