# Git Intermediário:

## Branch:

Uma branch nada mais é do que uma ramificação do projeto

branch master -> ramo principal

               Base                                       -----> branch funcionalidadeB
início --------\-----------------------------------------/-----> projeto final
                -----> branch funcionalidadeA            Base

> OBS: O git é um repositório descentralizado

> q - saí da fizualização dos commits 
> ls - mostra os arquivos e diretórios existentes
> ls -la - mostra todos os arquivos e diretórios inclusive os ocultos
> touch 'nome_arquivo' - cria um novo arquivo no diretório

> git branch - Mostra em qual ramificação está sendo trabalhada
> git branch 'nome_da_branch' - Cria uma nova ramificação
> git checkout 'nome_da_branch' - Troca para a ramificação especificada

> Obs: Aquilo que acontece em uma branch precisa ser comitado e não vai aparecer nas outras branchs quando trocar,
a não ser que tenham herdado ou seja trazido para elas.

> git branch -d 'nome_do_arquivo' - Deleta a branch, mas antes confere se tudo que existe na branch que será deletada existe na principal e caso tenha algo diferente pede para digitar git branch -D 'nome_do_arquivo' para ter certeza que deseja deletar.
> git branch -D 'nome_do_arquivo' - Deleta a branch de qualquer maneira

> git merge 'nome_branch' - Mistura a branch especificada com a branch que está sendo usada, mas não deleta a branch especificada apenas mistura o conteúdo das duas.

> git checkout -b 'nome-brach' - Cria uma nova branch e troca direto par ela

> git rebase 'nome_branch' - Altera a base da ramificação do commit para outra
> git rebase - Reorganiza os arquivos e reaplica os commits

> git push - Faz com que o repositório original receba as mudanças feitas no repositório clonado, pois os publica enão funciona sem o bare repository
> git fetch - Baixa os arquivos sem realizar o merge

> git pull - Faz o processo de git fetch + git rebase de uma vez e também abre um editor de texto na qual se pode fazer algumas ações extras