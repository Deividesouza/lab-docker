# 🚀 DevOps Labs — Docker, Nginx, Kaniko e Traefik

Repositório criado para estudo e prática de **DevOps**, abordando desde os fundamentos do Docker até a configuração de proxies reversos e pipelines de build automatizados.

---

## 🧩 Laboratórios Concluídos

| Lab | Tema | Descrição |
|-----|------|------------|
| **Lab 1** | Fundamentos Docker | Criação, execução e gerenciamento de containers. |
| **Lab 2** | Dockerfile & Entrypoint | Construção de imagens personalizadas e uso de scripts de inicialização. |
| **Lab 3** | Build com Kaniko | Build de imagens sem daemon Docker (ideal para CI/CD). |
| **Lab 4** | Makefile e Pipeline | Automação de build, tag e push de imagens. |
| **Lab 5** | Nginx Proxy | Configuração de proxy reverso com Nginx para múltiplas aplicações. |
| **Lab 6** | Traefik Proxy | Implementação de proxy dinâmico com Traefik e dashboard. |
| **Lab 7** | Docker Compose Avançado — Redes e Volumes | Criação de Muilti-containeres com Docker Compose|
| **Lab 8** | Kubernetes (K3s/MicroK8s) — Deploy e Services | Iniciar Pods com K8s e Expose das portas com forward |
| **Lab 9** | Terraform — Provisionamento de Infraestrutura | Provisionamento de maquinas na AWS|
---

## 🔜 Próximos Labs

| Lab | Tema Planejado |
|-----|----------------|


| **Lab 10** | Ansible — Automação de Configuração |


---

## ⚙️ Execução Básica

## Para iniciar qualquer laboratório:
docker compose up -d

## Para visualizar logs de um serviço específico:
docker logs <nome-do-container>

## Para encerrar o ambiente:
docker compose down

## Conceitos Trabalhados

- Imagens e containers Docker

- Automação de build com Makefile

- Build de imagens com Kaniko

- Proxies reversos com Nginx e Traefik

- Organização modular de ambientes
  
- Fundamentos de pipelines DevOps
