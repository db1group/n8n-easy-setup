# Instruções para setup facilitado do N8N com Docker

> **O que é Docker?** Docker é um programa que permite rodar outros programas de forma fácil, sem precisar instalar tudo manualmente. O Docker Compose ajuda a gerenciar vários serviços juntos.

> **O que é N8N?** N8N é uma ferramenta de automação que permite conectar diferentes aplicativos e serviços para automatizar tarefas.

## Instalando o Docker e Docker Compose

### Windows
O Docker deve rodar no WSL2 (Windows Subsystem for Linux).
- Verifique se o WSL2 está instalado e configurado corretamente: https://learn.microsoft.com/pt-br/windows/wsl/install
- Instale o Rancher Desktop para Windows, que inclui o Docker: https://rancherdesktop.io/

### Linux 
Você pode utilizar o script rápido de instalação do Docker. Abra o terminal (Ctrl+Alt+T) e execute os comandos abaixo, um de cada vez:

```bash
curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh get-docker.sh
```

> Se pedir senha, digite a senha do seu usuário. Se aparecer alguma mensagem de erro, confira se você está usando um usuário com permissões de administrador (sudo).

Mais detalhes sobre a instalação do Docker podem ser encontrados em: https://docs.docker.com/engine/install/

### MacOS
Você pode baixar Rancher Desktop, que inclui o Docker: https://rancherdesktop.io/

> Caso necessário, instale as ferramentas de linha de comando do Docker e Docker Compose com o Homebrew. No terminal, digite:

```bash
brew install docker docker-compose
```

> Caso não tenha o Homebrew instalado, você pode seguir as instruções em: https://brew.sh/

## Executando o N8N com Docker

1. Baixe ou clone este repositório:
    - Via terminal, execute o comando:
        ```bash
        git clone https://github.com/db1group/n8n-easy-setup.git
        ```
    - Ou baixe o arquivo ZIP do repositório e extraia-o: https://github.com/db1group/n8n-easy-setup/archive/refs/heads/master.zip

1. No terminal, navegue até o diretório onde o repositório foi clonado ou extraído:
    ```bash
    cd n8n-easy-setup
    ```

1. Rode o comando para executar o Docker Compose e iniciar o N8N:
    ```bash
    docker-compose up -d
    ```
    > Aguarde alguns segundos. Para verificar se o N8N está rodando, execute:

1. Acesse o N8N pelo navegador em: [http://localhost:5678](http://localhost:5678)
