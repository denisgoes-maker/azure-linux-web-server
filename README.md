# Azure Linux Web Server

Projeto prático de Cloud Infrastructure utilizando Microsoft Azure, Ubuntu Linux e NGINX.

## Objetivo

Provisionar uma máquina virtual Linux no Azure, configurar acesso remoto via SSH, instalar um servidor web NGINX e publicar uma página HTML acessível pela Internet.

## Ambiente

- Cloud: Microsoft Azure
- Subscription: Azure for Students
- OS: Ubuntu Server 24.04 LTS
- Web Server: NGINX
- Acesso remoto: SSH
- Protocolo web: HTTP
- Arquitetura: VM Linux + rede virtual + IP público

## Implementações realizadas

- Criação do Resource Group
- Provisionamento da VM Ubuntu
- Configuração de autenticação por chave SSH
- Acesso remoto à VM via SSH
- Identificação de IP público e IP privado
- Diagnóstico de rede e portas
- Instalação do NGINX
- Validação da configuração do NGINX
- Inicialização e verificação do serviço
- Validação da porta TCP 80
- Criação de uma página HTML personalizada
- Publicação da página através do IP público da VM

## Troubleshooting

Durante o laboratório foram tratados problemas relacionados a:

- Caminho incorreto da chave SSH
- Permissões da chave privada no Windows
- Autenticação SSH
- Localização de arquivos no Linux
- Instalação do NGINX
- Erro 404 durante instalação de pacotes
- Permissões administrativas com `sudo`
- Validação do serviço NGINX
- Verificação da porta HTTP 80
- Edição e validação de arquivos HTML

## Comandos Linux praticados

```bash
whoami
hostname
ip addr
df -h
free -h
uptime
ss -tuln
systemctl status nginx
sudo systemctl start nginx
sudo nginx -t
ls
ls /var/www/
ls /var/www/html/
cat /var/www/html/index.nginx-debian.html
sudo nano /var/www/html/index.nginx-debian.html
