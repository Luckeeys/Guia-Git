# 🌐 Como ativar a chave SSH

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