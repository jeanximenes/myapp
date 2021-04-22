# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Projeto criado para exemplificar a publicação utilizando o gh-pages

Passo a passo para publicação, seguindo a fonte mencionada na descrição deste projeto:

### Passos para publicar no gitHub:

- npm init react-app <nome-projeto>
- cd <nome-projeto>
- npm install gh-pages --save-dev
- edite o package.json da app para incluir:
   - "homepage": "https://jeanximenes.github.io/app", e
   - "scripts": {
	"predeploy": "npm run build",
	"deploy": "gh-pages -d build", ...
- crie um novo repositorio no github, p.e.: no browser entre na url "github/new"
- na página seguinte do github, siga os passos "..or push an existing from the command line", no caso deste passo a passo:
   - git remote add origin https://github.com/jeanximenes/app.git
   - git branch -M main
   - git push -u origin main
- npm run deploy
