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
git remote add origin https://github.com/cod3rleo/cod3rleo.git
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
git remote add origin https://github.com/cod3rleo/cod3rleo.git
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
git clone https://github.com/cod3rleo/cod3rleo.git
```
