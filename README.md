# Boilerplate FiveM React & Tailwind (Javascript)

Template de React.JS e Tailwind para criação de resources para FiveM

## Configuração

A configuração é simples, para funcionar apenas altere resName em `config/config.js` para funcionar perfeitamente

## Custom Hooks

### useFetch
Utilização:
```javascript
// callbackName é o callback que vai ser chamado no client-side
// payload pode ser qualquer informação enviada para o client-side, pode ser um objeto, uma array, uma string, qualquer valor
useFetch("callbackName", payload);

useFetch("callbackName", payload).then(response => console.log(response));
```
```lua
RegisterNUICallback("callbackName", function(payload)
  print("Recebido: "..json.encode(payload))
end)

RegisterNUICallback("callbackName", function(payload, response)
  print("Recebido: "..json.encode(payload))
  response("Retornado")
end)
```

## Instalação

Faça a instalação do repositório, abra o Prompt de Comando no caminho do arquivo
Comandos de execução:

### NPM
```sh
npm install
npm run dev
```

### YARN
```sh
yarn
yarn dev
```

## Suporte
Entre em [contato](https://github.com/marquezzx) comigo para obter suporte.
