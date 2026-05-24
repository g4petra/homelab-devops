# Infraestrutura do Homelab

## Objetivo

Ambiente de estudos para:
- DevOps
- Docker
- Infraestrutura
- Backend
- Aplicações web
- Virtualização

---

# Hardware

## Servidor principal

- Intel i7-4770
- 16 GB RAM
- SSD 256 GB
- HD 1 TB
- Fonte 400W

---

# Virtualização

## Proxmox VE

Função:
- Host principal de virtualização
- Gerenciamento de VMs
- Snapshots
- Infraestrutura do laboratório

---

# Rede

## Tailscale

Objetivo:
- Acesso remoto seguro
- VPN privada
- Administração remota do Proxmox e VMs

---

# VM Principal

## ubuntu-docker

Configuração:
- 4 vCPU
- 6 GB RAM
- 80 GB SSD
- IP fixo: 192.168.100.109

Função:
- Host Docker principal
- Backend
- Frontend
- Banco de dados
- Reverse proxy

---

# Docker

Objetivo:
- Gerenciamento de containers
- Isolamento de serviços
- Facilidade de deploy

---

# Containers Atuais

## Portainer
Função:
- Administração visual do Docker

## PostgreSQL
Função:
- Banco de dados principal do sistema

## Caddy
Função:
- Reverse proxy
- HTTPS
- Roteamento de aplicações

---

# Estrutura de Diretórios

```text
/srv
├── backups
├── docker
│   ├── backend
│   ├── caddy
│   ├── cloudflared
│   ├── frontend
│   ├── portainer
│   └── postgres
├── logs
└── uploads
```

---

# Próximos Passos

- Estruturar backend
- Criar autenticação
- Modelar banco
- Criar frontend
- Configurar domínio
- Configurar Cloudflare Tunnel
- Implementar IA auxiliar