# Help Me
__Do you need help?__

### Indice:
- [Help Me](#help-me)
    - [Indice:](#indice)
  - [Ubuntu:](#ubuntu)
  - [Git:](#git)
  - [Django:](#django)
  - [Python:](#python)
  - [PostgreSQL:](#postgresql)
  - [Docker:](#docker)
  - [Docker Compose:](#docker-compose)

## Ubuntu:
Lista dos programas instalados atualmente:
```shell
dpkg --list
```

Desinstalar Softwares no Ubuntu:
```shell
sudo apt-get --purge remove nomedoprograma
```

Lista os diretorios ocultos:
```shell
ls -a
```

Interragi com os diretorios:
```shell
cd nomedodiretorio
```

Criar um arquivo:
```shell
touch nomedoaquivo.txt
```

Crie um diretorios:
```shell
mkdir nomedodiretorio
```

Verifica atualizações de todos os pacotes de um sistema Linux:
```shell
sudo apt-get upgrade
```

O comando pwd informa o diretório absoluto corrente:
```shell
pwd
```

Entra na pasta:
```shell
nautilus nome_da_pasta
```

Intalando atualizações dos seus apps:
```shell
sudo dpkg -i nome_do_arquivo.deb
```

## Git:
Seguinte comando pode ser usado para definir o email:
```shell
git config --global user.email "samueloficial@protonmail.com"
```

Seguinte comando pode ser usado para definir o Nome:
```shell
git config --global user.name "SamuelBarbosaDev"
```

Clona o repositorio:
```shell
git clone https://github.com/SamuelBarbosaDev/My_Site.git
```

Diz qual é o status do repositorio:
```shell
git status
```

Adiciona o arquivo ao índice:
```shell
git add nomedoarquivo.extenção
```

O comando git commit é usado para confirmar as alterações na cabeça:
```shell
git commit –m “coloque sua mensagem aqui”
```

Envia as alterações feitas para o ramo mestre do repositório remoto:
```shell
git push
```

Nome configurado:
opções:
--local
--global
--system

```shell
git config --local user.name "SeuUserName"
```

E-mail configurando:
opções:
--local
--global
--system

```shell
git config --local user.email "samueloficial@protonmail.com"
```

Salva usuario e senha por 8 horas:
opções:
--local
--global
--system

```shell
git config --local credential.helper 'cache --timeout=28800'
```

Salva usuario e senha permanente:
opções:
--local
--global
--system

```shell
git config --local credential.helper cache
```

echo "# Meu-Portfolio" >> README.md
```shell
git init
```

```shell
git add README.md
```

```shell
git commit -m "first commit"
```

```shell
git branch -M main
```

```shell
git remote add origin https://github.com/SamuelBarbosaDev/Meu-Portfolio.git
```

```shell
git push -u origin main
```

## Django:
Criar Projeto:
```shell
django-admin startproject nome_do_projeto
```

Criar Aplicação:
```shell
python manage.py startapp nome_da_app
```

Criar Migrações:
```shell
python mananage.py makemigrations
```

Executar Migrações:
```shell
python manage.py migrate
```

Executar Servidor de Desenvolvimento:
```shell
python manage.py runserver
```

Limpar Banco de Dados:
```shell
python manage.py flush
```

Abrir Shell do Banco de Dados Configurado:
```shell
python manage.py dbshell
```

Mapear BD existente para o projeto Django:
```shell
python manage.py inspectdb > nome_da_app.models.py
```
## Python:
Criando ambiente virtual:
```shell
python3 -m venv venv
```

Ativando ambiente virtual:
```shell
source venv/bin/activate
```

Adicionando todas as Libs ao arquivo requeriments.txt:
```shell
pip freeze > requirements.txt
```

Adiciona libs especificas ao arquivo requeriments.txt:
```shell
pip freeze | grep jwt >> requirements.txt 
```

Atualizando um pacote:
```shell
pip install --upgrade <package-name>
```

Removendo Varios pacotes:
```shell
pip uninstall -r requirementstmp.txt -y
```

## PostgreSQL:
Como acessar o prompt de comando do PostgreSQL:
```shell
sudo -u postgres psql postgres
```

Para sair do prompt de comando do PostgreSQL:
```shell
\q 
```

Como encontrar as informações sobre o banco de dados:
```shell
select version();
```

Lista dos bancos de dados no cluster:
```shell
\l+
```

Lista de usuários no cluster:
```shell
\du+
```

Lista de tablespaces customizados no cluster:
```shell
\db+
```

Criar usuario:
```shell
sudo -u postgres createuser -d -P samuelbarbosa_dev
```

Mais informações sobre o createuser do PostgreSQL:
```shell
createuser --help
```

Criando um banco de dados:
```shell
sudo -u postgres createdb -O nomedousuario nomedobancodedados
```

Excluí o banco de dados:
```shell
DROP DATABASE databasename; 
```

Excluí o usuário:
```shell
DROP USER nomedousuario;
```

Conectando ao banco de dados:
```shell
\connect nomedobancodedados
```

## Docker:
Verificarmos informações do Docker Host:
```shell
docker info
```

Verificando a versão do cliente:
```shell
docker version
```

Listarmos as imagens:
```shell
docker images
```

Procurando uma imagem:
```shell
docker search postgres
```

Baixando imagem:
```shell
docker pull postgres
```

Criando um container:
```shell
docker run container_nome
```

Para o container:
```shell
docker stop container_nome
```

Lista os containers:
```shell
docker ps 
```

Lista todos os containers:
```shell
docker ps -a
```

Informações sobre um container:
```shell
docker stats container_nome
```

Detalhes da imagem:
```shell
docker inspect postgres
```

Deletar a imagem:
```shell
docker rmi postgres
```

Executar qualquer comando no containers sem precisar estar na console:
```shell
docker exec container_nome
```

Criando imagem personalizada:
```shell
docker build -t NOME_DA_IMAGEM CAMINHO_DO_DOCKERFILE
```

Criando um volume, exemplo:
```shell
docker run -d --name db -e POSTGRES_PASSWORD=postgres -v db_volume:/var/lib/postgresql/data -p 5433:5432 postgres
```

## Docker Compose:
Cria e inicia os contêineres:
```shell
docker-compose up
```

Cria e inicia os contêineres em segundo plano:
```shell
docker-compose up -d
```

Remove todos os contêineres:
```shell
docker-compose down
```

Lista os contêineres em execução:
```shell
docker-compose ps
```

Exibe os logs dos contêineres:
```shell
docker-compose logs
```

Executa um comando dentro de um contêiner específico definido no arquivo `docker-compose.yml`:
```shell
docker-compose exec meu-servico bash
```

Reconstrói as imagens dos contêineres a partir do Dockerfile:
```shell
docker-compose build
```

Atualiza as imagens dos contêineres a partir do registro (como Docker Hub):
```shell
docker-compose pull
```

Inicia os contêineres de acordo com um arquivo:
```shell
docker-compose -f /caminho/para/outro/docker-compose.yml up
```
