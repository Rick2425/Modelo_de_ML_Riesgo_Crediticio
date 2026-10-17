## 🚀 Versión 1.0: Primer Modelo Base (LightGBM)

En esta primera iteración del proyecto, el enfoque principal estuvo en establecer un modelo de clasificación sólido utilizando exclusivamente **variables cuantitativas**. 

### 🛠️ Preprocesamiento y Feature Engineering
* **Transformación de Variables:** Se aplicaron criterios de transformación y creación de nuevas categorías a partir de los datos numéricos, lo cual aportó un valor predictivo significativo al algoritmo.
* **Manejo de Desbalance:** La variable objetivo (`Moroso`) presentaba un sesgo considerable. Para mitigar esto y evitar que el algoritmo priorizara la clase mayoritaria, se implementó un método de **muestreo estratificado**, garantizando una representación equitativa durante el entrenamiento.

### 🧠 Algoritmo y Entrenamiento
* **Modelo Seleccionado:** **LightGBM**. Se optó por este modelo basado en árboles de decisión debido a su probada eficacia y excelente rendimiento para este tipo de datos.
* **Código Fuente:** El detalle de los *features* utilizados y el flujo de trabajo se encuentran en el cuaderno [`PrimerModelo.ipynb`](PrimerModelo.ipynb).

### 📊 Evaluación y Resultados
Para validar el potencial del modelo en la clasificación correcta de nuestro Target, se evaluó su capacidad predictiva mediante la **Curva ROC y el AUC**, midiendo la tasa de falsos positivos y falsos negativos.

* **Score AUC Obtenido:** **🏆 0.74541**

Alcanzar este puntaje en nuestro primer análisis completo ha sido un resultado genial y un gran alivio. Este desempeño establece un excelente punto de partida (*baseline*) sólido, el cual quedará documentado en este repositorio para medir y comparar directamente cómo evoluciona el rendimiento del modelo en las futuras iteraciones.
