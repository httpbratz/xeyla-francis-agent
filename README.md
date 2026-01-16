# Francis Agent

Agent IA conversationnel déployé sur ArgoCD + AWS EKS.

## Déploiement

L'agent est déployé automatiquement via ArgoCD depuis ce repository.

### Configuration

- **Environnement**: Development
- **Cluster**: AWS EKS (xeylaChat)
- **Namespace**: francis-dev
- **Secrets**: AWS Secrets Manager

### Services

- **API**: Interface REST
- **Workers**: Traitement asynchrone avec KEDA auto-scaling
- **Monitoring**: Better Stack

## Infrastructure

- ArgoCD pour GitOps
- External Secrets Operator
- KEDA pour auto-scaling
- AWS Secrets Manager