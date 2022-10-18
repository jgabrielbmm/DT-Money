## DT Money
**DT Money** é uma aplicação de gestão financeira feita em **ReactJS** e **TypeScript** , alêm disso foi usado o **json-server** para simular um API do back-end. Nesta aplicação você pode cadastrar novas entradas e saídas especificando uma descrição, preço, categoria e tipo.

### Instalação e Inicialização da Aplicação

Instalar dependências:
```js
npm install
```

Após instalar as dependências deve-se inicializar a API, que está rodando na porta 3333 e com delay de 500ms
```js
npx dev:server
```
Caso queira mudar a porta ou o delay vá em **package.json** -> **script** -> **dev:server**
```yaml
  "scripts": {
    "dev": "vite",
    "build": "tsc && vite build",
    "preview": "vite preview",
    "dev:server": "json-server server.json -p 3333 -w -d 500",
    "lint": "eslint src --ext .ts,.tsx"
  }
```
Inicializar a aplicação:
```js
npm run dev
```
O projeto está rodando da porta 3000, caso você esteja com outra aplicação rodando nessa porta você pode trocar ela indo em **vite.config.ts** e alterar a port.
```js
export default defineConfig({
  plugins: [react()],
  server: {
    port: 3000,
  },
})
```

### Funcionalidades
* Listagem dos Income e Outcome
* Filtragem
* Sumário

### Conceitos usados no desenvolvimento 
* Estados
* ContextAPI
* Consumo de API
* Imutabilidade do estado 
* Lista e chaves no React JS
* Propriedades
* Componentização
* Styled-components