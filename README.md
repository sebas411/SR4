# SR4
Instrucciones:
- Clonar el proyecto
- Abrir una ventana de terminal en el directorio raiz del proyecto
- Utilizar el siguiente comando: "make && ./gl"
    (Esto compilara el programa y lo ejecutará)
Luego de seguir estos pasos el programa automáticamente generará una imagen bmp llamada image.bmp con el objeto renderizado y también otra llamada zbuffer.bmp que es el buffer de z renderizado.

Si se quieren probar los distintos features se debe tomar en cuenta lo siguiente:
* Para cargar un objeto se utiliza la funcion glLoad(filename, tx, ty, sx, sy)
* Para renderizar la imagen se utiliza glFinish()
* Para renderizar el zBuffer se utiliza glZrender()  
Es importante utilizar glZrender() despues de glFinish() ya que modifica el framebuffer y de ser ejecutados al revés glFinish() renderizaría el zBuffer también.

Nota: Se necesita el compilador g++ para utilizar el programa.
