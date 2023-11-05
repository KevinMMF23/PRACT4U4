# Práctica 4: Formularios y Flask

## Descripción

Este repositorio corresponde a la Práctica 4 de Formularios y Flask. Aquí se presenta el proyecto desarrollado utilizando las siguientes herramientas:

- **Herramientas utilizadas:**
  - Visual Studio Code: Editor de código.
  - HTML: Lenguaje de marcado para estructurar el contenido web.
  - CSS: Lenguaje de estilo para diseñar la apariencia de las páginas web.
  - Python: Lenguaje de programación utilizado con el framework Flask para la creación del servidor web.

## Estructura del Proyecto

- `practica_4/`
  - `app/`
    - `static/`
      - `css/`
        - (archivos CSS)
      - `imgs/`
        - (archivos de imágenes)
    - `templates/`
      - `public/`
        - (archivos HTML)
  - `venv/`
    - (entorno virtual de Python)
  - `.gitignore`
  - `README.md`

## Marco Teórico

### Flask

Flask es un framework de desarrollo web escrito en Python. Es ligero y flexible, lo que lo convierte en una excelente elección para crear aplicaciones web. Flask se basa en el concepto de rutas, vistas y plantillas, lo que permite construir páginas web dinámicas de manera eficiente.

### HTML y CSS

HTML (HyperText Markup Language) se utiliza para estructurar el contenido de las páginas web. Define los elementos y su jerarquía en el documento.

CSS (Cascading Style Sheets) se utiliza para dar estilo y diseño a las páginas web. Permite controlar la apariencia de los elementos HTML, como colores, fuentes, tamaños, márgenes y más.

## Pasos Seguidos

### Paso 1: Crear una estructura

Se creó la estructura del proyecto, organizando archivos y carpetas de manera que los recursos estén separados adecuadamente.

### Paso 2: Instalar entorno virtual y Flask

Se estableció un entorno virtual y se instaló Flask para la creación del servidor web.

### Paso 3: Creación de páginas web

Se configuraron las páginas web utilizando HTML y CSS, asegurando que los recursos se encuentren en las carpetas correspondientes. Se utilizaron rutas relativas para acceder a los recursos.

### Paso 4: Creación de rutas

Se implementaron rutas utilizando Flask para cada página del proyecto. Estas rutas permiten a los usuarios acceder a las páginas web.

### Paso 5: Vincular enlaces de las páginas con las rutas

Se actualizaron los enlaces en las páginas HTML para que utilicen `url_for` y apunten a las rutas definidas en Flask.

## Resultados de la Tarea

Se logró implementar el proyecto de Práctica 4 de Formularios y Flask con éxito. El repositorio contiene los archivos y carpetas necesarios, así como una estructura organizada. Las páginas web se han configurado y vinculado correctamente a través de las rutas definidas en Flask.

## Ejemplo de Código

A continuación, se presenta un fragmento de código que demuestra cómo se definen las rutas en Flask para este proyecto. Este código se encuentra en el archivo `app.py`:

```python
from flask import Flask, render_template

app = Flask(__name__)

@app.route("/")
def inicio():
    return render_template("public/index.html")

@app.route("/pagina1")
def pagina1():
    return render_template("public/pagina1.html")

@app.route("/pagina2")
def pagina2():
    return render_template("public/pagina2.html")

# Agrega más rutas según sea necesario
```
