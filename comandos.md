# Comandos Básicos de Linux para Manejo de Archivos

## Listar Archivos y Directorios

- **`ls`**: Muestra un listado de archivos y directorios.
  - **`ls -l`**: Muestra información detallada (permisos, dueño, tamaño, etc.).
  - **`ls -a`**: Incluye archivos ocultos (nombres que comienzan con `.`).

## Visualizar Contenido de Archivos

- **`cat`**: Muestra el contenido de un archivo. También útil para concatenar archivos.
- **`more`**: Muestra el contenido de archivos largos de forma paginada (pausa por pantalla).
- **`less`**: Similar a `more`, pero con navegación interactiva (flechas, páginas arriba/abajo). Presionar `q` para salir.

## Comodines para Operaciones con Archivos

- **`*`**: Representa cualquier cadena de caracteres (incluye cadena vacía).
- **`?`**: Representa un único carácter (debe estar presente).
- **`[ ]`**: Especifica un rango de caracteres o números. Ejemplo: `[0-6]`.
- **`{ }`**: Indica opciones separadas por comas. Ejemplo: `{SD,tti,PS}*`.

## Copiar, Mover y Renombrar Archivos

- **`cp`**: Copia archivos o directorios.
  - Ejemplo:  
    ```bash
    cp archivo1 archivo2          # Copia archivo1 a archivo2
    cp archivo1 ~/Escritorio/     # Copia archivo1 al Escritorio
    ```
- **`mv`**: Mueve o renombra archivos/directorios.
  - Ejemplo:  
    ```bash
    mv archivo1 archivo_1         # Renombra archivo1
    mv archivo1 ~/Escritorio/     # Mueve archivo1 al Escritorio
    ```

## Eliminar Archivos y Directorios

- **`rm`**: Elimina archivos.
  - **`rm -r`**: Elimina directorios y su contenido de forma recursiva.
  - **`rm -rf`**: Fuerza la eliminación sin confirmación (¡usar con cuidado!).

## Crear Enlaces entre Archivos

- **`ln`**: Crea enlaces simbólicos o duros.
  - Ejemplo:  
    ```bash
    ln archivo_origen enlace      # Crea un enlace a archivo_origen
    ```

## Buscar Archivos con `find`

- **Sintaxis básica**:  
  ```bash
  find [directorio] -criterio [argumento]
