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
git commit -m "mensagem"
git commit -am "mensagem" todos os arquivos
-------------------------
visualizando logs
git log
git log --decorate    
git log --author="nome"  filtrar pelo autor
git shortlog    mostra em ordem alfabetica os autores
git shortlog -sn quantidade de commit e nome
git log --graph   mostra de forma grafica
git show +hash  mostra pela hash
---------------------------
visualizando mudancas antes de enviar.
git diff    mostra a modificacao
git diff --name-only   nome somente dos aqrquivos modificados 
----------------------------
desfazendo coisas
git checkout nomearquivo   retorna para antes da midificacao
git reset HEAD nomearquivo 
git reset --soft +hash  mata o commit mas fica no staged   
git reset --mixed +hash   mata o comite e fica antes do staged
git reset --hard +hash  ignora o comite e mata tudo
-----------------------------
ligando repositorio local a um remoto
git remote add origin git@github.com:xXfabio/curso-angular.git
git branch -M main 
git push -u origin main       envia todos os arquivos
------------------------------
clonando 
git clone endereço repositorio
-------------------------------
fork
------------------------------
branch
git checkout -b teste    cria um novo breanch
git branch     lista os breanch
git checkout nomeBranch   muda o branch
git branch -D nomeBranch   deleta git 
--------------------------------
merge e rebase
git log --graph     mostra os commit em grafico
git merge nomeBranch  
git rebase nomeBranch  
---------------------------------
gitignore
.gitignore   cria o arquivo
---------------------------------
stash  quarda a modificação pra depois 
git slash
git stash aplay
git slash list
git slash clear
----------------------------------
criando atalhos
git config --global alias.letraAtalho oComando
-----------------------------------
criando tags
git tag    mostra todas as tags
git tag -a 1.0.0 -m "mensagem" cria atag
git push origin master --tag  manda a tag
------------------------------------
reverter commit
git revert hashCommit
------------------------------------
apagamdo tags e branches remoto
git push origin :nomeTag
git push origin :nomeBranch

