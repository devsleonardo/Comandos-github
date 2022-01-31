⚠ | Não é um projeto completo de comandos git somente alguns mais usados no GitHub***

## ...git ajuda

```bash
git help
git help add
git help commit
git help <qualquer_comando_git> 
```

## ... configurando Ambiente
 ```bash
git config --global user.name "nomeGithub"
git config --global user.email "emailGithub
```

## ... criar um novo repositório na linha de comando

```bash
git init
git status
git add .
git commit -m "Nome do commit "
git branch -M main
git remote add origin https://github.com/devsleonardo/devsleonardo.git
git push -u origin main
```
Os repositórios podem ser colocados individualmente da seguinte forma

```bash
Adicionar um arquivo em específico:    git add meu_arquivo.txt
Adicionar um diretório em específico:  git add meu_diretorio
```

## ... remover arquivo/diretório

```bash
git rm meu_arquivo.txt
git rm -r diretorio
```

## ... repositório remoto

Exibir os repositórios remotos
```bash
git remote
git remote -v
```
Vincular repositório local com um repositório remoto
```bash
git remote add origin https://github.com/devsleonardo/devsleonardo.git
```
Exibir informações dos repositórios remotos
```bash
git remote show origin
```

Renomear um repositório remoto
```bash
git remote rename origin listaComandosGit
```

Desvincular um repositório remoto
```bash
git remote rm listaComandosGit
```

Enviar arquivos/diretórios para o repositório remoto
```bash
git push -u origin master
```

Os demais pushes não precisam dessa informação
```bash
git push
```

Atualizar repositório local de acordo com o repositório remoto
```bash
git pull
```

Buscar as alterações, mas não aplica-las no branch atual
```bash
git fetch
```

Clonar um repositório remoto já existente
```bash
git clone https://github.com/devsleonardo/devsleonardo.git
```


## ... branches
O master é o branch principal do GIT

Criando um novo branch
```bash
git branch devsleonardo
```

Trocando para um branch existente
```bash
git checkout devsleonardo
```

>Neste caso, o ponteiro principal HEAD esta apontando para o branch chamado devsleonardo

Criar um novo branch e trocar
```bash
git checkout -b devsleonardo
```

Enviar o branch atual e definir o remoto como upstream
```bash
 git push --set-upstream origin devsleonardo
```


Voltar para o branch principal (master)
```bash
git checkout master
```


Resolver merge entre os branches
```bash
git merge devsleonardo
```

## ... stash

Para alternar entre um branch e outro é necessário fazer o commit das alterações atuais para depois trocar para um outro branch. Se existir a necessidade de realizar a troca sem fazer o commit é possível criar um stash. O Stash como se fosse um branch temporário que contem apenas as alterações ainda não commitadas.

Criar um stash
```bash
git stash
```


Listar stashes
```bash
git stash list
```


Voltar para o último stash
```bash
git stash apply
```


Voltar para um stash específico
```bash
git stash apply stash@{2}
```
>Onde 2 é o indíce do stash desejado


Criar um branch a partir de um stash
```bash
git stash branch meu_branch
```
