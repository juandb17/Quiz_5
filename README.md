# Proyecto: Búsqueda con Drones usando PSO 
Usar el algoritmo **PSO (Particle Swarm Optimization)** para ubicar drones en un área de búsqueda y tratar de cubrir la mayor probabilidad de encontrar supervivientes.

---

## Descripción del problema

- Área de búsqueda: **5 km x 5 km** (5000 m x 5000 m).  
- Número de drones: **10**.  
- Cada dron puede detectar en un radio de **200 m**.  
- Hay un **mapa de probabilidades** que indica en qué zonas es más probable encontrar supervivientes.  
- El objetivo es **colocar los drones** de forma que se cubra la mayor probabilidad posible.

En esta versión básica los drones **no se mueven**, solo se colocan en posiciones fijas.  

---

## Cómo funciona el código

1. Se crea un **mapa de probabilidades aleatorio** (una matriz de valores que suman 1).  
2. Cada partícula del PSO representa las **coordenadas (x,y)** de los 10 drones.  
3. La **función de evaluación** revisa cuánta probabilidad del mapa queda cubierta por el rango de detección de los drones.  
4. El algoritmo PSO busca las mejores posiciones actualizando la población de soluciones durante varias iteraciones.  
5. Al final se imprime la mejor cobertura encontrada y se muestra un gráfico con:  
   - El mapa de probabilidades (colores).  
   - Las posiciones de los drones (puntos rojos con `x`).  

---

## Requisitos

Este código está pensado para ejecutarse en **Google Colab** o en Python local.  
Necesita las siguientes librerías:
- `numpy`
- `matplotlib`

---

## Ejecución

En Colab:
1. Crear un nuevo notebook.  
2. Copiar y pegar el código en una celda.  
3. Ejecutar la celda.  

Se verá algo como esto:

- Mensajes de progreso:  
