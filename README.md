# Git Básico

## Configurando o GIT
- git config --global user.name "nome do usuário"
- git config --global user.email "email do usuário"

## Iniciando o Git
- para iniciar o git usamos na pasta que queremos versionar o git init
- git status: mostra o que foi feito 
- git add . : adiciona todos os arquivos
- git add -A: adiciona todos os arquivos também
- git add arquivo: adiciona um arquivo especifico.
- git commit -m "mensagem": salvamos a alteração e colocamos uma mensagem. Podemos adicionar os arquivos no commit fazendo -am ao invés de só -m.
- git log: histórico do que foi feito. Mostra uma chave do commit, qual branch que estava, o nome do usuário e a data de alteração.
- git branch: mostra qual a branch que estamos.
- git branch nomeDaBranch: cria uma branch nova.
- git checkout nomeDaBranch: muda para a branch escrita
- git checkout: muda branch e commits. HEAD -- arquivo
- git reset --funcao Hash do commit: volta para o estado desejado que pode ser: 
  - --soft, que volta para o commit anterior mas as alterações ficam adicionados. 
  - --mixed volta para o commit anterior e temos que dar o commit novamente. 
  - --hard que volta para o commit anterior e esquece e apaga tudo que fizemos.
- git diff: mostra as alterações do documento. --name-only: mostra quais arquivos foram alterados. nomeDoArquivo: mostra somente o arquivo que você passou o nome.

## Conexão com o Github
- No repositório que queremos enviar para o github  fizemos: git remote add origin linkRepositorioGitHub. 
- git push -u origin master - envia as alterações para o github, que seria origin, da branch master que está no meu computador.
- git fetch -u origin master - recupera as alterações ou arquivos que estão no repositório remoto.