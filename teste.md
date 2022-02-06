Configurando o git

gitconfig sistema como um todo do usuario e do projeto

para todos os repositorio do usuario global
git config –global user.name “nome”

git config –global user.email “e-mail”

definir editor
git config –global core.editor editor

mostrar informações
git config user.name
git config user.email
git config –list
-------------------------------
inicializando o repositorio
criando a pasta do projeto
mkdir git-course

inicializando o projeto na pasta
git init
---------------------------------
ciclo de vida dos arquivos
untracked
acabou de ser adicionado mas ainda nao foi visto  
pelo git
unmodified
existe mais nao teve modificacao
modified
arquivo modificado
staged
subir os arquivos

--------------------
comandos git
git status
git add arquivo
---------------------
committed
ciar a versao do arquivo
git commit -m "add teste.md"
