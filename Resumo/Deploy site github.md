# 🌐 Criando um deploy para o Git Pages no Angular

1. Adicionar o comando abaixo no arquivo package.json
2. Criar uma branch pro deploy
3. E depois executa-lo com o npm run
4. Ele criará uma pasta chamada docs com o projeto
5. comitar as mudanças pro repositorio no GitHub
5. Depois acessar as configurações do GitHub Pages e apontar para o repositorio de deploy e a pasta docs.

```
ng build --configuration=production --output-path docs --base-href /NomeDoRepositorio/"
```