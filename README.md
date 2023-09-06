
# DIO | Resumos Git e GitHub

Repositorio para armazenar resumos de códigos do Git e GitHub da [Digital Innovation One (DIO)](https://www.dio.me)

## 📚 Documentação

- [Documentação Git](https://git-scm.com/doc)
- [Documentação GitHub](https://docs.github.com/pt)
- [Documentação do MarkDown](https://docs.github.com/pt/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

## 🌐 Como ativar a chave SSH

1. Abra o Git Bash;

2. Digite o comando `ls -al ~/.ssh` para saber se há chaves SSH existente;
    ```
    id_rsa.pub
    id_ecdsa.pub
    id_ed25519.pub
     ' O nome das chaves publicas compativeis com git geralmente são essas
    ```
3. Digite o comando `ssh-keygen -t ed25519 -C "your_email@example.com"` substituindo pelo seu e-mail do GitHub;

4. Altere o diretório de armazenamento da chave, ou mantenha o padrão e adiciona uma passphrase (senha);

5. Use o comando `eval "$(ssh-agent -s)"` e depois `ssh-add ~/.ssh/id_ed25519`;

6. No site do GitHub, vá até settings na aba **SSH and GPG keys** clique em **New SSH key**;

7. Digite um nome para a Chave que ficará salva no site, e em key coloque o id da chave;

8. Para obter o ID da Chave vá até o diretório que estão armazenadas as chaves, caso esteja no padrão o comando será `cd ~/.ssh` e digite `ls` para listar as chaves presentes

## 💻 Códigos

Abaixo alguns códigos que podem ser úteis na gestão de repositórios

```
$ git init
 ' Inicia um Repositório local
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

## 🔍 Referências
[DIO](https://www.dio.me)


