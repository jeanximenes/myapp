# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Projeto criado para exemplificar a publicação utilizando o gh-pages

Passo a passo para publicação, seguindo a fonte mencionada na descrição deste projeto:

### Passos para publicar no gitHub:

1 npm init react-app <nome-projeto>
2 cd <nome-projeto>
3 npm install gh-pages --save-dev
4 edite o package.json da app para incluir:
   - "homepage": "https://jeanximenes.github.io/app", e
   - "scripts": {
	"predeploy": "npm run build",
	"deploy": "gh-pages -d build", ...
5 crie um novo repositorio no github, p.e.: no browser entre na url "github/new"
6 na página seguinte do github, siga os passos "..or push an existing from the command line", no caso deste passo a passo:
   - git remote add origin https://github.com/jeanximenes/app.git
   - git branch -M main
   - git push -u origin main
7 npm run deploy
