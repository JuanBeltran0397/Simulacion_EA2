# 🚗 Simulación y Predicción de Tráfico Vehicular mediante Modelos Ocultos de Markov (HMM)

Este proyecto implementa un **Modelo Oculto de Markov (HMM)** en Python para simular, analizar y predecir el comportamiento del tráfico vehicular en el contexto de una *Smart City*. A través de procesos estocásticos, el modelo infiere el estado real del tráfico basándose en lecturas probabilísticas de velocidad.

**Autores:** Camilo Alegría y Juan Beltrán

---

## 📋 Descripción del Proyecto

En el desarrollo de ciudades inteligentes, los sensores IoT a menudo capturan observaciones indirectas (como la velocidad promedio de los vehículos) en lugar del estado real y general de la vía. Este proyecto utiliza Cadenas de Markov para resolver este problema:

* **Estados Ocultos:** Tráfico Fluido, Tráfico Moderado, Tráfico Congestionado.
* **Observaciones (Emisiones):** Velocidad Alta (80-100 km/h), Media (40-80 km/h) y Baja (0-40 km/h).

El código incluye simulaciones de 24 horas (intervalos de 30 minutos), análisis de impacto ambiental (emisiones de CO2) y una comparación profunda entre la convergencia analítica y la simulación empírica de Monte Carlo.

---

## 🚀 Características Principales

* **Motor Estocástico:** Implementación desde cero de la clase `TrafficHMM` con matrices de transición y emisión personalizadas.
* **Métricas Avanzadas:** Cálculo automático de horas de congestión, índice de tráfico (0-100) y estimación de emisiones de CO2 basadas en el estado del flujo vehicular.
* **Visualización de Datos:** Generación de mapas de calor (Heatmaps), curvas de velocidad y un sistema de alertas semaforizado (🟢🟡🔴).
* **Análisis Teórico:** * Cálculo de la **Distribución Estacionaria** utilizando Eigenvectores (Álgebra Lineal).
    * Experimentación con la **Velocidad de Mezcla (Mixing Rate)** alterando la "inercia" de la matriz de transición.
    * Simulaciones **Monte Carlo** (100 ejecuciones) para validar la robustez probabilística del modelo.

---

## 🛠️ Tecnologías Utilizadas

El proyecto está desarrollado íntegramente en un entorno Jupyter Notebook utilizando las siguientes librerías de ciencia de datos:

* `Python 3.x`
* `NumPy`: Para operaciones matriciales, álgebra lineal y generación de números pseudoaleatorios.
* `Pandas`: Para estructuración, manipulación de datos temporales y cálculo de métricas.
* `Matplotlib` & `Seaborn`: Para la visualización avanzada de curvas de convergencia y mapas de calor.

---

## ⚙️ Instalación y Uso

1. **Clonar el repositorio:**
   ```bash
   git clone [https://github.com/tu_usuario/tu_repositorio.git](https://github.com/tu_usuario/tu_repositorio.git)
   cd tu_repositorio
