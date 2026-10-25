# 🎬 Guion para el Video de Presentación (2 a 4 minutos)

**Actividad Didáctica 2-M1: Simulación de Yahtzee con Método de Montecarlo (Grupo 3)**  
**Presentadores:** Raúl Santiago Morales Henao y David Octavio Castro Mora  
*(Integrantes del Grupo 3: Raúl Santiago Morales Henao, David Octavio Castro Mora y Claudia Dilbani Enríquez Botina)*

Este guion está organizado y distribuido equitativamente entre **Santiago** y **David** para una explicación fluida, dinámica y alineada con el cuaderno [`Grupo3_Montecarlo.ipynb`](file:///c:/Users/shena/OneDrive/Desktop/S20%20-%20M%C3%B3dulo%201.%20Actividad%20did%C3%A1ctica%202-M1%20-%20Grupo%203/Grupo3_Montecarlo.ipynb).

---

### ⏱️ Minuto 0:00 - 0:45 | 1. Introducción y Objetivo
*(En pantalla: Portada del documento o inicio del cuaderno de Google Colab `Grupo3_Montecarlo.ipynb`)*

🎤 **SANTIAGO:**
> *"Hola a todos, cordial saludo. Mi nombre es **Santiago Morales Henao** y hoy, junto a mi compañero **David Castro Mora**, les presentaremos el desarrollo de la Actividad Didáctica 2 del Módulo 1 para la asignatura de Simulación. Nuestro equipo, el Grupo 3, está conformado por Claudia Dilbani Enríquez, David Castro y quien les habla."*

🎤 **DAVID:**
> *"Hola a todos. El objetivo principal de nuestro proyecto es comprender e implementar computacionalmente el **Método de Montecarlo** aplicado al juego clásico de dados **Yahtzee** para dos jugadores. A través de este simulador en Python, modelamos la incertidumbre propia de los lanzamientos y explotamos estadísticamente miles de resultados aleatorios para validar la teoría de probabilidades."*

---

### ⏱️ Minuto 0:45 - 1:35 | 2. Fundamento Teórico (Distribución Uniforme y Cadenas de Markov)
*(En pantalla: Sección 1 del cuaderno de Google Colab mostrando las fórmulas de probabilidad)*

🎤 **DAVID:**
> *"Para construir el modelo matemático, partimos de dos conceptos clave:*  
> *Primero, la **Distribución de Probabilidad Uniforme Discreta**: en el juego utilizamos 5 dados balanceados e independientes de 6 caras. Por tanto, cada cara del 1 al 6 tiene exactamente la misma probabilidad de salir en cada tiro, que es de un sexto, es decir, aproximadamente un **16.67%**."*

🎤 **SANTIAGO:**
> *"Y segundo, la relación con los **Procesos y Cadenas de Markov**: en cada turno de Yahtzee, un jugador tiene hasta tres lanzamientos. Cada lanzamiento representa un 'estado' definido por los dados que el jugador decide conservar. La probabilidad de lograr una jugada en el siguiente tiro depende únicamente de los dados retenidos en el estado actual y del azar de los dados relanzados, sin importar qué salió en los tiros pasados, cumpliendo así la propiedad de pérdida de memoria de Markov."*

---

### ⏱️ Minuto 1:35 - 2:35 | 3. Explicación del Código en Google Colab
*(En pantalla: Secciones 2, 4 y 5 del archivo `Grupo3_Montecarlo.ipynb` en Google Colab)*

🎤 **SANTIAGO:**
> *"Pasando a la implementación en Google Colab, estructuramos el código en bloques modulares:*  
> *- En la función `lanzar_dados()`, utilizamos `random.randint(1, 6)` para generar tiradas pseudoaleatorias bajo el método de Montecarlo.*  
> *- Luego, en la función `calcular_puntos()`, programamos la lógica de las **13 categorías oficiales**: tanto la sección superior (de Unos a Seises) como la sección inferior (Trío, Cuarteto, Full House, Escalera Menor, Escalera Mayor, Yahtzee y Chance)."*

🎤 **DAVID:**
> *"Más abajo implementamos la dinámica interactiva para **dos jugadores** mediante las funciones `crear_tablero()`, `mostrar_marcador()`, `turno_jugador()` y `jugar()`.*  
> *En cada ronda, el sistema alterna el turno entre los dos jugadores, muestra los 5 dados iniciales y permite decidir hasta dos veces qué posiciones conservar o volver a lanzar. Al final del turno, el programa calcula automáticamente los puntos posibles en las categorías disponibles y actualiza el marcador general hasta declarar al ganador."*

---

### ⏱️ Minuto 2:35 - 3:30 | 4. Resultados y Simulación de Montecarlo (10,000 Tiradas)
*(En pantalla: Sección 3 del cuaderno con las dos gráficas de barras y la tabla de resultados numéricos)*

🎤 **DAVID:**
> *"Para la explotación estadística de Montecarlo, ejecutamos un experimento de **10,000 tiradas consecutivas** de 5 dados, lo que equivale a 50,000 dados lanzados:*  
> *En la **primera gráfica** (a la izquierda), comprobamos cómo la frecuencia empírica de cada una de las 6 caras converge justo sobre la línea roja del **16.67% teórico**, demostrando la Ley de los Grandes Números."*

🎤 **SANTIAGO:**
> *"Y en la **segunda gráfica** (a la derecha), analizamos la probabilidad empírica de obtener jugadas directas en el primer lanzamiento. En nuestra corrida de 10,000 simulaciones obtuvimos:*  
> *- **Trío:** alrededor del **21.4%***  
> *- **Escalera Menor:** cerca del **15.5%***  
> *- **Full House:** aproximadamente **4.1%***  
> *- **Escalera Mayor:** un **2.9%***  
> *- Y el **Yahtzee** directo (5 dados iguales): apenas un **0.11%**, cifras que coinciden con gran precisión con las probabilidades teóricas combinatorias."*

---

### ⏱️ Minuto 3:30 - 4:00 | 5. Conclusiones y Cierre
*(En pantalla: Consola con la ejecución de la partida de prueba entre David y Santiago, y vista del repositorio en GitHub)*

🎤 **DAVID:**
> *"Como conclusión, el Método de Montecarlo nos permitió verificar experimentalmente probabilidades complejas sin necesidad de cálculos analíticos extensos, demostrando además cómo las Cadenas de Markov modelan la toma de decisiones bajo incertidumbre en juegos de estrategia."*

🎤 **SANTIAGO:**
> *"Todo el código fuente, la simulación interactiva y la documentación completa están disponibles en nuestro repositorio de GitHub y en el cuaderno de Google Colab adjuntos en el informe. Muchas gracias por su atención."*

🎤 **DAVID:**
> *"¡Muchas gracias!"*

---

### 💡 Recomendaciones rápidas para la grabación (David y Santiago):
1. **Reunión en Meet / Zoom / Teams:** Uno de los dos comparte pantalla con el cuaderno `Grupo3_Montecarlo.ipynb` abierto en Google Colab y va bajando suavemente mientras cada uno habla.
2. **Duración ideal:** Siguiendo este guion a ritmo natural, les tomará cerca de **3 minutos y 15 segundos**, cumpliendo perfectamente el rango de 2 a 4 minutos de la rúbrica.
3. **Respaldo visual:** Al hablar de la sección 5, muestren brevemente la salida de consola donde aparecen los turnos jugados entre `david` y `santiago`.
