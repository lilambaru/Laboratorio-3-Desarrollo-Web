
Después de la estructura del proyecto, agrega esto:

```markdown
## Funcionamiento del Sistema

El sistema permite registrar la información de un aspirante mediante un formulario ubicado en `index.php`.

Los datos son enviados utilizando el método POST hacia el archivo `procesar.php`, donde se realizan las validaciones correspondientes antes de procesar y mostrar la información.

El formulario también permite subir una fotografía del aspirante mediante el atributo `multipart/form-data`.

---

## Validaciones realizadas

Durante el procesamiento de los datos se implementaron diferentes validaciones para garantizar el correcto funcionamiento del sistema.

- Validación de campos obligatorios.
- Validación de datos desde el servidor utilizando PHP.
- Uso de `htmlspecialchars()` para evitar la interpretación de código HTML ingresado por el usuario.
- Validación de la fotografía subida por el aspirante.
- Validación de extensiones de imagen permitidas como JPEG, PNG y GIF.
- Almacenamiento de las fotografías en la carpeta `uploaded_files`.
- Normalización y procesamiento de los datos antes de mostrarlos.

---

## Organización mediante Includes

Para evitar repetir código y mantener una estructura más organizada, se utilizaron archivos PHP externos mediante `include`.

El archivo `header.php` contiene la parte superior de la página y la navegación del sistema.

El archivo `footer.php` contiene el pie de página.

Estos archivos pueden reutilizarse en diferentes páginas del proyecto, facilitando el mantenimiento del código.

---

## Seguridad

Se aplicaron medidas básicas de seguridad durante el procesamiento de la información.

La función `htmlspecialchars()` permite convertir caracteres especiales en entidades HTML, evitando que código introducido en el formulario sea interpretado directamente por el navegador.

También se realizó una validación del tipo de archivo permitido antes de almacenar las fotografías en el servidor.

---

## Conclusión

El desarrollo de este laboratorio permitió aplicar conocimientos de HTML5, Bootstrap y PHP para construir una aplicación web capaz de recibir y procesar información.

Además, se trabajó con formularios, validaciones del lado del servidor, carga de archivos, organización mediante carpetas e includes y medidas básicas de seguridad.

Finalmente, el proyecto fue organizado y almacenado en un repositorio de GitHub, permitiendo mantener el código fuente documentado y accesible.
