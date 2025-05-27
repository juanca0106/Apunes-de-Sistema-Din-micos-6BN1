# CORTE 3 
## clase de Sistemas de tanques
### 📅 **Curso:** sistemas dinamicos 
### 👨‍🏫 **Profesor:** Ing. Jorge Eduardo Cote Ballesteros
### 🧑‍🎓 **Semestre:** Sexto (2025)
### 🧑‍🎓 **estudiantes** juan camilo cruz quintana,daniel corredor peña,Joan Sebastian Rojas**
------------------------------------------------------------------------
>* 🔑 **Sistemas de tanques**:
En sistemas industrials de tanques es deseable mantener flujo o nivel constante
------------------------------------------------------------------------
## ✍️ Introducción

### **¿QUE ES?**:
Un sistema de tanques es un modelo físico y matemático que representa cómo cambia el nivel de líquido (u otra variable como concentración o temperatura) en uno o más tanques interconectados a lo largo del tiempo. Este tipo de sistema se usa mucho en:
* Ingeniería de procesos (química, alimentos, petróleo)
* Automatización y control
* Dinámica de fluidos
* Educación en modelado matemático
-------------------------------------------------------------
### **🔧 Componentes típicos de un sistema de tanques**
 
* Tanques: Recipientes que almacenan un fluido.

* Entradas: Flujo de líquido que entra al tanque (bombas, válvulas, fuentes).

* Salidas: Flujo que sale del tanque (por gravedad, bombeo, etc.).

* Interconexiones: Flujo entre tanques, por tuberías.

* Sensores y actuadores (en sistemas de control): Para medir y regular el nivel.

-------------------------------------------------------------------------------------
## **🧮 ¿Qué se modela?**
La base del modelo es la ley de conservación de masa (o volumen, si el fluido es incomprensible):

**cambio del volumen = entrada-salida**

Si el área del tanque es constante (A), el volumen es V=Ah, y se puede expresar la variación del nivel del líquido h(t) como una ecuación diferencial.

----------------------------------------------------------------------------
### 💡 Ejemplo 1: 2 tamques 

![image](https://github.com/user-attachments/assets/4a283122-97a0-408c-9472-88a81e9dfb8a)

* 𝑞𝑖, 𝑞𝑜: 𝐹𝑙𝑢𝑗𝑜𝑠 𝑑𝑒 𝑒𝑛𝑡𝑟𝑎𝑑𝑎 𝑦 𝑠𝑎𝑙𝑖𝑑𝑎 𝑑𝑒 𝑙í𝑞𝑢𝑖𝑑o
* 𝑅1: 𝑅𝑒𝑠𝑖𝑠𝑡𝑒𝑛𝑐𝑖𝑎 𝑎𝑙 𝑓𝑙𝑢𝑗o
* 𝐴1: Á𝑟𝑒𝑎 𝑡𝑟𝑎𝑛𝑠𝑣𝑒𝑟𝑠𝑎𝑙 𝑑𝑒𝑙 𝑡𝑎𝑛𝑞𝑢e
* ℎ1: 𝑁𝑖𝑣𝑒𝑙 𝑑𝑒 𝑙í𝑞𝑢𝑖𝑑𝑜 𝑒𝑛 𝑒𝑙 𝑡𝑎𝑛𝑞𝑢e

 ## modelo de un tanque 
**Flujo de salida del tanque**

$$
q_1 = \frac{h_1}{r_1}
$$

esta ecuacion es analoga a la ley de ohm en electricidad: el flujo es proporcional a la "presion" cuanto mas alto este el nivel del lquidomayor sera el flujo de salida 

**Intercambio de energía**

$$
A_1 \frac{dh_1}{dt} = q_i - q_1
$$

donde: 

* el area tranversal del tanque es:
  
  <a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=A_{1}"><img src="http://www.alciro.org/cgi/tex.cgi?A_{1}" title="A_{1}" border="0" /></a>

* variacion de altura del liquido con respecto al tiempo es:

  <a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=\frac{dh_1}{dt}"><img src="http://www.alciro.org/cgi/tex.cgi?\frac{dh_1}{dt}" title="\frac{dh_1}{dt}" border="0" /></a>

* el flujo de etrada del tanque es:
  
  <a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=q_{i}"><img src="http://www.alciro.org/cgi/tex.cgi?q_{i}" title="q_{i}" border="0" /></a>

* el flujo de salida del tanque es:

  <a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=q_{1}"><img src="http://www.alciro.org/cgi/tex.cgi?q_{1}" title="q_{1}" border="0" /></a>

  
 ## Modelo 𝑞𝑖 como entrada y ℎ1 como salida

 **ecuaciones**

* <a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=q_1 = \frac{h_1}{r_1}"><img src="http://www.alciro.org/cgi/tex.cgi?q_1 = \frac{h_1}{r_1}" title="q_1 = \frac{h_1}{r_1}" border="0" /></a> 

*  <a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=\( A_1 \frac{dh_1}{dt} = q_i - q_1 \)"><img src="http://www.alciro.org/cgi/tex.cgi?\( A_1 \frac{dh_1}{dt} = q_i - q_1 \)" title="\( A_1 \frac{dh_1}{dt} = q_i - q_1 \)" border="0" /></a>

**remplazamos**

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=A_1 \frac{dh_1}{dt} = q_i - \frac{h_1}{R_1}"><img src="http://www.alciro.org/cgi/tex.cgi?A_1\frac{dh_1}{dt} = q_i - \frac{h_1}{R_1}" title="A_1 \frac{dh_1}{dt} = q_i - \frac{h_1}{R_1}" border="0" /></a>

esta ecuacion de primer orden describe como responder el nivel liquido (h1) ante el cambio de flujo de entrada (qi) 

## Modelo 𝑞𝑖 como entrada y 𝑞1 como salida

 **ecuaciones**

* <a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=q_1 = \frac{h_1}{r_1}"><img src="http://www.alciro.org/cgi/tex.cgi?q_1 = \frac{h_1}{r_1}" title="q_1 = \frac{h_1}{r_1}" border="0" /></a> 

*  <a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=\( A_1 \frac{dh_1}{dt} = q_i - q_1 \)"><img src="http://www.alciro.org/cgi/tex.cgi?\( A_1 \frac{dh_1}{dt} = q_i - q_1 \)" title="\( A_1 \frac{dh_1}{dt} = q_i - q_1 \)" border="0" /></a>


**despejamos h1**

$$
h_1 = q_1 R_1 
$$

el nivel del liquido tambien se puede representar de esa manera

**remplazamos en la ecuacion**

*  <a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=\( A_1 \frac{dh_1}{dt} = q_i - q_1 \)"><img src="http://www.alciro.org/cgi/tex.cgi?\( A_1 \frac{dh_1}{dt} = q_i - q_1 \)" title="\( A_1 \frac{dh_1}{dt} = q_i - q_1 \)" border="0" /></a>

eso quedaria como:

$$
R_1 A_1 \frac{dq_1}{dt} = q_i - q_1
$$

el cambio en el flujo de salida (q1) esta determinado por la diferencia entre el flujo que entra al tanque y el flujo que sale. 

----------------------------
### 📚 Ejercicio 1

![image](https://github.com/user-attachments/assets/60ae6e66-78ae-4775-9a32-8e0c7311e243)

**ecuaciones**

$$
q_1 = \frac{h_1}{r_1} , A_1 \frac{d h_1}{dt} = q_i - q_1
$$

**despejamos h1**

$$
h_1 = q_1 R_1
$$

**remplazamos en la ecuacion**

*  <a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=\( A_1 \frac{dh_1}{dt} = q_i - q_1 \)"><img src="http://www.alciro.org/cgi/tex.cgi?\( A_1 \frac{dh_1}{dt} = q_i - q_1 \)" title="\( A_1 \frac{dh_1}{dt} = q_i - q_1 \)" border="0" /></a>

eso quedaria como:

$$
R_1 A_1 \frac{dq_1}{dt} = q_i - q_1
$$

para el tanque 2 
se aplican las mismas ecuaciones 

**ecuaciones**

$$
q_2 = \frac{h_2}{r_2} , A_2 \frac{d h_2}{dt} = q_1 - q_2
$$

para esta ecuacion no ahi que despejar (h2) solo se remplaza (q2) directamente en la la otra ecuacion 

**remplazamos**

$$
A_2 \frac{dq_2}{dt} = q_1 - \frac{ h_2}{r_2}
$$

**despejamos q1**

$$
q_1 = A_2 \frac{dq_2}{dt} + \frac{h_2}{r_2}
$$

**derivamos  q1**

$$
\frac{dq_1}{dt} = A_2 \frac{d^2 q_2}{dt^2} + \frac{dh_2}{dt} + \frac{1}{R_2}
$$

**remplazamos en la siguiente ecuacion** 

$$
R_1 A_1 \frac{dq_1}{dt} = q_i - q_1
$$

quedaria: 

$$
A_1 k_1 \left[ A_2 \frac{d^2 q_2}{dt^2} + \frac{dh_2}{dt} \right] = q_i - \left[ A_2 \frac{dq_2}{dt} + \frac{h_2}{R_2} \right]
$$

-----------------------------------------------------------------

### 💡 Ejemplo 2: 2 tamques interconectados 

![image](https://github.com/user-attachments/assets/f0bc1ad3-4721-4ba2-a74a-25b46bff89b6)

para este sistema tendremos  escuciones 

1. tanque 1 

$$
q_1 = \frac{h_1 - h_2}{R_1} , A_1 \frac{dh_1}{dt} = (q_i - q_1)
$$

2. tanque 2 

$$
q_2 = \frac{h_2}{R_2} , A_2 \frac{dh_2}{dt} = (q_1 - q_2)
$$

**despejamos h2**

$$
h_2 = q_2 R_2
$$

**despejamos q1** 

$$
q_1 = A_2 \frac{dh_2}{dt} + q_2
$$

**remplazamos h2 en la ecuacion q1**


$$
q_1 = A_2 R_2 \frac{dq_2}{dt} + q_2
$$

**remplazamos q1 en la siguiente ecuacion**

$$
A_1 \frac{dh_1}{dt} = (q_i - q_1)
$$

**nos daria** 

$$
A_1 \frac{dh_1}{dt} = q_i - \left( A_2 R_2 \frac{dq_2}{dt} + q_2 \right)
$$


**despues depejamos h1**

$$
q_1 = \frac{h_1 - h_2}{R_1}
$$

 **daria esto**

$$
h_1 = q_1 R_1 + h_2
$$

**despejamos h2 en la escuaion**

$$
q_2 = \frac{h_2}{r_2}
$$
**daria**
$$
h_2 = q_2 R_2
$$

**remplazamos q1 y h2  en la ecuacion**

$$
h_1 = \left( A_2 R_2 \frac{dq_2}{dt} + q_2 \right) R_1 + q_2 R_2
$$

**derivamos h1 y remplazamos en la siguiente ecuacion**

$$
A_1 \frac{dh_1}{dt} = q_i - \left( A_2 R_2 \frac{dq_2}{dt} + q_2 \right)
$$

**daria**

$$
A_1 \frac{d}{dt} \left( R_1 \left( R_2 A_2 \frac{dq_2}{dt} + q_2 \right) + R_2 q_2 \right) = \left( q_i - R_2 A_2 \frac{dq_2}{dt} + q_2 \right)
$$

para finalizar depejamos qi

**despejando qi**

$$
 A_1 R_1 R_2 A_2 \frac{d^2 q_2}{dt^2} + (A_1 R_1 + A_1 R_2 + R_2 A_2) \frac{dq_2}{dt} - q_2 = q_i
$$

----------------------------
### 📚 Ejercicio 2

**modelo con h2 de salida**

![image](https://github.com/user-attachments/assets/ea24cc11-22fa-45f0-acf0-137198653201)

**ecuaciones**

**ecuacion 1**

$$
q_1 = \frac{h_1 - h_2}{R_1}  
$$

**ecuacion 2**

$$
q_2 = \frac{h_2}{R_2} 
$$

**ecuacion 3**

$$
A_1 \frac{dh_1}{dt} = (q_i - q_1)
$$

**ecuacion 4**

$$
A_2 \frac{dh_2}{dt} = (q_1 - q_2)
$$

------------------------------------

**reamplazamos q2 en la ecucion 4 y despejamos q1**

$$
A_2 \frac{dh_2}{dt} + \frac{h_2}{R_2} = q_{1}
$$

**en la ecuacion 3 reamplazamos q1**

$$
A_1 \frac{dh_1}{dt} = q_i - A_2 \frac{dh_2}{dt} - \frac{h_2}{R_2}
$$

**en la ecuacion 1 depejamos h1**

$$
h_1 = q_1 R_1 + h_2
$$

**remplazamos q1**

$$
h_1 = \left( A_2 \frac{dh_2}{dt} + \frac{h_2}{R_2} \right) R_1 + h_2
$$


$$
h_1 = R_1 A_2 \frac{dh_2}{dt} + h_2 \frac{R_1}{R_2} + h_2
$$

**derivamos h1**

$$
\frac{dh_1}{dt} = R_1 A_2 \frac{d^2 h_2}{dt^2} + \frac{dh_2}{dt} \frac{R_1}{R_2} + \frac{dh_2}{dt}
$$

**remplazamos la derivada de h1 y despejamos qi en la siguiente ecuacion**

$$
A_1 \frac{dh_1}{dt} = q_i - A_2 \frac{dh_2}{dt} - \frac{h_2}{R_2}
$$

**daria lo siguiente**

$$
A_1 \left( R_1 A_2 \frac{d^2 h_2}{dt^2} + \frac{dh_2}{dt} \frac{R_1}{R_2} + \frac{dh_2}{dt} \right) + A_2 \frac{dh_2}{dt} - \frac{h_2}{R_2} = q_i
$$


$$
A_1 R_1 A_2 \frac{d^2 h_2}{dt^2} + A_1 \frac{dh_2}{dt} \frac{R_1}{R_2} + A_1 \frac{dh_2}{dt} + A_2 \frac{dh_2}{dt} - \frac{h_2}{R_2} = q_i
$$

$$
A_1 R_1 A_2 \frac{d^2 h_2}{dt^2} + \left( A_1 \frac{R_1}{R_2} + A_1 + A_2 \right) \frac{dh_2}{dt} - \frac{h_2}{R_2} = q_i
$$

--------------------------------------------

### referencias 

file:///C:/Users/ESTACION/Downloads/6.%20Sistemas%20hidr%C3%A1ulicos%20%20y%20t%C3%A9rmicos.pdf

https://www.youtube.com/watch?v=7uI9Xfn_BME

https://controlautomaticoeducacion.com/analisis-de-sistemas/tanques-en-serie/

