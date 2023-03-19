# Help Me
__Do you need help?__

## UBUNTU:

1. Lista dos programas instalados atualmente:
```
dpkg --list
```


2. Desinstalar Softwares no Ubuntu:
```
sudo apt-get --purge remove nomedoprograma
```


3. Lista os diretorios ocultos:
```
ls -a
```


4. Interragi com os diretorios:
```
cd nomedodiretorio
```


5. Criar um arquivo:
```
touch nomedoaquivo.txt
```

6. Crie um diretorios:
```
mkdir nomedodiretorio
```

7. Verifica atualizações de todos os pacotes de um sistema Linux:
```
sudo apt-get upgrade
```

8. O comando pwd informa o diretório absoluto corrente:
```
pwd
```

9. Entra na pasta:
```
nautilus nome_da_pasta
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

Criando ambiente virtual
```
python3 -m venv venv
```

Ativando ambiente virtual:
```
source venv/bin/activate
```

adicionando todas as Libs ao arquivo requeriments.txt:
```
pip freeze > requirements.txt
```

adiciona libs especificas ao arquivo requeriments.txt:
```
pip freeze | grep jwt >> requirements.txt 
```

Atualizando um pacote:
```
pip install --upgrade <package-name>
```

Removendo Varios pacotes:
```
pip uninstall -r requirementstmp.txt -y
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

Excluí o banco de dados:
```
DROP DATABASE databasename; 
```

Excluí o usuário:
```
DROP USER nomedousuario;
```

Conectando ao banco de dados:
```
\connect nomedobancodedados
```
