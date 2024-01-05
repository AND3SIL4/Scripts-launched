[Documentación archivo scraping](#documentación-del-ejecutable-para-extraer-datos)

[Documentación arhivo organizador](#documentación-del-script-de-organización-de-carpetas)

## Documentación del Ejecutable para extraer datos

## Introducción

Este ejecutable automatiza tareas utilizando Selenium para interactuar con una aplicación web. El script ha sido convertido en un archivo ejecutable, eliminando la necesidad de una instalación de Python.

## Requisitos

- Sistema Operativo: Windows
- No se requiere una instalación adicional de Python.

## Uso

1. **Descargar el Ejecutable:**
   - Descargar el archivo ejecutable (`scraping.exe`).

2. **Ejecutar el Ejecutable:**
   - Hacer doble clic en el archivo ejecutable para ejecutarlo.
   - Si se solicita por el sistema operativo o el software antivirus, permitir la ejecución.

3. **Configurar Ajustes (Opcional):**
   - Si se requiere personalización, editar la configuración dentro del script o en el archivo de configuración asociado.

4. **Revisar Resultados:**
   - El script realizará tareas automatizadas en la aplicación web especificada.
   - Verificar la consola o los archivos generados para obtener información relevante.

## Configuración

- **Configuración del Navegador:**
  - Asegurarse de tener el controlador de Chrome (`chromedriver`) instalado y configurado en el PATH del sistema.

- **Configuración del Script:**
  - Si es necesario, puede personalizar la URL de inicio de sesión, nombre de usuario, contraseña y otras configuraciones dentro del script o archivo de configuración asociado.

## Errores Comunes y Solución de Problemas

- **Archivo No Encontrado:**
  - Si se encuentra un error de "Archivo No Encontrado", asegurarse de que todos los archivos necesarios, incluido el ejecutable y cualquier controlador necesario, estén presentes.

- **Error de Permiso:**
  - Si los permisos impiden escribir en ciertos archivos o directorios, ejecutar el ejecutable como administrador.

- **Error del Navegador:**
  - Si hay un problema al iniciar el navegador, verificar el entorno del ejecutable y asegurarse de que cualquier dependencia requerida esté disponible.

## Resultados Exportados

- Los datos extraídos durante la ejecución del script pueden guardarse en archivos o mostrarse en la consola.

## Tiempo de Ejecución

- El script mostrará el tiempo total de ejecución al finalizar.

## Documentación del Script de Organización de Carpetas

## Introducción

Este script en Python está diseñado para organizar archivos en una carpeta especificada según sus extensiones de archivo. Categoriza los archivos en diferentes carpetas según reglas predefinidas, facilitando la gestión y ubicación de archivos.

## Requisitos para uso

- Sistema operativo Windows

## Requisitos para modificación

- Python 3.12
- Módulos `os` y `shutil`

## Uso usuarios

1. **Descargar el Script:**
   - [Descargue el script (`organizador.exe`)](https://github.com/AND3SIL4/Scripts-launched/blob/main/organizador.exe).

2. **Ejecutar el Script:**
   - Ejecute dando enter o doble clic.
   - El sistema le preguntará por la ruta de la carpeta que se necesita organizar.
   - - **Nota:** Utilice barras invertidas (`\`) en la ruta.
   - Estas son las extensiones recividas, por el momento
     - .txt: documentos,
     - .docx: documentos,
     - .pdf: documentos,
     - .jpg: imagenes,
     - .png: imagenes,
     - .exe: ejecutables,
     - predeterminada = 'otros'  

## Para modificaciones

1. **Descargar el Script:**
   - Asegúrese de tener instalado Python 3.x en su sistema.
   - [Descargue el script (`organizador.py`)](https://github.com/AND3SIL4/Genesis-CeluWeb/blob/main/python-script-genesis/scraping.py).

2. **Ejecutar el Script:**
   - Abra una terminal o símbolo del sistema.
   - Navegue al directorio que contiene el script usando el comando `cd`.
   - Ejecute el script con el siguiente comando:
  
     ```bash
     python organizador.py
     ```

3. **Ingresar la Ruta de la Carpeta:**
   - Ingrese la ruta completa de la carpeta que desea organizar cuando se le solicite.
     - **Nota:** Utilice barras invertidas (`\`) en la ruta.

4. **Revisar la Salida:**
   - El script organizará los archivos según sus extensiones en carpetas respectivas.
   - Se mostrará un mensaje indicando que los archivos se han organizado correctamente.

## Configuración

El script utiliza un diccionario (`extenciones_dict`) para mapear extensiones de archivo a nombres de carpeta específicos. Puede personalizar este diccionario según sus preferencias.

```python
extenciones_dict = {
    '.txt': 'documentos',
    '.docx': 'documentos',
    '.pdf': 'documentos',
    '.jpg': 'imagenes',
    '.png': 'imagenes',
    '.exe': 'ejecutables',
}

predeterminada = 'otros'  # Carpeta predeterminada para extensiones no identificadas
