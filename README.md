# Proyecto Final - Vision por Computador

Proyecto de la semana 1 con desarrollo en notebook para:

- Parte 1: extraccion de caracteristicas y comparacion de filtros.
- Parte 2: clasificacion de imagenes (gatos vs perros) con HOG + SVM.

## Estructura actual del proyecto

```text
ProyectoSemanaUno/
├─ .github/
├─ src/
│  ├─ code/
│  │  └─ trabajo_grupal.ipynb
│  ├─ dataset/
│  │  ├─ train/
│  │  │  ├─ cats/
│  │  │  └─ dogs/
│  │  ├─ val/
│  │  │  ├─ cats/
│  │  │  └─ dogs/
│  │  └─ test/
│  │     ├─ cats/
│  │     └─ dogs/
│  └─ docs/
└─ README.md
```

## Estado finalizado

- Notebook principal creado: `src/code/trabajo_grupal.ipynb`.
- Titulos y formato de presentacion listos (Parte 1 y Parte 2).
- Integrantes del grupo agregados en la portada del notebook.
- Seleccion de imagen aleatoria desde `train/cats` para la Parte 1.
- Paso previo de instalacion condicional de librerias agregado (solo instala si faltan).
- Dataset dividido en entrenamiento, validacion y prueba.

## Distribucion del dataset

Division aplicada: `70/15/15` estratificada por clase.

- `train/cats`: 708
- `train/dogs`: 709
- `val/cats`: 152
- `val/dogs`: 152
- `test/cats`: 152
- `test/dogs`: 152

## Que contiene el notebook

1. Paso previo para instalar dependencias si no estan disponibles.
2. Parte 1:
	- Carga de imagen (aleatoria en entrenamiento de gatos).
	- Escala de grises.
	- Canny y Sobel.
	- Comparacion visual y analisis.
3. Parte 2:
	- Carga de dataset por split.
	- Visualizacion de ejemplos.
	- Extraccion de caracteristicas HOG.
	- Entrenamiento con `LinearSVC`.
	- Evaluacion con exactitud, reporte de clasificacion y matriz de confusion.

## Dependencias

- Python 3.10+
- opencv-python
- numpy
- matplotlib
- scikit-learn

## Ejecucion recomendada

Desde `src/code/trabajo_grupal.ipynb`, ejecutar celdas en orden:

1. Instalacion condicional de librerias.
2. Imports.
3. Parte 1 completa.
4. Parte 2 completa.

Si el kernel ya tiene librerias instaladas, el paso de instalacion no realiza cambios.
