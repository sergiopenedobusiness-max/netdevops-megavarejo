# Infraestrutura como Código (IaC) - NetDevOps
Repositório de automação da **MegaVarejo Cloud**.

## Arquitetura de Rede
- **VLAN 10:** CI/CD Pipeline (Esteiras e runners)
- **VLAN 30:** Banco de Dados Produção
- **Mecanismo:** Ansible declarativo com `state: merged` (Idempotência garantida).
- **Validação:** Esteira automatizada de CI via GitHub Actions com `yamllint` e `ansible-lint`.