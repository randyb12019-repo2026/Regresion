# Regresion - Proyecto de Modelos de Regresion

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
├── src/                              # Modulos Python reutilizables (pendiente)
├── data/                             # Datasets generados o descargados (sklearn)
├── reports/                          # Reportes y conclusiones del analisis
├── Dockerfile                        # Imagen Python 3.13-slim con Jupyter
├── docker-compose.yml                # Orquestacion del contenedor con volumenes
├── .venv/                            # Entorno virtual Python 3.13
├── .gitignore                        # Exclusiones para git
├── requirements.txt                  # Dependencias del proyecto
├── LICENSE                           # Licencia MIT
└── README.md                         # Documentacion del proyecto
```

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

Randy Bonucci Martin — Proyecto educativo, Bootcamp Data & IA

## Licencia

MIT
