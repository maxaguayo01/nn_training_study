

````markdown
# 🧠 Proyecto de Experimentos de Modelos Baseline y Ejes (Axes)

## 📘 Introducción
Este proyecto tiene como objetivo realizar y comparar diferentes experimentos de aprendizaje automático utilizando modelos base (*baselines*) y variaciones a lo largo de distintos ejes experimentales (*axis experiments*).  

Se busca evaluar el rendimiento de los modelos, analizar los efectos de distintos hiperparámetros y documentar los resultados obtenidos de manera reproducible y organizada.  

El repositorio incluye todos los archivos necesarios para replicar los experimentos: dependencias, configuraciones, instrucciones de ejecución y resultados del mejor modelo.

---

## 🎯 Objetivos
- Implementar modelos base que sirvan como punto de comparación inicial.  
- Diseñar experimentos modificando hiperparámetros y estructuras de red para evaluar su impacto.  
- Documentar de forma clara los pasos de entrenamiento y evaluación.  
- Guardar y compartir el mejor modelo con su configuración exacta para asegurar reproducibilidad.

---

## ⚙️ Configuración del entorno

### Opción 1: Usando `requirements.txt`
```bash
pip install -r requirements.txt
````

### Opción 2: Usando `environment.yml` (Conda)

```bash
conda env create -f environment.yml
conda activate experiment_env
```

### Dependencias principales

* `torch`
* `torchvision`
* `numpy`
* `pandas`
* `tqdm`
* `scikit-learn`
* `matplotlib`

---

## 🧩 Estructura del Proyecto

```
📂 proyecto_experimentos/
│
├── Untitled-4.ipynb           # Notebook principal con los experimentos
├── requirements.txt           # Dependencias exactas (para pip)
├── environment.yml            # Entorno reproducible (para conda)
├── README.md                  # Instrucciones y reporte del proyecto
├── best_checkpoint.pt         # Mejor modelo entrenado (opcional)
└── best_config.json           # Configuración del mejor modelo
```

---

## 🚀 Ejecución de los Experimentos

### 1️⃣ Correr los modelos *Baseline*

Abre el notebook principal:

```bash
jupyter notebook nn_training_study.ipynb
```

Ejecuta las primeras celdas para entrenar los modelos base (ej. Regresión Lineal, Random Forest, MLP simple).
Estos resultados servirán como punto de referencia.

### 2️⃣ Correr los *Axis Experiments*

Cada “eje” representa un cambio experimental específico:

* **Eje 1 – Modelo:** probar diferentes algoritmos (Random Forest, Gradient Boosting, MLP, etc.)
* **Eje 2 – Hiperparámetros:** variar *learning rate*, *batch size*, *n_estimators*, *hidden layers*, etc.
* **Eje 3 – Datos:** usar distintas divisiones o preprocesamientos del dataset.
* **Eje 4 – Regularización:** aplicar técnicas como *dropout*, *early stopping*, *weight decay*.



## 📊 Resultados y Análisis

Los resultados mostraron mejoras notables al ajustar los hiperparámetros y aplicar técnicas de regularización.
Los modelos optimizados superaron a los baselines en métricas como **MAPE**, **RMSE** y **R²**.


**Conclusiones:**

* Los modelos baselines sirvieron como un punto sólido de comparación.
* Los ejes experimentales facilitaron el análisis sistemático de las variables más influyentes.
* La regularización mejoró significativamente la capacidad de generalización.
* Se logró un entorno totalmente reproducible y documentado.

---

## 📁 Archivos Entregables

| Archivo              | Descripción                                         |
| -------------------- | --------------------------------------------------- |
| `requirements.txt`   | Lista exacta de dependencias (pip).                 |
| `environment.yml`    | Configuración de entorno (conda).                   |
| `Untitled-4.ipynb`   | Notebook con la ejecución de los experimentos.      |
| `best_checkpoint.pt` | Checkpoint del mejor modelo entrenado.              |
| `best_config.json`   | Configuración del mejor modelo.                     |
| `README.md`          | Documento con reporte e instrucciones del proyecto. |

---

## 📚 Referencias

* [PyTorch Documentation](https://pytorch.org/docs/)
* [NumPy Documentation](https://numpy.org/doc/)
* [Scikit-learn](https://scikit-learn.org/stable/)
* [tqdm Progress Bars](https://tqdm.github.io/)
* [Matplotlib](https://matplotlib.org/)

---

## ✍️ Autores

**Nombre:** Maximiliano,cesar, ivanna, david 
**Curso:** Gestión de Riesgos / Machine Learning Experiments
**Fecha:** Octubre 2025

```


