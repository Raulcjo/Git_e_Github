# Anotações sobre git e github

## gitignore

### Com apenas o nome será ignorado somente esse arquivo
- db.sqlite3

### Com 1 asterísco qualquer arquivo com sqlite3 será ignorado
- *.sqlite3

### Com 2 asteriscos ele procura em diretórios e em subdiretórios
- **arquivos

## Comandos git

- Sempre que criar um repositório tem que colocar nome e email.

- git init - Inicia o git

- git config user.name = "Geek University" - local (compartilhado)
- git config user.email = "contato@geekuniversity.com.br"
- git config --global user.email "contato@geekuniversity.com.br" - configuração global (privado)
- git config core.pager cat - Volta ao comportamento que o terminal fazia

- git add nome_arquivo - adiciona ao monitoramento do git e também atualiza o arquivo
- git add . - Adiciona todos os arquivos

- git log - Mostra o histórico de commits
- git log --oneline - Traz o resumo em uma linha dos commits
- git log -n1 - Traz apenas 1 commit
- git log --oneline -n1 - É possível misturar os dois

- git log --before="ano-mês-dia" - Devolve todos os commits antes da data específicada
- git log --after="ano-mês-dia" - Devolve todos os commits depois da data específicada
- git log --since="data" - Devolve todos os logs desde da data específicada

- git log author="Geek" - Devolve todos os commits com autor pedido

- git help log - Aparece todas as possibilidades de log
- git checkout "numero de id do commit" - Volta para quando o commit foi feito (Visualização)
- git checkout "nome_do_arquivo" - Retorna página para a formatação do último commit

- git mv 'arquivo1' 'arquivo1_renomeado' - Renomear arquivos através do git
- Caso renomear o arquivo fora do git, o git entenderá que o arquivo original foi deletado, 
será necessário adicionar o novo arquivo, informar que o status do anterior e fazer um commit 
informando que foi trocado.

- git rm 'nome_arquivo' - remove um arquivo através do git
- Mesmo processo do mv

- git diff --staged - Compara as alterações com o último commit realizado
- git commit --amend -m "Nome_do_commit" - Adiciona alterações no último commit
- git restore --staged 'nome_do_arquivo' - retira o arquivo do monitorameto do git
- git reset HEAD --hard - Volta os arquivos para o estado do último commit


