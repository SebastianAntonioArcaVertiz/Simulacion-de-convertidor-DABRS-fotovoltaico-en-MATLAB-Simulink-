**Simulación de Convertidor DC-DC DAB-SR con Algoritmo MPPT y aplicación en AppDesigner**



Este repositorio contiene la simulación interactiva de un convertidor DC-DC de Doble Puente Activo Serie Resonante (DAB-SR) aplicado a sistemas solares fotovoltaicos. 



La topología del circuito, el principio del algoritmo de Perturbar y Observar (P\&O) y los parámetros teóricos base utilizados en este proyecto toman como referencia el siguiente artículo de investigación:



> Arredondo, J., \& Sal y Rosas, D. (2019). **Series-Resonant DC-DC Converter for Solar Photovoltaic Non Isolated Applications.** CHILECON 2019, Valparaíso, Chile.



Además, a partir de esta misma referencia se realizó un examen parcial para el curso de Electrónica de Potencia II.



Este repositorio aporta el desarrollo de software y la simulación computacional:

**Modelado en Simulink:** Implementación del circuito de potencia con un switch que permite alternar entre el modo manual (donde el usuario es capaz de colocar el ángulo con el que quiere controlar el convertidor), y el modo PI (el cual me da una respuesta estabilizada en un punto.

**Aplicativo en App Designer**: Aplicación diseñada desde cero en App Designer para permitir la modificación de variables, el monitoreo del seguimiento del punto de máxima potencia (MPPT) y la visualización del estado estacionario en tiempo real.



**Para ejecutar este proyecto, es necesario contar con:**

\* MATLAB (Versión R2024b o superior).

\* Simulink.

\* Simscape Electrical.

\*Control System Toolbox

\*Simulink Control Design

**Se tienen que seguir los siguientes pasos:**

1\. Se tiene que abrir el archivo PARCIAL\_POTENCIAII.slx

2\. Se abre el archivo app.mlapp

3\. En la aplicación, se establece la frecuencia de conmutación (según el paper es 50000 hz), esto es para diferenciar entre ZVS y ZCS, cabe aclarar, que según los componentes, la frecuencia de resonancia siempre sera 45.45 khz. Si queremos ZVS, la frecuencia de conmutación será mayor a este valor, y si queremos ZCS, será menor.

4\. Se puede activar o desactivar el PI.

5\. Si se opta por el modo manual, podemos controlar la corriente de entrada estableciendo un ángulo de desfase.

6\. Para simular, presionamos el botón simular y graficar, (EL SIMULINK DEBE ESTAR ABIERTO)

