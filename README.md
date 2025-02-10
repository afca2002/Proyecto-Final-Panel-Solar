# Proyecto-Final-Panel-Solar

# Instalación de Dependencias para el Simulador de Seguidor Solar

Este proyecto requiere varias bibliotecas de Python para calcular la posición del sol, determinar los ángulos de orientación de un panel solar y visualizar los resultados en una interfaz gráfica.

## Prerrequisitos

- Tener Python 3.8 o superior instalado. Puedes verificar tu versión de Python ejecutando:
  ```sh
  python --version
  ```
- Tener `pip` actualizado:
  ```sh
  python -m pip install --upgrade pip
  ```

## Instalación de Librerías

Ejecuta el siguiente comando en una celda de Jupyter Notebook para instalar todas las dependencias necesarias:

```python
!pip install matplotlib numpy tkinter pytz pysolar astral
```

### Explicación de las dependencias

- `matplotlib`: Para generar gráficos en 3D.
- `numpy`: Para cálculos matemáticos y manipulación de matrices.
- `tkinter`: Para la interfaz gráfica interactiva (incluido en Python por defecto).
- `pytz`: Para manejar zonas horarias correctamente.
- `pysolar`: Para calcular la posición del sol en función de coordenadas geográficas y tiempo.
- `astral`: Para obtener información sobre el amanecer y atardecer.

## Ejecución del Programa

Una vez instaladas las librerías, puedes ejecutar el código en una celda de Jupyter Notebook:

```python
%run nombre_del_script.ipynb
```

Donde `nombre_del_script.ipynb` es el archivo que contiene el código.

## Solución de Problemas

Si experimentas problemas con `tkinter`, asegúrate de que está correctamente instalado en tu sistema:

- En Ubuntu/Debian:
  ```sh
  sudo apt-get install python3-tk
  ```
- En macOS:
  ```sh
  brew install python-tk
  ```

Si algún módulo falta o hay errores de importación, intenta reinstalarlo con:

```python
!pip install --force-reinstall nombre_del_paquete
```

## Notas

- Si deseas ejecutar el código en un entorno virtual dentro de Jupyter Notebook, puedes configurarlo con:
  ```sh
  python -m venv venv
  source venv/bin/activate  # En Windows usa: venv\Scripts\activate
  pip install -r requirements.txt
  ```
  Y para salir del entorno virtual:
  ```sh
  deactivate
  ```

¡Listo! Ahora puedes ejecutar el simulador de seguidor solar sin problemas en Jupyter Notebook.
