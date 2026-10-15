## Ambiente de simulación para entrenamiento de RL

Se desarrolló un ambiente de simulación utilizando el simulador MuJoCo y los modelos de los robots Unitree G1 y Booster T1. Este ambiente simula la dinámica de los robots incluyendo varias variables importantes para el entrenamiento de caminatas como:

* Fricciones viscosas y secas en las articulaciones
* Fricción del pie con el suelo
* Fuerza de contacto del pie con el suelo
* Colisiones del robot consigo mismo

La siguiente imagen muestra un ejemplo de dicho ambiente con el robot Unitree G1:

[simulador](https://github.com/mnegretev/PAPIIT-IN118226/blob/main/Resultados%20de%20RL%20en%20simulación/Simulador.png)

En esta misma carpeta se incluyen algunos videos con los resultados obtenidos usando este simulador:

* "booster_t1_balanceado.mp4" muestra un entrenamiento para recuperación de caída usando Proximal Policy Optimization para el robot Booster T1.
* "unitree_mala_recompensa.mp4" muestra un entrenamiento similar pero para el robot Unitree G1.
* "unitree_levantamiento.mp4" muestra un entrenamiento para recuperación de caída con una alta penalización a la energía consumida.
* "unitree_levantamiento2.mp4" muestra un entrenamiento similar pero sin penalizar el consumo de energía, lo que hace que se vean movimientos bruscos.
* "Caminata1.mp4" y "Caminata2.mp4" muestran los resultados de entrenamientos para caminata ya probados en el robot Unitree G1 en el Laboratorio de Investigación en Robótica Avanzada. 
