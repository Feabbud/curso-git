# Git Básico

## Configurando o GIT
- git config --global user.name "nome do usuário"
- git config --global user.email "email do usuário"

## Iniciando o Git
- para iniciar o git usamos na pasta que queremos versionar o git init
- git status: mostra o que foi feito 
- git add . : adiciona todos os arquivos
- git add -A: adiciona todos os aruqivos também
- git add arquivo: adiciona um arquivo especifico.
- git commit -m "mensagem": salvamos a alteração e colocamos uma mensagem. Podemos adicionar os arquivos no commit fazendo -am ao invés de só -m.
- git log: histórico do que foi feito. Mostra uma chave do commit, qual branch que estava, o nome do usuário e a data de alteração.
- git branch: mostra qual a branch que estamos.
- git reset --funcao Hash do commit: volta para o estado desejado que pode ser: --soft, que volta para o commit anterior mas as alterações ficam adicionados. --mixed volta para o commit anterior e temos que dar o commit novamente. --hard que volta para o commit anterior e esquece e apaga tudo que fizemos.

## Branch
- branch são versões diferentes do sistema
  - quando iniciamos o git é criada a branch master