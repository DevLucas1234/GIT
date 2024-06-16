
<img src="https://git-scm.com/images/logos/downloads/Git-Icon-1788C.png" width="100px" height="auto">

# COMANDOS DO #GIT
## GIT - Conceitos Básicos

### Comandos
- definindo o seu nome no terminal e no github:
```bash
git config --global user.name "xxx"
```
- definindo seu email do github:
```bash
git config --global user.email xxxxx@gmail.com
```
- definindo o editor de texto:
```bash
git config --global core.editor "code --wait"
```
> [!NOTE]
> ❗ Lembrando que ``code --wait`` diz ao terminal para esperar fechar a instancia do visual studio code, que será o editor padrão
- configurando erros que pode ocorrer no texto no terminal:
```bash
git config --global core.autocrlt true
```
> [!NOTE]
> ❗ Se estiver no linux mude **true** para **input**
- para ver todas as configurações feitas acima do GIT:
```bash
git config --global -e
```
- iniciando um Repositório GIT:
```bash
git init
```
- adicionando no GIT:
  - ``git add nome.md gui.md``, adicionando arquivos determinados
  - ``git add *.md``, adiciona tudo que estiver na extensão **md**
  - ``git add .``, adiciona tudo (arquivos e pastas)
> [!NOTE]
> Estão na área de STADING prontos para ser commitados (commit)
- para commitar:
```bash
git commit
```
> [!NOTE]
> ❗ Caso remova algum arquivo com comando ``rm``, ele ainda estará no STADING:
```bash
git ls-files
```
- para ignorar arquivos/pastas:
```bash
echo "log/" > .gitignore
```
