# Módulo 4 – Orquestração de Contêineres com Kubernetes

## 1. Conceitos principais

- Estrutura de um cluster:
  - **Master/Control Plane**
  - **Nodes (trabalhadores)**
- Objetos fundamentais:
  - **Pod** – unidade mínima de execução
  - **Deployment** – controla réplicas e atualizações
  - **Service** – expõe os pods e oferece IP estável

## 2. Ambiente de desenvolvimento Kubernetes

- Utilização de `kubectl` para:
  - listar recursos (`get`)
  - inspecionar (`describe`)
  - aplicar manifests (`apply`)
- Manifestos YAML para:
  - deployments
  - services
  - volumes/persistent volumes (quando necessário)

## 3. Clusters em nuvem

- Vantagens de usar cluster gerenciado:
  - alta disponibilidade
  - atualizações automáticas
  - integração com serviços de nuvem
- Conceitos de:
  - autoscaling
  - monitoramento
  - observabilidade

## 4. Pipeline GitLab + Docker + Kubernetes

- Etapas do desafio de projeto:
  - código versionado no GitLab
  - pipeline CI/CD com:
    - build da imagem Docker
    - push para um registry
    - deploy no cluster Kubernetes aplicando manifests
- Benefícios:
  - padronização do processo
  - menos tarefas manuais
  - facilidade para rollback

## 5. Conclusão

Esse módulo conectou:
- containers Docker → orquestração Kubernetes
- código em repositório → pipeline automatizado
- necessidade de alta disponibilidade → uso de réplicas e services
