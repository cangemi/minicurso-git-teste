# Mini curso Git GitHub

Descrição  do projeto.

## Tecnologias

- HTML
- CSS

## Roteiro

Verifica se o Git está instalado e a versão.
```bash
git -v
```
Inicializa um repositório Git na pasta atual
```bash
git init
```
Adiciona todos os arquivos
```bash
git add -A
```
ou
```bash
git add .
```
Verifica a branch atual
```bash
git branch
```

Modifica o nome da branch
```bash
git branch -M <novo nome>
```
Adicionar repositório remoto
```bash
git remote add origin <endereco do repositorio>
```

Faz um commit com uma mensagem descritiva sobre as alterações realizadas
```bash
git commit -m "descricao do commit"
```

Envia os arquivos para o repositório e configura o push para origem e branch main
```bash
git push -U origin main
```

Uma vez configurado basta somente usar o:
```bash
git push
```
-----//------

Criar pag2.html e o readme.md

Adiciona todos os arquivos
```bash
git add .
```
para saber o status dos arquivos
```bash
git status
```

Faz um commit com uma mensagem descritiva sobre as alterações realizadas
```bash
git commit -m "descricao do commit"
```
Envia os arquivos para o repositório
```bash
git push
```

-----//------

Deletar style.css e recuperar

Ver o histórico
```bash
git reflog
```
Voltar e apagar tudo que veio depois
```bash
git reset --hard "HEAD@{<numero do commit>}"
```

ou

```bash
git reset --hard <hash>
```
só voltar o commit mas manter os arquivos intactos não recupera arquivos
```bash
git reset --soft "HEAD@{<numero do commit>}"
```