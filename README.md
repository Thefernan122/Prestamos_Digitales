# Prestamos_Digitales
📊 Predicción del Monto de Préstamos Digitales con Python y Redes Neuronales
🎯 Objetivo General
Aplicar técnicas de regresión lineal y redes neuronales artificiales para predecir el monto de préstamos digitales otorgados a clientes peruanos, utilizando Python, TensorFlow/Keras y control de versiones con GitHub.

🎯 Objetivos Específicos
Implementar una regresión lineal simple.

Desarrollar una red neuronal con Keras.

Manipular datos usando Pandas y NumPy.

Visualizar resultados con Matplotlib.

Aplicar estructuras básicas de programación.

Usar GitHub como sistema de control de versiones.

🧾 Descripción del Dataset
Fuente: Kaggle
Archivo: dataBasePrestDigital.csv
Columnas relevantes:

ventaPrestDig: Variable objetivo (monto del préstamo digital).

promConsBanco3Um, promSaldoBanco3Um, promSaldoPrest3Um: Variables numéricas usadas como input para la red neuronal. (Nota: Asegúrate de listar todas las que usaste para la NN y la variable para la Regresión Lineal)

🧰 Librerías Utilizadas
pandas

numpy

matplotlib

tensorflow / keras

scikit-learn

🤖 Modelos Desarrollados
🔹 Regresión Lineal Simple
Se seleccionó la variable promSaldoBanco3Um como predictora del monto. (Confirma si esta fue la variable para la Regresión Lineal Simple, en tu código anterior era trxDigitalUm).

Se aplicó LinearRegression() de sklearn.

🔹 Red Neuronal Artificial
Arquitectura:

Capa oculta 1: 32 neuronas, activación relu

Capa oculta 2: 16 neuronas, activación relu

Capa salida: 1 neurona, activación linear

Configuración:

Pérdida: mse

Métrica: mae

Epochs: 50

Batch size: 32

📈 Gráficas
(Aquí deberías insertar tus gráficas. Ejemplo de cómo referenciarlas si están en una carpeta imagenes)

Evolución del Error (MSE) de la Red Neuronal:
![descarga3](https://github.com/user-attachments/assets/9202eadb-1c14-4f7f-8ece-b573ff1b6431)

Predicción vs Real (Red Neuronal):
![descarga4](https://github.com/user-attachments/assets/dffe602d-9a13-4070-876d-e9dc3934f202)

Regresión Lineal Simple:

![descarga5](https://github.com/user-attachments/assets/a2333eda-a960-46bb-9039-de5380a39358)


🧠 Lógica de Programación
Uso de lista (errores) para almacenar errores absolutos de las predicciones de la red neuronal.

Uso de diccionario (conteo) para agrupar los errores por rangos predefinidos.

Implementación de estructuras de control for (para iterar sobre predicciones) y if (para clasificar los errores) en el análisis del modelo de red neuronal.

✅ Conclusiones Personales
La red neuronal tuvo un muy buen rendimiento, con un error medio absoluto (MAE) de 0.0061 en el conjunto de prueba. (Asegúrate que esta métrica y valor sean los correctos de tu evaluación final).

Más del 96% de las predicciones de la red neuronal tuvieron un error absoluto menor a 0.01, lo cual es excelente y demuestra una alta precisión del modelo.

El uso de Keras facilita enormemente la creación y experimentación con modelos de redes neuronales potentes, requiriendo relativamente pocas líneas de código.

Este proyecto demuestra el potencial de la inteligencia artificial y el machine learning para desarrollar herramientas de apoyo en la toma de decisiones financieras, como la estimación de montos de préstamos.
