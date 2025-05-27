# CORTE 3 
## clase de Sistemas de tanques
### 📅 **Curso:** sistemas dinamicos 
### 👨‍🏫 **Profesor:** Ing. Jorge Eduardo Cote Ballesteros
### 🧑‍🎓 **Semestre:** Sexto (2025)
### 🧑‍🎓 ** estudiantes** juan camilo cruz quintana,daniel corredor peña,Joan Sebastian Rojas.
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
### 💡 Ejemplo 1

![image](https://github.com/user-attachments/assets/4a283122-97a0-408c-9472-88a81e9dfb8a)

* 𝑞𝑖, 𝑞𝑜: 𝐹𝑙𝑢𝑗𝑜𝑠 𝑑𝑒 𝑒𝑛𝑡𝑟𝑎𝑑𝑎 𝑦 𝑠𝑎𝑙𝑖𝑑𝑎 𝑑𝑒 𝑙í𝑞𝑢𝑖𝑑o
* 𝑅1: 𝑅𝑒𝑠𝑖𝑠𝑡𝑒𝑛𝑐𝑖𝑎 𝑎𝑙 𝑓𝑙𝑢𝑗o
* 𝐴1: Á𝑟𝑒𝑎 𝑡𝑟𝑎𝑛𝑠𝑣𝑒𝑟𝑠𝑎𝑙 𝑑𝑒𝑙 𝑡𝑎𝑛𝑞𝑢e
* ℎ1: 𝑁𝑖𝑣𝑒𝑙 𝑑𝑒 𝑙í𝑞𝑢𝑖𝑑𝑜 𝑒𝑛 𝑒𝑙 𝑡𝑎𝑛𝑞𝑢e

 ## modelo de un tanque 
**Flujo de salida del tanque**

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=q_1 = \frac{h_1}{r_1}"><img src="http://www.alciro.org/cgi/tex.cgi?q_1 = \frac{h_1}{r_1}" title="q_1 = \frac{h_1}{r_1}" border="0" /></a>

esta ecuacion es analoga a la ley de ohm en electricidad: el flujo es proporcional a la "presion" cuanto mas alto este el nivel del lquidomayor sera el flujo de salida 

