# mytailwindcss

mytailwindcss

### Install Tailwind CSS

Install tailwindcss via npm, and create your tailwind.config.js file.

```sh
$ npm install -D tailwindcss
$ npx tailwindcss init # ou npx tailwindcss init --full
```

### Add the Tailwind directives to your CSS

Add the @tailwind directives for each of Tailwind’s layers to your main CSS file.

crie um diretório com o nome de _src_ e adicione o arquivo **input.css** nele com o seguinte conteúdo

```javascript
@tailwind base;
@tailwind components;
@tailwind utilities;

```

### Start the Tailwind CLI build process

Run the CLI tool to scan your template files for classes and build your CSS.

```sh
$ npx tailwindcss -i ./src/input.css -o ./src/output.css --watch

```

### Crie um exemplo

Crie um arquivo src/index.html com o seguinte conteúdo.

```html
<!DOCTYPE html>
<html lang="pt-br">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link href="./output.css" rel="stylesheet" />
  </head>
  <body>
    <h1 class="text-3xl font-bold underline">Hello world!</h1>
  </body>
</html>
```
