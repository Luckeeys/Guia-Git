# 🌐 Criando um deploy para o Git Pages no Angular

1. Adicionar o comando abaixo no arquivo package.json
2. Criar uma branch pro deploy
3. E depois executa-lo com o npm run
4. Ele criará uma pasta chamada docs com o projeto esse index.html estará apontando para a extensão da url do projeto
5. Criar uma copia do index.html da pasta docs e renomeá-lo para 404.html isso fara com que em caso de atualização da pagina esse arquivo seja carregado, mantendo a navegação do site 
6. Commitar as mudanças pro repositorio no GitHub
5. Depois acessar as configurações do GitHub Pages e apontar para o repositorio de deploy e a pasta docs.

```
ng build --configuration=production --output-path docs --base-href /NomeDoRepositorio/"
```
