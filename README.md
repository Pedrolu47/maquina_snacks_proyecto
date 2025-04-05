# Máquina de Snacks

Este proyecto es una aplicación de consola que simula el funcionamiento de una máquina expendedora de snacks. Permite a los usuarios comprar snacks, agregar nuevos productos al inventario, y consultar el inventario disponible.

## Características

- **Comprar Snacks**: Los usuarios pueden seleccionar un snack por su ID y agregarlo a su ticket de compra.
- **Mostrar Ticket**: Muestra un resumen de los productos comprados y el total a pagar.
- **Agregar Snacks**: Permite agregar nuevos snacks al inventario.
- **Inventario de Snacks**: Muestra todos los snacks disponibles en la máquina.

## Estructura del Proyecto

El proyecto está organizado de la siguiente manera:

```
maquina_snacks_proyecto/
├── __init__.py
├── maquina_snacks.py       # Archivo principal que ejecuta la aplicación
├── servicio_snacks.py      # Lógica para gestionar el inventario de snacks
├── snack.py                # Clase que representa un snack
├── snacks.txt              # Archivo que almacena los snacks disponibles
└── __pycache__/            # Archivos compilados de Python
```

## Archivos Principales

### `maquina_snacks.py`
Este archivo contiene la clase `MaquinaSnacks`, que gestiona el flujo principal de la aplicación, incluyendo el menú interactivo y las opciones disponibles.

### `servicio_snacks.py`
Contiene la clase `ServicioSnacks`, que maneja la lógica relacionada con el inventario, como cargar snacks desde un archivo, guardar nuevos snacks y mostrar el inventario.

### `snack.py`
Define la clase `Snack`, que representa un producto con atributos como ID, nombre y precio.

### `snacks.txt`
Archivo de texto que almacena los snacks disponibles en la máquina. Se genera automáticamente si no existe.

## Requisitos Previos

- Python 3.10 o superior.
- Sistema operativo Windows.

## Instalación

1. Clona este repositorio o copia los archivos en tu máquina local.
2. Asegúrate de tener Python instalado.
3. Navega al directorio `maquina_snacks_proyecto`.

## Uso

1. Ejecuta el archivo principal:
   ```
   python maquina_snacks.py
   ```
2. Sigue las instrucciones en pantalla para interactuar con la máquina de snacks.

## Ejemplo de Uso

Al iniciar la aplicación, verás un menú como este:

```
*** Maquina de Snacks ***
Menu:
1. Comprar Snack
2. Mostrar ticket
3. Agregar Nuevo snack al inventario
4. Inventario de Snacks
5. Salir
Elige una opcion:
```

### Comprar un Snack
Selecciona la opción 1 e ingresa el ID del snack que deseas comprar. El snack se agregará a tu ticket.

### Mostrar el Ticket
Selecciona la opción 2 para ver un resumen de los snacks comprados y el total a pagar.

### Agregar un Nuevo Snack
Selecciona la opción 3 e ingresa el nombre y precio del nuevo snack. Este se agregará al inventario y se guardará en el archivo `snacks.txt`.

### Ver el Inventario
Selecciona la opción 4 para ver todos los snacks disponibles en la máquina.

## Notas

- El archivo `snacks.txt` se genera automáticamente si no existe.
- Si el archivo `snacks.txt` contiene datos duplicados o mal formateados, podrían ocurrir errores.

## Contribuciones

Si deseas contribuir a este proyecto, puedes enviar un pull request o reportar problemas en el repositorio.

## Licencia

Este proyecto está bajo la Licencia MIT.
