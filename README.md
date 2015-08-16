# Portada para documentos de la URL para LaTeX

Esta es una plantilla básica para crear portadas para documentos de la Universidad Rafael Landivar.

La plantilla no es oficial, es simplemente una propuesta de cómo se debería de entregar los documentos.

## Inicio rápido

* [Descarga][descarga-plantilla] y extrae la plantilla o bien usa git, ya sea clonando o realizando un fork del repositorio en la carpeta del proyecto de LaTeX.
* Al documento principal de LaTeX se debe agregar los siguientes comandos, con los valores correspondientes para su uso.
  ```latex
  \newcommand{\HBar}{\rule{\linewidth}{0.5mm}}
  \newcommand{\logoURL}{logoURL}
  \newcommand{\nAutor}{Nombre del autor}
  \newcommand{\nCurso}{Curso}
  \newcommand{\cTituloA}{Titulo 1}
  \newcommand{\cTituloB}{Titulo 2}
  \newcommand{\cFecha}{Agosto de 2,014.}
  ```
  En caso de no necesitar algun comando, el contenido debe quedar en blanco:
  ```latex
  \newcommand{\cTituloB}{}
  ```
  
* Agregue al documento principal la plantilla luego del inicio del documento.
  ```latex
  \begin{document}

  \input{portada/Portada.tex}
  ```

## Licencia
[![Creative Commons License][license-image]][license]

Esta plantilla esta bajo una licencia [Creative Commons Attribution-ShareAlike 4.0 International License][license], eso significa que:


Usted es libre para:

* Compartir — copiar y redistribuir el material en cualquier medio o formato
* Adaptar — remezclar, transformar y crear a partir del material

Para cualquier propósito, incluso comercialmente

El licenciante no puede revocar estas libertades en tanto usted siga los términos de la licencia

La licencia aplica solamente a la plantilla y no a los documentos que se generen con ella.

### Logotipo de la Universidad Rafael Landivar
El logotipo de la Universidad Rafael Landivar es propiedad de la [Universidad Rafael Landivar][url-page] y solo se distribuye en éste documento para su fácil uso.

## Hacks

### Cambiando el Logotipo

La plantilla cuenta con un logotipo base, pero se puede cambiar por cualquier otro, para realizarlo se debe seguir éstos pasos:

* El logotipo se debe [descargar][descarga-logo] de la página urlmedia de la URL.
* El nuevo logotipo debe ser colocado en la misma carpeta donde se encuentra la plantilla.
* Se debe cambiar el valor del comando **logoURL** en **\\newcommand{\\logoURL}{nombreDeArchivo}** por el nombre de la imagen, no es necesario agregarle la extensión.

[descarga-plantilla]: https://https://github.com/dhabyx/latex-url-portada/archive/master.zip
[descarga-logo]: http://urlmedia.url.edu.gt/Pages/Busqueda.aspx?filtro=&b=logo
[license-image]: https://i.creativecommons.org/l/by-sa/4.0/88x31.png
[license]: https://creativecommons.org/licenses/by-sa/4.0/
[url-page]: http://www.url.edu.gt
