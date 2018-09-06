# Git Básico

## Configurando o GIT
- git config --global user.name "nome do usuário"
- git config --global user.email "email do usuário"

## Iniciando com Git
- para iniciar o git usamos na pasta que queremos versionar o git init
- git status: mostra o que foi feito. 
- git add . : adiciona todos os arquivos.
- git add -A: adiciona todos os arquivos também.
- git add arquivo: adiciona um arquivo especifico.
- git commit -m "mensagem": salvamos a alteração e colocamos uma mensagem. Podemos adicionar os arquivos no commit fazendo -am ao invés de só -m.
- git log: histórico do que foi feito. Mostra uma chave do commit, qual branch que estava, o nome do usuário e a data de alteração.
- git diff: mostra as alterações do documento. --name-only: mostra quais arquivos foram alterados. nomeDoArquivo: mostra somente o arquivo que você passou o nome.

## Branchs
- git branch: mostra qual a branch que estamos.
- git branch nomeDaBranch: cria uma branch nova.
- git branch -D branchLocal: deleta a branch passada no repositorio local.
- git checkout nomeDaBranch: muda para a branch escrita.

## Revertendo ações
- git checkout: muda branch e commits. HEAD -- arquivo.
- git reset --funcao HashDoCommit: volta para o estado desejado que pode ser: 
  - --soft, que volta para o commit anterior mas as alterações ficam adicionados. 
  - --mixed volta para o commit anterior e temos que dar o commit novamente. 
  - --hard que volta para o commit anterior e esquece e apaga tudo que fizemos.
- git revert HashDoCommit: faz um commit reverso do commit passado. Se o commit adicionou uma linha, ele apaga. Adicionou um arquivo, ele deleta.

## Conexão com o Github
- No repositório que queremos enviar para o github  fizemos: git remote add origin linkRepositorioGitHub. 
- git push -u origin master - envia as alterações do repositorio local para o repositorio remoto, que seria o github.
- git fetch origin - pega todos os dados do repositório remoto que ainda não temos no nosso local mas não faz o merge.
- git pull origin master: atualiza o repositório local com as modificações do repositório remoto e ja faz o merge automaticamente.
- git push origin :branchRemoto: deleta a branch passada no repositorio remoto.
- git remote -v: exibe os repositorios remotos e mostra sua URL..
- git remote show nomeDoRemote: Lista informações completas do repositório remoto.

## Ignorando arquivos para o repositório remoto
 - criamos o arquivo .gitignore
 - colocamos nesse arquivo o que não queremos enviar para o repositório remoto que pode ser:
  - arquivos
  - *.extensão
  - pastas/*.extensão
  - pasta/
