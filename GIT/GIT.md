# GIT
## 1. Introdução ao Git
### O que é GIT?
Git é um sistema de controle de versçao distribuído, em termos simples, o git é uma ferramenta que ajuda você a acompanhar as alterações nno seu código ao longo do tempo.

## 2. Configuração Inical do Git
Depois de instalar o Git, você precisa condigurá-lo com suas informalçies pessiaus. Isso é importantge para que os commits que você fizer sejam corretamente atribuídos a você.
### Configurar Nome de Usuário e Email
Execute os seguintes comandos no terminal (ou Git Bast, se estiver no Windows):
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@example.com"
```
Isso configura seu nome de usuário e email globalmente, ou seja, para todos os repositórios que você criar ou clonar.
### Configurando Editor Padrão
O Git usa um editor de texto para algumas operações, como editar mensagens de commit. você pode configurar seu editor preferido com:
- **VS Code**:
```bash
git config --global core.editor "code --wait"
# '--wait' faz com que o terminal espere você fechar o editor, depois de fechado a execução volta normalmente
```
- **Vim**:
```bash
git config --global core.editor "vim"
```
- **Nano**:
```bash
git config --global core.editor "nano"
```
## 3. Comandos Básicos do Git
### Inicialização de um Repositório (``git init``)
O comando ``git init`` é usado para criar um novo repositório Git. Quando você executa esse comando, ele inicializa um repositório vazio no diretório atual, criando um subdiretório ``.git`` que contém todos os arquivos necessários do repositório.
```bash
git init
```
**Exemplo**:
```bash
mkdir meu-projeto # cria uma pasta vazia
cd meu-projeto # entra na pasta
git init
```
### Clonagem de Repositórios (``git clone``)
O comando ``git clone`` cria uma cópia local de um repositório remoto. É muito usado para começar a trabalhar em um projeto existente.
```bash
git clone <url-do-repositorio>
```
### Status do Repositório (``git status``)
O comando ``git status`` mostra o estado atual do diretório de trabalho e da staging area. Ele informa quais arquivos foram modificados, quais estão prontos para serem commitados e quais não estão sendo rastreados pelo Git.
```bash
git status
```
### Adição de Arquivos (``git add``)
O comando ``git add`` adiciona mudanças do diretório de trabalho à staging area. Isso permite que você prepare suas alterações para serem commitadas. Você pode adicionar arquivos individuais, múltiplos arquivos ou todos de uma vez.
```bash
git add <nome-do-arquivo>
git add . # inseri tudo (tenha cuidado)
```
**Exemplo**:
```bash
git add meu-arquivo.txt
git add .
```
### Commit de Alterações (``git commit``)
O comando ``git commit`` grava as alterações da staging area no repositório. Cada commit deve ter uma mensagem descritiva que explique as alterações feitas.
```bash
git commit -m "Mensagem"
```
**Exemplo**:
```bash
git commit -m "Meu primeiro commit"
```
### Visualização de Histórico (``git log``)
O comando ``git log`` mostra o histórico de commits do repositório. Ele exibber uma lista de commits em ordem cronológica inversa, começando pelo commit mais recente.
```bash
git log
```
**Exemplo**:
```bash
git log --oneline --graph --all
```