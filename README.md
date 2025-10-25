### Demostración: https://grupo-3-sistemas-operativos-umg.github.io/proyecto-3/

# Integrantes
* Andrea María Sarazúa Roca - 1990-23-17938
* Danny Emanuel Tiu - 1990-22-10522
* Luis René López Hernández - 1990-20-11078
* Willy David Tejax. - 1990-22-12652
* Wilson Armando Felipe 1990-18-7148

# Manual de usuario
El proyecto simula cómo un sistema operativo gestiona varios procesos usando distintos algoritmos de planificación:

* FCFS (First Come, First Served) → El primero que llega es el primero en ejecutarse.
<img width="1363" height="692" alt="image" src="https://github.com/user-attachments/assets/f198a892-6f56-4cce-bb15-dc5f41edb3c1" />

* SJF (Shortest Job First) → El proceso con menor tiempo requerido se ejecuta primero.
<img width="1345" height="689" alt="image" src="https://github.com/user-attachments/assets/23fd595c-88a4-4f54-b78b-8368316565a6" />

* Round Robin → Cada proceso obtiene un turno de CPU con duración igual al quantum. Cuando se le acaba, si aún no terminó, vuelve a la cola.
<img width="1350" height="681" alt="image" src="https://github.com/user-attachments/assets/0589bb85-ca8c-488d-b8fe-cf0b2057ed5e" />


El programa automatiza el trabajo del planificador: recibe procesos como entrada, aplica el algoritmo elegido y  muestra cómo se van ejecutando hasta que todos terminan.


## Instalación
1. Abrir el link compartido por el autor para poder ejecutar el simulador en la web.
2. También puede clonar el repositorio y abrirlo en un editor de código como visual studio


## Demostración de uso

## ¿Cómo interpretar la interfaz gráfica (UI)?

### Formulario de entrada (Nombre, Tiempo CPU, Llegada, Quantum)
Aquí se define los procesos:

* Nombre de Proceso: identificador que eliges (ej. “P1”).

* Duración: cuántas unidades de tiempo necesita el proceso en CPU.

* Llegada: en qué instante “entra” al sistema.

* Quantum: solo relevante si se usa Round Robin, es el tiempo en el cual un procecso puede tener el ocupado el CPU
  antes de generar un cambio de contexto.

### Tabla de procesos Ingresados
Lista todos los procesos que agregaste, mostrando su PID, nombre, tiempo, llegada y quantum.

### Configuración (Selector de Algoritmo)
Permite elegir qué estrategia de planificación aplicar, puede elegir entre FCFS, SJF o Round Robin como se muestra en
las imagenes de inicio de este manual de usuario.

Debajo de la configuración se tiene 2 opciones disponibles los cuales son:
1. Ejecutar en modo compacto -> el cual hace la vista más resumida pero siempre respetando los 3 segundos por cada unidad de tiempo
2. Reutilizar procesos para otro algoritmo al finalizar -> Este permite reutilizar los procesos ya añadidos para realizar
   simulación con otro algoritmo.

### Botón “Iniciar" Simulación
Lanza la simulación en tiempo real. Cada unidad de tiempo equivale a 3 segundos reales, por lo que verás la ejecución avanzar poco a poco.

### Diagrama de Procesos (Gantt)
Muestra visualmente el avance en vivo de ejecución de los procesos, representado en un Gantt (modo tabla) en este se 
diferencia cada proceso de otro ya que se representa cada proceso en una línea y con un color distinto.

Debajo del diagrama se muestra en modo lista, cómo fue la ejecución de los procesos y la cola respectiva generado en cada ejecución.

### Tabla Resumen de Ejecución
En esta tabla se muestra el resumen completo del simulador, como se muestra en la siguiente imagen:
<img width="1278" height="281" alt="image" src="https://github.com/user-attachments/assets/cefe50f2-7f8a-4454-bfab-ecc33594e383" />
