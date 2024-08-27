# python-programming-course
An introductory Python programming course
import matplotlib.pyplot as plt
import numpy as np

# Datos proporcionados
tráfico = np.array([1, 2, 3, 4, 5, 6, 7])
desgaste = np.array([3, 5, 6, 8, 10, 12, 13])

# Estimaciones de los parámetros
beta_0 = 1.7143
beta_1 = 1.6786

# Línea de regresión
y_regresion = beta_0 + beta_1 * tráfico

# Crear gráfico
plt.figure(figsize=(8, 6))
plt.scatter(tráfico, desgaste, color='blue', label='Datos observados')
plt.plot(tráfico, y_regresion, color='red', label='Línea de regresión')
plt.xlabel('Tráfico')
plt.ylabel('Desgaste')
plt.title('Regresión Lineal del Desgaste en Función del Tráfico')
plt.legend()
plt.grid(True)
plt.show()

