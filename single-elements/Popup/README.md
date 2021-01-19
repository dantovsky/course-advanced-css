# Popup (Light Box)

Neste tutorial utilizou-se:
- Popup with only CSS
- How to use the :target pseudo-class
- How to create bxes with equal height using display: table-cell
- How to create CSS text columns
- How to automatically hyphnate words using hyphens

---

# SASS / SCSS Config

https://www.npmjs.com/package/node-sass

## Instalar o SCSS:  
```
npm install node-sass --save-dev
```

## Implementar e compilar SASS localmente

- Criar pasta sass
- Criar arquivo main.scss
- Add o script em package.json:
```
"compile:sass": "node-sass sass/main.scss css/style.css"
```
- Ou, adicionar com a flag "watching" para compilar sempre que houver alteração.
```
"compile:sass": "node-sass sass/main.scss css/style.css -w"
```

**Estrutura do comando node-sass**
```
node-sass <input file> <output file>
```

## Como fazer auto reloading na página quando o arquivo é alterado

### Opção 1

- Pode ser instalado o live-server globalmente
```
sudo npm install live-server -g
```
- Na raiz da app (onde se encontra o package.json), digitar:
```
live-server
```
- Aceder o endereço: http://127.0.0.1:8080

Obs: os dois comandos (auto compiling do SASS e auto reloading com o live-server) precisam ser iniciados em linha de comandos separadas.

### Opção 2

- Utilizar a extensão Live Server do VS Code.
- No ficheiro index.html » botão direito do mouse » Opem witn Live Server
