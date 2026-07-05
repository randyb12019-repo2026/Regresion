# Regresion - Proyecto de Modelos de Regresion

[![GitHub Pages](https://img.shields.io/badge/demo-%F0%9F%9A%80%20GitHub%20Pages-00f0ff?style=for-the-badge)](https://randyb12019-repo2026.github.io/Regresion/)
[![NBViewer](https://img.shields.io/badge/demo-%F0%9F%93%93%20NBViewer-a855f7?style=for-the-badge)](https://nbviewer.org/github/randyb12019-repo2026/Regresion/blob/main/notebooks/regresion.ipynb)

Actividad del Bootcamp de Data Analysis & IA en **Upgrade Hub**.

Proyecto educativo de regresion lineal, multiple y polinomica con Python y scikit-learn.

## Datasets utilizados

- **California Housing** — 20,640 bloques de viviendas, 8 variables (MedInc, HouseAge, AveRooms, etc.)
- **Diabetes** — 442 pacientes, 10 variables clinicas (edad, IMC, presion, etc.)
- **Coches (sintetico)** — 500 registros generados con relacion conocida precio = f(antiguedad, kms, potencia)

## Contenido del notebook

1. Regresion Lineal Simple (MedInc vs precio)
2. Regresion Lineal Simple (HouseAge vs precio)
3. Metricas: MAE, RMSE, R²
4. Regresion Multiple (todas las variables)
5. Regresion Polinomica (grados 1-15, deteccion de overfitting)
6. Modelo con Diabetes dataset (entrenamiento, evaluacion, prediccion)
7. Modelo con datos sinteticos de coches
8. Tabla comparativa de modelos de regresion (Ridge, Lasso, ElasticNet, etc.)

## Estructura del proyecto

```
Regresion/
├── notebooks/
│   └── regresion.ipynb               # Notebook principal con modelos de regresion
├── Dockerfile                        # Imagen Python 3.13-slim con Jupyter
├── docker-compose.yml                # Orquestacion del contenedor con volumenes
├── .venv/                            # Entorno virtual Python 3.13
├── .gitkeep
├── requirements.txt                  # Dependencias del proyecto
├── LICENSE                           # Licencia MIT
└── README.md                         # Documentacion del proyecto
```

## Demo

Puedes ver el notebook completo renderizado aquí:

- **🚀 GitHub Pages** — https://randyb12019-repo2026.github.io/Regresion/
- **📓 NBViewer** — https://nbviewer.org/github/randyb12019-repo2026/Regresion/blob/main/notebooks/regresion.ipynb

## Requisitos

```bash
pip install -r requirements.txt
```

## Docker

### Construir y ejecutar

```bash
docker compose build
docker compose up
```

Esto inicia un contenedor con el notebook listo para usar.

### Ejecutar notebook dentro del contenedor

```bash
docker compose run --rm regresion jupyter notebook --ip=0.0.0.0 --port=8888 --allow-root
```

## Autor

Randy Bonucci — Proyecto educativo, Bootcamp Data & IA

## Licencia

MIT
