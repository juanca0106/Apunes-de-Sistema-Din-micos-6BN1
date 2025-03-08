# Clase 2
## 07/02/2025
### Definiciones y repaso de ecuaciones diferenciales 
#### 1. Definiciones

>* 🔑 **Sistema**:
Un sistema es un conjunto de componentes que interactúan para lograr un objetivo específico, siguiendo reglas o principios que vinculan entradas con salidas.

💡 Ejemplo 1: un automóvil.

* Componentes: motor, transmisión, frenos, dirección, etc
* Entradas: combustible, energía eléctrica, fuerza del conductor
* Proceso: el motor convierte el combustible en energía mecánica, que se transmite a las ruedas.
* Salidas: movimiento del vehículo, emisión de gases, consumo de energía.

 El automóvil funciona siguiendo principios mecánicos y físicos que relacionan las entradas con las salidas para cumplir su objetivo: 
 transportar personas o carga.
 
 💡 Ejemplo 2: figura de ilustracion.

![image](https://github.com/user-attachments/assets/a69a2ce2-5ae3-4804-997b-bde9b8fceb0b)
---------------------------------------------------------------------------------------------
>* 🔑 **Sistema dinámico**:
>* Un sistema se llama dinámico si su salida en el presente depende de una entrada en el pasado
>* Si su salida en curso depende solamente de la entrada en curso, el sistema se conoce como estático.

💡 Ejemplo 1: calentador de agua con termostato:
* Entrada: temperatura del agua en el pasado y presente.
* Proceso: el termostato ajusta la potencia de calentamiento en función de la temperatura previa.
* Salida: temperatura del agua en el presente.
* Como la temperatura actual depende de valores anteriores (no solo de la entrada actual), es un sistema dinámico.

En contraste, un sistema estático sería una resistencia eléctrica, donde la temperatura del agua solo depende de la potencia aplicada en ese instante, sin influencia del pasado.

 💡 Ejemplo 2: figuras de ilustracion. 
 
   ![image](https://github.com/user-attachments/assets/faacb3e7-fef1-4133-8d89-182731af8da8)
--------------------------------------------------------------------------------------------------------------------
>* 🔑 **Planta**:
>* Es todo lo físico que permite que se lleve a cabo un proceso
>* Puede ser representado matemáticamente
>* Puede ser representado a través de uno o varios sistemas

💡 Ejemplo 1: Planta en un sistema de control de temperatura
* Físico: Un horno industrial.
* Proceso: La resistencia calienta el aire dentro del horno.
* Representación matemática: Se modela con ecuaciones diferenciales que relacionan la energía suministrada con la temperatura interna.
* Sistemas involucrados: Sistema de calefacción, sensores de temperatura, controlador PID

 ##### **ecuacion del ejemplo 1**
<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=   C\frac{dT}{dt}= P-h(T-T_{a})"><img src="http://www.alciro.org/cgi/tex.cgi?   C\frac{dT}{dt}= P-h(T-T_{a})" title="   C\frac{dT}{dt}= P-h(T-T_{a})" border="0" /></a>

donde 
* T: es la temperatura del horno (°C).
* t: es el tiempo (s).
* C: es la capacidad térmica del sistema (J/°C).
* P: es la potencia de calefacción aplicada (W).
* h: es el coeficiente de disipación de calor (W/°C).
* Ta: es la temperatura ambiente (°C).

💡 Ejemplo 2: Planta en un sistema de control de velocidad de un motor eléctrico
* Físico: Un motor de corriente continua.
* Proceso: La velocidad del motor depende del voltaje aplicado.
* Representación matemática: Se modela con ecuaciones de dinámica rotacional y circuitos eléctricos.
* Sistemas involucrados: Fuente de alimentación, controlador de velocidad, sensores de posición.

 ##### **ecuacion del ejemplo 2**
<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=   V= L\frac{di}{dt}+Ri+K_{b}\omega "><img src="http://www.alciro.org/cgi/tex.cgi?   V= L\frac{di}{dt}+Ri+K_{b}\omega " title="   V= L\frac{di}{dt}+Ri+K_{b}\omega " border="0" /></a>

donde 
* V: es el voltaje aplicado al motor (V).
* R: es la resistencia del devanado (Ω).
* i: es la corriente en el motor (A).
* Kb: es la constante de fuerza contraelectromotriz (V·s/rad).
* ω es la velocidad angular del motor (rad/s).
------------------------------------------------------------------------------------
>* 🔑 **Proceso**:
>* Es la secuencia de pasos que permite el desarrollo, o fabricación de un objetivo o producto
>* En el área de control se usa como sinónimo de planta
(Aunque en sentido estricto no lo son)
------------------------------------------------------------------------------------
>* 🔑 **Modelos dinámicos**:
>* En control interesa obtener un modelo matemático que relacione las variables de interés con el tiempo.

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=f(t)"><img src="http://www.alciro.org/cgi/tex.cgi?f(t)" title="f(t)" border="0" /></a>

>* Hay cambios de la variable con respecto al tiempo
>* Es necesario cuantificar cuanto cambia las variables de interés con respecto al tiempo.

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=\frac{df(t)}{dt}"><img src="http://www.alciro.org/cgi/tex.cgi?\frac{df(t)}{dt}" title="\frac{df(t)}{dt}" border="0" /></a>

------------------------------------------------------------------------------------
