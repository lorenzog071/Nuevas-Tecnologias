# Tutorial Tailwind CSS

Tailwind CSS es un Framework de CSS que principalmente brinda clases para el desarrollo web. Cuenta con un conjuto de clases que nosotros podemos usar y editar para la personalizacion de una pagina web.

## Instalacion 
Hay dos tipos de instalacion, nosotros usaremos la mas compleja ya que esta nos permite sacarle mas provecho a tailwind.

Antes de arrancar tenemos que tener instalado Node.js: https://nodejs.org/es/

Creamos ```package.json```
<pre>
npm init -y
</pre>

Instalamos Tailwind
<pre>
npm i tailwindcss
</pre>

### Crear archivos
Crear un directorio ```public/index.html```

Crear un directorio ```src/estilos.css``` y le agregamos lo siguiente:
<pre>
@tailwind base;
@tailwind components;
@tailwind utilities;
</pre>

### Compilar
<pre>
npx tailwindcss build src/estilos.css -o public/output.css
</pre>

Llamar al archivo creado <pre> href="output.css" </pre>

### Personalizar
Creamos el archivo <pre> npx tailwindcss init </pre>

Una vez creado el archivo nos aparecera lo siguente y aqui ya podemos empezar a crear nuestras propias clases
<pre>
module.exports = {
  purge: [],
  theme: {
    extend: {},
  },
  variants: {},
  plugins: [],
}
</pre>

## Ejemplo 
Archivo ```tailwind.config.js ```
<pre>
module.exports = {
  future: {

  },
  purge: [],
  theme: {
    fontFamily:{
      play: ['Playfair Display'],
      secular: ['Secular One'],
      pedana: ['Peddana']
    },
    extend: {
      colors:{
        celeste: '#132743',
        rojo:'#931a25'
      }
    },
  },
  variants: {},
  plugins: [],
}
</pre>
