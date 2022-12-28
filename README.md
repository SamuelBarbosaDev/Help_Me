# Help Me
__Do you need help?__

## UBUNTU:

1. Lista dos programas instalados atualmente.
```
dpkg --list
```


2. Desinstalar Softwares no Ubuntu.
```
sudo apt-get --purge remove nomedoprograma
```


3. Lista os diretorios ocultos.
```
ls -a
```


4. Interragi com os diretorios.
```
cd nomedodiretorio
```


5. Criar um arquivo
```
touch nomedoaquivo.txt
```

6. Crie um diretorios.
```
mkdir nomedodiretorio
```


## GIT:

1. Seguinte comando pode ser usado para definir o email:
```
git config --global user.email "samueloficial@protonmail.com"
```


2. Seguinte comando pode ser usado para definir o Nome:
```
git config --global user.name "SamuelBarbosaDev"
```


3. Clona o repositorio:
```
git clone https://github.com/SamuelBarbosaDev/My_Site.git
```


4. Diz qual é o status do repositorio
```
git status
```


5. Adiciona o arquivo ao índice:
```
git add nomedoarquivo.extenção
```


6. O comando git commit é usado para confirmar as alterações na cabeça:
```
git commit –m “coloque sua mensagem aqui”
```


7. Envia as alterações feitas para o ramo mestre do repositório remoto:
```
git push
```


9. nome configurado:
opções:
--local
--global
--system

```
git config --local user.name "SeuUserName"
```


10. E-mail configurando:
opções:
--local
--global
--system

```
git config --local user.email "samueloficial@protonmail.com"
```


11. salva usuario e senha por 8 horas:
opções:
--local
--global
--system

```
git config --local credential.helper 'cache --timeout=28800'
```


12. salva usuario e senha permanente:
opções:
--local
--global
--system

```
git config --local credential.helper cache
```

13. echo "# Meu-Portfolio" >> README.md
```
git init
```

```
git add README.md
```

```
git commit -m "first commit"
```

```
git branch -M main
```

```
git remote add origin https://github.com/SamuelBarbosaDev/Meu-Portfolio.git
```

```
git push -u origin main
```
## Django:

Criar Projeto.
```
django-admin startproject nome_do_projeto
```

Criar Aplicação.
```
python manage.py startapp nome_da_app
```

Criar Migrações.
```
python mananage.py makemigrations
```

Executar Migrações.
```
python manage.py migrate
```

Executar Servidor de Desenvolvimento.
```
python manage.py runserver
```

Limpar Banco de Dados.
```
python manage.py flush
```

Abrir Shell do Banco de Dados Configurado.
```
python manage.py dbshell
```

Mapear BD existente para o projeto Django.
```
python manage.py inspectdb > nome_da_app.models.py
```
## Python:

adicionando todas as Libs ao arquivo requeriments.txt:
```
pip freeze > requirements.txt
```

adiciona libs especificas ao arquivo requeriments.txt:
```
pip freeze | grep jwt >> requirements.txt 
```

## PostgreSQL:

Como acessar o prompt de comando do PostgreSQL:
```
sudo -u postgres psql postgres
```

Para sair do prompt de comando do PostgreSQL:
```
\q 
```

Como encontrar as informações sobre o banco de dados:
```
select version();
```

Lista dos bancos de dados no cluster:
```
\l+
```

Lista de usuários no cluster:
```
\du+
```

Lista de tablespaces customizados no cluster:
```
\db+
```

Criar usuario:
```
sudo -u postgres createuser -d -P samuelbarbosa_dev
```

Mais informações sobre o createuser do PostgreSQL:
```
createuser --help
```

Criando um banco de dados:
```
sudo -u postgres createdb -O nomedousuario nomedobancodedados
```
Output:
==========================================================================================================
createuser cria uma nova role do PostgreSQL.

Uso:
  createuser [OPÇÃO]... [NOME_ROLE]

Opções:
  -c, --connection-limit=N  limite de conexão por role (padrão: ilimitado)
  -d, --createdb            role pode criar novos bancos de dados
  -D, --no-createdb         role não pode criar novos bancos de dados (padrão)
  -e, --echo                mostra os comandos enviados ao servidor
  -g, --role=ROLE           nova role será um membro desta role
  -i, --inherit             role herda privilégios de roles das quais ela
                            é um membro (padrão)
  -I, --no-inherit          role não herda privilégios
  -l, --login               role pode efetuar login (padrão)
  -L, --no-login            role não pode efetuar login
  -P, --pwprompt            atribui uma senha a nova role
  -r, --createrole          role pode criar novas roles
  -R, --no-createrole       role não pode criar novas roles (padrão)
  -s, --superuser           role será super-usuário
  -S, --no-superuser        role não será super-usuário (padrão)
  -V, --version                mostra informação sobre a versão e termina
  --interactive             pergunta pelo nome e atributos não informados da role
                            ao invés de utilizar o padrão
  --replication             role pode iniciar replicação
  --no-replication          role não pode iniciar replicação
  -?, --help                   mostra essa ajuda e termina

Opções de conexão:
  -h, --host=MÁQUINA        máquina do servidor de banco de dados ou diretório do soquete
  -p, --port=PORTA          porta do servidor de banco de dados
  -U, --username=USUÁRIO    nome do usuário para se conectar (não é o usuário a ser criado)
  -w, --no-password         nunca pergunta senha
  -W, --password            pergunta senha

Relate erros a <pgsql-bugs@lists.postgresql.org>.
página web do PostgreSQL: <https://www.postgresql.org/>
 
==========================================================================================================
