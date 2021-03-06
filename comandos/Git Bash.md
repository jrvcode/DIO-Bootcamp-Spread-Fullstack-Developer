# Comandos Essenciais Git Bash

#### Clonar repositorio do GITHUB para sua maquina
    $ git clone nome_do_caminho_ssh_do_githut
    $ git clone git@github.com:nome_git/nome_repositorio.git

#### Iniciar repositorio / Criar repositorio .git
    $ git init

#### Adicionar arquivos para 'commint'
    $ git add nome_arquivo

#### Adiciona todos arquivos para poder receber o "commit"
    $ git add *
    $ git add .

#### Cria arquivos commit para enviar para 'push'
    $ git commit

#### Prepara os arquivos selecionados para receber a "push"
    $ git commit -m "comentario_do_commit"
    $ git commit -m "commit inicial"

#### Verifica os status dos arquivos
    $ git status

#### Verifica os status da configurações do git
    $ git config --list

#### Remover e email ou nome configurado
    $ git config --global --unset user.email 
    $ git config --global --unset user.name

#### Configura repositorio do Git na pasta original para fazer os push e pull
    $ git remote add origin https://github.com/nome_git/nome_repositorio.git

#### Verificar lista de repositorios	
    $ git remote -v

#### Envia arquivos locais para repositorio remoto
    $ git push origin master
    $ git push origin main

#### Recebe arquivos remotos no repositorio local 
    $ git push origin master
    $ git push origin main


# Comando para configurar SSH do no seu GIT para Github

#### Criar minha chave publica e privada
    $ ssh-keygen -t ed25519 -C seu_email@gmail.com

#### Inicializar chave criada / Start key
    $ eval $(ssh-agent -s)

#### Ativar chave para o agente
    $ ssh-add id_ed25519

#### Configurar e-mail do autor para o commit
    $ git config --global user.mail "seu_email@gmail.com"

#### Configurar name do autor do commit
    $ git config --global user.name seu_nome_de_usuario


# Comandos Essenciais 
## Windows
- #### Comandos Básicos para Shell
    - cd
    - dir
    - mkdir
    - del / rmdir

## Unix
- ### Comandos Básicos para Shell
    - cd
    - ls
    - mkdir
    - rm -rf


## Criando arquivos com comando no Shell

    $ echo hello > hello.txt

    $ echo "Olá mundo!" | openssl sha1
    $ echo "Olá mundo!" | openssl sha1 > teste.txt

    $ echo 'conteudo' | git hash-object --stdin

### BLOB
    $ echo -e  'conteudo' | openssl sha1
    $ echo -e 'blob 9\0conteudo' | openssl sha1

### TREE
    $