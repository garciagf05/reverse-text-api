# App para invertir texto _v0.0.1_

Reverse Text App es una aplicación que toma un texto dado y lo invierte, así mismo, también es capaz de determinar si dicho texto es palindromo o no.

## Caracteristicas

- Puede revertir un texto, ejemplo: "Prueba" -> "abeurP".
- Puede determinar si un texto es palindromo, por ejemplo, la palabra "Radar", o la frase "Anita lava la tina".
- Reconoce palabras sin importar el case.

## ¿Como probar?

La aplicación fue realizada en node@12.22.1 y no posee ninguna dependencia al sistema operativo mas que el propio ambiente de Node. Para probar la aplicación se deben ejecutar los siguientes pasos:

1. Abrir la terminal del sistema.
2. Clonar el repositorio desde github a su equipo en el directorio que prefiera con el comando:
```sh
git clone https://github.com/garciagf05/reverse-text-api.git
```

3. Ingresar al proyecto previamente clonado en la terminal.
4. Ejecutar en la raíz del proyecto para descargar los paquetes necesarios el siguiente comando:
```sh
npm install
```
5. Para levantar el aplicativo, ejecutar comando:.
```sh
npm start
```

6. Ahora puede probar en el siguiente endpoint, donde el query **"text"** es el texto a invertir :
```sh
http://localhost:3000/api/iecho?text=example
```

**Notas importantes:**
- Por defecto se estableció el uso del puerto 3000 para levantar la aplicación, si por algún motivo debe cambiar el puerto puede hacerlo en el siguiente fichero: **src/constants/index.js**, en la linea 3.
- Para que una frase u oración sea considerada palindrome, debe poseer la misma acentuación al derecho y al inverso.