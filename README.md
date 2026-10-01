# Azure Linux Web Server

Projeto prático de Cloud Infrastructure utilizando Microsoft Azure, Ubuntu Linux e NGINX.

## 🎯 Objetivo

Provisionar uma máquina virtual Linux no Microsoft Azure, configurar acesso remoto via SSH, instalar e configurar o NGINX e publicar uma página HTML acessível pela Internet.

## ☁️ Ambiente

- **Cloud:** Microsoft Azure
- **Subscription:** Azure for Students
- **Sistema operacional:** Ubuntu Server 24.04 LTS
- **Web Server:** NGINX
- **Acesso remoto:** SSH
- **Protocolo web:** HTTP
- **Arquitetura:** VM Linux + VNet + Subnet + IP público

## 🛠️ Implementações

- Criação do Resource Group
- Provisionamento da VM Ubuntu
- Configuração de autenticação por chave SSH
- Configuração de rede virtual e subnet
- Configuração de acesso SSH pela porta TCP 22
- Instalação do NGINX
- Validação do serviço NGINX
- Validação da porta HTTP 80
- Criação de página HTML personalizada
- Publicação da página através do IP público da VM

## 🔎 Troubleshooting

Durante o laboratório foram investigados e solucionados problemas relacionados a:

- Caminho incorreto da chave SSH
- Permissões da chave privada no Windows
- Autenticação SSH
- Localização de arquivos no Linux
- Permissões administrativas com `sudo`
- Falha na instalação inicial do NGINX
- Validação da configuração do NGINX
- Inicialização e status do serviço
- Verificação das portas TCP
- Edição e publicação do arquivo HTML

## 🐧 Comandos Linux praticados

```bash
whoami
hostname
ip addr
df -h
free -h
uptime
ss -tuln
ls
ls /var/www/
ls /var/www/html/
cat /var/www/html/index.nginx-debian.html
sudo nano /var/www/html/index.nginx-debian.html
sudo nginx -t
sudo systemctl start nginx
sudo systemctl status nginx
