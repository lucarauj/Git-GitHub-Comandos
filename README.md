[![NPM](https://img.shields.io/npm/l/react)](https://github.com/lucarauj/Git-GitHub-Comandos/blob/main/LICENSE)

<h1 align="center">Comandos Git/GitHub</h1>

<p align="center"><img width="450px" src="https://github.com/lucarauj/assets/blob/main/Git_GitHub.jpg"/></p>

## Configurando identificação no Git:

```
git config --global user.name "Seu nome"
git config --global user.email "Seu email de cadastro do Github"

git config --list
```

## Verificando arquivos dentro de uma pasta:

```
ls
```

## Limpando a tela do terminarl GIT:

```
clear
```

## Verificando o remote:

```
git remote -v
```

## Salvando um projeto no GitHub:

```
git init 
git add . (envia arquivos para stage)
git status (mostra o status do projeto)[modified/untracked/deleted]
git commit -m "Mensagem do trabalho adicionado"
git branch -M main
git remote add origin git@github.com:"usuario"/"repositório criado".git
git push OU git push -u origin main (envia os arquivos para o gitHub)[-u origin main: primeiro push]
```

## Salvando nova versão de um projeto no GitHub:

```
git status
git add .
git commit -m "Mensagem do trabalho adicionado"
git push
```

## Clonando um projeto do GitHub e modificando:

```
git clone git@github.com:"usuario"/"repositório criado".git
git add . (adiciona todas modificações)
git add "nome do arquivo" (adiciona somente o arquivo indicado)
git commit -m "Mensagem do trabalho adicionado"
git push
```

## Modificando mensagem do commit:

```
git commit --amend -m "Nova mensagem" 
```

## Navegando entre pastas no Git:

```
cd "nome da pasta" (avança)
cd .. (volta)
```

## Abrindo VS Code dentro de uma pasta do projeto:

```
code .
```

## Explorando a movimentação de um repositório:

```
git log
git log --oneline (forma resumida)
```

## Explorando a movimentação de um repositório (com detalhes):

```
git reflog
```

## Verificando a diferença entre modificações:

```
git diff "nome do arquivo"
```

## Criando uma branch:

```
git branch "nome da branch"
```

## Para subir essa branch para o repositório:

```
git push -u "remote" "nome-da-branch"
```

## Verificando as ramificações:

```
git branch OU git branch --list
```

## Trocando de branch:

```
git checkout "outra branch"
```

## Criando e mudando para uma branch:

```
git checkout -b "nome-da-branch"
```

## Verificando o último commit das branches:

```
git branch -v
```

## Deletando uma brach:

```
git branch -d "nome-da-branch"
```

## Modificando temporariamente arquivos do projeto ao estado de um dado commit ou branch:

Obs.: NÃO modificar o projeto enquanto estiver destacado em outro commit.
Caso isso aconteça, execute os seguinte comandos:

```
git reset
git clean -df
git checkout -- .
```

- HEAD: referencia o último commit do histórico da branch;
- HEAD ~ 1: penúltimo commit
- HEAD ~ 2: antipenúltimo commit

```
git checkout "código do commit"
```

```
git checkout main (volta ao último commit do branch main)
```

## Desfazendo modificações não salvas:

```
git status
git reset
git clean -df
git checkout -- .
```

## Desfazendo alterações que não foram enviadas para o stage:

```
git restore <nome do arquivo + extensão>
```

## Retirando arquivos/modificações do stage (add .):

```
git status
git reset
```
```
git status
git reset <nome do arquivo>
```

## Editor VIM:

- tecla 'i' para edição
- ESC :wq ENTER para salvar edição
- ESC :q! ENTER para NÃO salvar edição

## Desfazendo último commit mantendo as alterações:

```
git status
git reset --soft HEAD~1
```

## Desfazendo último commit e as alterações:

```
git status
git reset --hard "código do commit"
```

```
git status
git reset --hard HEAD~1 [volta ao estado do penúltimo commit]
```

```
git revert "número do hash"
```

## Desfazendo último commit e push no repositório remoto:

```
git reset --hard HEAD~1
```
```
git push --force
```

## Atualizando repositório local em relação ao remoto:

```
git status 
git pull "nome do remoto" "nome do branch"
```

## Push rejeitado:

```
git push [rejected] -> normalmente o repositório local não está atualizado em relação ao remoto
git pull "nome do remoto" "nome do branch" -> Editor VIM -> ESC :wq ENTER
```

## Sobrescrevendo um histório no Github (Ação destrutiva):

```
git reset --hard "código do commit"
git push -f "nome do remoto" "nome do branch" [-f força a operação]
```

## Apontando o projeto para outro repositório remoto:

```
git remote set-url origin git@github.com:"usuario"/"repositório criado".git
```

## Mesclando branches:

```
git merge "nome-da-branch"
```

## Salvando alterações sem commit:

```
git stash
```

## Listando staches:

```
git stash list
```

## Autor

#### Lucas Araujo

<a href="https://www.linkedin.com/in/lucarauj"><img alt="lucarauj | LinkdeIN" width="40px" src="https://user-images.githubusercontent.com/43545812/144035037-0f415fc7-9f96-4517-a370-ccc6e78a714b.png" /></a>
