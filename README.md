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
O main é o branch principal do GIT

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


Voltar para o branch principal (main)
```bash
git checkout main
```


Resolver merge entre os branches
```bash
git merge devsleonardo
```

Removendo uma branch local
```bash
git branch -d devsleonardo
```
Caso você receba o seguinte erro:

>error: The branch 'teste' is not fully merged.

Isso significa que você possui algum commit recente nesta branch, e excluí-la significaria perder este commit

Caso queira salvar algum commit, faça um merge com outra branch. Caso contrário, faça um force delete com o parâmetro -D
```bash
git branch -D devsleonardo
```

Removendo uma branch remota
```bash
git push origin --delete devsleonardo
```
ou
```bash
git push origin :devsleonardo
```
