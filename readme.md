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
git add .
```
lista as branches
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

Verifica usuario logado no github
```bash
git config --global user.email
```


define o email do usuário
```bash
git config --global user.email "you@example.com"
```
define o email do usuário
```bash
git config --global --unset user.email "you@example.com"
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
Voltar para o commit
```bash
git reset --hard "HEAD@{<numero do commit>}"
```

ou

```bash
git reset --hard <hash>
```

-----//------

criar pag3 e pag4 com branchs diferentes

Clonar projeto
```bash
git clone <endereco do projeto>
```
lista as branches
```bash
git branch
```

cria uma nova branch
```bash
git branch <nome da branch>
```
muda para branch
```bash
git checkout <nome da branch>
```
cria e muda para branch
```bash
git checkout -b <nome da branch>
```
realiza o commit

push na branch
```bash
git push -u origin <nome da branch>
```

fazer merge

remoto precisa criar uma cópia

lista as branches locais e remotas
```bash
git branch -a
```

Caso não tenha as branches locais:
```bash
git branch <nome da branch> origin/<nome da branch>
```

cria e muda para a branch, neste caso para fazer o merge precisa voltar para branch principal
```bash
git checkout -b feature/pag3 origin/<nome da branch>
```
faz o merge para cada branch
```bash
git merge <nome da branch>
```

Faz o push da branch principal atualizada
```bash
git push origin main
```
Para deletar a branch
```bash
git branch -d <nome da branch>
```

Para deletar a branch se ainda não tiver realizado merge
```bash
git branch -D <nome da branch>
```
Para deletar a branch remota
```bash
git push origin --delete <nome da branch>
```


-----//------

criar gitignore

.gitignore
    css e deletar a pasta
    fazer um push
    voltar a pasta e adicionar somente
    style.css

    para remover do cache do projeto projeto
    ```bash
    git rm --cashed <endereço do arquivo>
    ```

    evitar envio de todo arquivo de uma extensão especifica
    *.html

mostrar gitignore.io

criar arquivo

.env

adicionar ao gitignore

Definir um environment no github e uma secret

criar um git actions

