# Definimos las dimensiones de la matriz 3D
from main import temperaturas

ciudades = ["Quito", "Guayaquil", "Cuenca"]
dias = ["lunes","Martes","Miercoles","Jueves","Viernes"]
semanas = 2
# Inicializamos la matriz 3D con datos de temperaturas aleatorios
import random

temperaturas = [[[random.randint(10, 30)for-in range(len(dias))] for _ in range(semanas)] for _ in range(len(ciudades))]

# Imprimir la matriz de temperaturas para verificar los datos generados
for ciudad_index, ciudad in enumerate(ciudades):
    print(f"temperaturas para {ciudad}")
    for dia_index, dia in enumerate():
        for semana_index in range(semanas):
            print(f"  Semana {semana_index + 1}: {temperaturas[ciudad_index][semana_index]}")
        print()

# Calcular el promedio de temperaturas para cada ciudad por semana
for ciudad_index, ciudad in enumerate(ciudades):
    print(f"Promedios de temperaturas semanales para {ciudad}:")
    for semana_index in range(semanas):
    suma_temperaturas = sum(temperaturas[ciudad_index][semana_index])
    promedio_temperatura = suma_temperaturas / len(dias)
    print(f"  Semana {semana_index + 1}: {promedio_temperatura:.2f}°C")
print()
