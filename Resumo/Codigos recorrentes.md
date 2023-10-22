# 💻 Códigos Recorrentes

Abaixo alguns códigos que podem ser úteis na gestão de repositórios

```
$ git init
 ' Inicia um Repositório local
```
```
$ git clone #URL
 ' clona um repositório (apenas a branch principal)
```
```
$ git clone #URL --branch #NomeDaBranch
 ' clona uma branch específica do repositório
```
```
$ git checkout -b #NomeDaBranch
 ' Cria uma branch local
```
```
$ git checkout #NomeDaBranch
 ' Muda para a branch citada
```
```
$ git branch
 ' Lista as branchs do projeto
```
```
$ git branch -d #NomeDaBranch
 ' Deleta uma branch existente
```
```
$ git stash
 ' Coloca uma modificação em stand e retorna a branch para a versão antes das modificações
```
```
$ git stash list
 ' Lista as alterações que estão em espera
```
```
$ git stash apply
 ' Retorna as alterações que estavam em standby
```
```
$ git statsh pop
 ' Remove a alteração que estava em standby
```
```
$ git merge #NomeDaBranch
 ' mescla uma branch com a outra
```
```
$ git add #NomeDoArquivo 
 ' no lugar do Nome do Arquivo coloque "." para adicionar todos os arquivos da arvore
```
```
$ git commit -m "mensagem do commit"
 ' Na mensagem colocar um resumo das alterações feitas
```
```
$ git commit --amend -m ¨mensagem¨
 ' Altera a mensagem do commit localmente, na mensagem colocar um resumo das alterações feitas
```
```
$ git log
 ' loga as ações feitas no comando
```
```
$ git reset --soft #ID do commit
 ' reseta para o commit referenciado mantendo todas as alterações posteriores na árvore de trabalho, para assim apenas corrigir a mensagem do commit 
```
```
$ git reset --mixed #ID do commit
 ' é o reset padrao do git -- reseta para o commit referenciado e limpa a arvore de trabalho, podendo remover arquivos que não serão mais commitados
```
```
$ git reset --hard #ID do commit
 ' reseta para o commit referenciado e deleta os arquivos que foram adicionados nos commits posteriores
```
