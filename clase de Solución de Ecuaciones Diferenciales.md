# CORTE 2 
## clase de Solución de Ecuaciones Diferenciales
### 📅 **Curso:** sistemas dinamicos 
### 👨‍🏫 **Profesor:** Ing. Jorge Eduardo Cote Ballesteros
### 🧑‍🎓 **Semestre:** Sexto (2025)
### 🧑‍🎓 ** estudiantes** juan camilo cruz quintana y daniel corredor peña 

-----

>* 🔑 **Solución ecuaciones diferenciales**:
Un sistema dinámico es cualquier cosa que evoluciona con el tiempo y cuyo comportamiento puede describirse con ecuaciones (usualmente diferenciales).

💡 Ejemplos:
* Un resorte con masa (sistema masa-resorte-amortiguador)

  ![image](https://github.com/user-attachments/assets/4c5b5ece-787e-4149-ba5f-9912b63fdff2)

* El voltaje y corriente en un circuito RLC

![image](https://github.com/user-attachments/assets/4e0c3a40-15e3-449c-9a3b-dff242a68ef4)

* El movimiento de un robot

![image](https://github.com/user-attachments/assets/80ad7ec3-9b67-4f98-aefa-a0940f7c1f55)
------
## ✍️ Introducción

La solución de ecuaciones diferenciales mediante la transformada de Laplace permite convertir ecuaciones diferenciales ordinarias (EDO) en ecuaciones algebraicas más fáciles de resolver. Esta técnica es especialmente útil para sistemas lineales con condiciones iniciales conocidas.

---

## 1️⃣ Metodología General

Pasos para resolver una EDO con la transformada de Laplace:

1. Aplicar la transformada de Laplace a ambos lados de la ecuación.
2. Sustituir las condiciones iniciales dadas.
3. Despejar la función transformada \( X(s) \) o \( Y(s) \).
4. Aplicar la transformada inversa de Laplace para encontrar la solución en el dominio del tiempo.

---

## 2️⃣ Ejemplos Resueltos

### 💡 Ejemplo 1

**Ecuación:**

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=\ddot{x} + 3\dot{x} + 2x = 0, x(0)=a,\quad \dot{x}(0)=b"><img src="http://www.alciro.org/cgi/tex.cgi?\ddot{x} + 3\dot{x} + 2x = 0, x(0)=a,\quad \dot{x}(0)=b" title="\ddot{x} + 3\dot{x} + 2x = 0, x(0)=a,\quad \dot{x}(0)=b" border="0" /></a>

**Transformada de Laplace:**

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=\[\left[ s^2 X(s) - s x(0) - \dot{x}(0) \right] + 3\left[ s X(s) - x(0) \right] + 2X(s) = 0\]"><img src="http://www.alciro.org/cgi/tex.cgi?\[\left[ s^2 X(s) - s x(0) - \dot{x}(0) \right] + 3\left[ s X(s) - x(0) \right] + 2X(s) = 0\]" title="\[\left[ s^2 X(s) - s x(0) - \dot{x}(0) \right] + 3\left[ s X(s) - x(0) \right] + 2X(s) = 0\]" border="0" /></a>



**Reemplazando condiciones iniciales:**

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=\[\left[ s^2 X(s) - a s - b \right] + 3 \left[ s X(s) - a \right] + 2 X(s) = 0\]"><img src="http://www.alciro.org/cgi/tex.cgi?\[\left[ s^2 X(s) - a s - b \right] + 3 \left[ s X(s) - a \right] + 2 X(s) = 0\]" title="\[\left[ s^2 X(s) - a s - b \right] + 3 \left[ s X(s) - a \right] + 2 X(s) = 0\]" border="0" /></a>

**despejamos x**

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=(s^2 +3s + 2) X(s) = a s + b + 3a"><img src="http://www.alciro.org/cgi/tex.cgi?(s^2 +3s + 2) X(s) = a s + b + 3a" title="(s^2 + 3s + 2) X(s) = a s + b + 3a" border="0" /></a>

------
<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=\[X(s) = \frac{a s + b + 3a}{s^2 + 3s + 2} = \frac{a s + b + 3a}{(s + 1)(s + 2)} = \frac{2a + b}{s + 1} - \frac{a + b}{s + 2}\]"><img src="http://www.alciro.org/cgi/tex.cgi?\[X(s) = \frac{a s + b + 3a}{s^2 + 3s + 2} = \frac{a s + b + 3a}{(s + 1)(s + 2)} = \frac{2a + b}{s + 1} - \frac{a + b}{s + 2}\]" title="\[X(s) = \frac{a s + b + 3a}{s^2 + 3s + 2} = \frac{a s + b + 3a}{(s + 1)(s + 2)} = \frac{2a + b}{s + 1} - \frac{a + b}{s + 2}\]" border="0" /></a>

**Aplicando transformada inversa desde las tablas para Volver al dominio del tiempo**

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=
x(t) = \mathcal{L}^{-1} \{ X(s) \} = \mathcal{L}^{-1} \left\{ \frac{2a + b}{s + 1} \right\} - \mathcal{L}^{-1} \left\{ \frac{a + b}{s + 2} \right\}"><img src="http://www.alciro.org/cgi/tex.cgi?x(t) = \mathcal{L}^{-1} \{ X(s) \} = \mathcal{L}^{-1} \left\{ \frac{2a + b}{s + 1} \right\} - \mathcal{L}^{-1} \left\{ \frac{a + b}{s + 2} \right\}" title="x(t) = \mathcal{L}^{-1} \{ X(s) \} = \mathcal{L}^{-1} \left\{ \frac{2a + b}{s + 1} \right\} - \mathcal{L}^{-1} \left\{ \frac{a + b}{s + 2} \right\}" border="0" /></a>

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=
x(t) = (2a + b)e^{-t} - (a + b)e^{-2t} \quad (t \geq 0)"><img src="http://www.alciro.org/cgi/tex.cgi?x(t) = (2a + b)e^{-t} - (a + b)e^{-2t}\quad (t \geq 0)" title="
x(t) = (2a + b)e^{-t} - (a + b)e^{-2t} \quad (t \geq 0)" border="0" /></a>

---

### 💡 Ejemplo 2

**Ecuación:**

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=\ddot{x} + 2\dot{x} + 5x = 3,   x(0) = 0, \quad \dot{x}(0) = 0"><img src="http://www.alciro.org/cgi/tex.cgi?\ddot{x} + 2\dot{x} + 5x = 3,   x(0) = 0, \quad \dot{x}(0) = 0" title="\ddot{x} + 2\dot{x} + 5x = 3,   x(0) = 0, \quad \dot{x}(0) = 0" border="0" /></a>

**Transformada de laplace:**

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=s^2 X(s) + 2s X(s) + 5 X(s) = \frac{3}{s}"><img src="http://www.alciro.org/cgi/tex.cgi?s^2 X(s) + 2s X(s) + 5 X(s) = \frac{3}{s}" title="s^2 X(s) + 2s X(s) + 5 X(s) = \frac{3}{s}" border="0" /></a>

**Factorizamos:**

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=X(s) = \frac{3}{s(s^2 + 2s + 5)}"><img src="http://www.alciro.org/cgi/tex.cgi?X(s) = \frac{3}{s(s^2 + 2s + 5)}" title="X(s) = \frac{3}{s(s^2 + 2s + 5)}" border="0" /></a>

**Fracciones parciales**

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=\frac{3}{s(s^2 + 2s + 5)} = \frac{A}{s} + \frac{Bs + C}{s^2 + 2s + 5}"><img src="http://www.alciro.org/cgi/tex.cgi?\frac{3}{s(s^2 + 2s + 5)} = \frac{A}{s} + \frac{Bs + C}{s^2 + 2s + 5}" title="\frac{3}{s(s^2 + 2s + 5)} = \frac{A}{s} + \frac{Bs + C}{s^2 + 2s + 5}" border="0" /></a>

**Sistema de ecuaciones para encontrar A, B, C** 

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=A + B =0 \\2A + C = 0 \\5A = 3"><img src="http://www.alciro.org/cgi/tex.cgi?A + B = 0 \\2A + C = 0 \\5A = 3" title="A + B = 0 \\2A + C = 0 \\5A = 3" border="0" /></a>

**Solución** 

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=A =\frac{3}{5}, \\B = -\frac{3}{5}, \\C = -\frac{6}{5}"><img src="http://www.alciro.org/cgi/tex.cgi?A = \frac{3}{5}, \\B = -\frac{3}{5}, \\C = -\frac{6}{5}" title="A = \frac{3}{5}, \\B = -\frac{3}{5}, \\C = -\frac{6}{5}" border="0" /></a>

**Sustituyendo** 

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=X(s) = \frac{3}{5} \cdot \frac{1}{s} - \frac{3}{5} \cdot \frac{s}{s^2 + 2s + 5} - \frac{6}{5} \cdot \frac{1}{s^2 + 2s + 5}"><img src="http://www.alciro.org/cgi/tex.cgi?X(s) = \frac{3}{5} \cdot \frac{1}{s} - \frac{3}{5} \cdot \frac{s}{s^2 + 2s + 5} - \frac{6}{5} \cdot \frac{1}{s^2 + 2s + 5}" title="X(s) = \frac{3}{5} \cdot \frac{1}{s} - \frac{3}{5} \cdot \frac{s}{s^2 + 2s + 5} - \frac{6}{5} \cdot \frac{1}{s^2 + 2s + 5}" border="0" /></a>

**Completando el cuadrado**

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=s^2 + 2s + 5 = (s + 1)^2 + 2^2"><img src="http://www.alciro.org/cgi/tex.cgi?s^2 + 2s + 5 = (s + 1)^2 + 2^2" title="s^2 + 2s + 5 = (s + 1)^2 + 2^2" border="0" /></a>

**Entonces**

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=X(s) = \frac{3}{5} \cdot \frac{1}{s} - \frac{3}{5} \cdot \frac{s + 1}{(s + 1)^2 + 2^2} - \frac{9}{5} \cdot \frac{1}{(s + 1)^2 + 2^2}"><img src="http://www.alciro.org/cgi/tex.cgi?X(s) = \frac{3}{5} \cdot \frac{1}{s} - \frac{3}{5} \cdot \frac{s + 1}{(s + 1)^2 + 2^2} - \frac{9}{5} \cdot \frac{1}{(s + 1)^2 + 2^2}" title="X(s) = \frac{3}{5} \cdot \frac{1}{s} - \frac{3}{5} \cdot \frac{s + 1}{(s + 1)^2 + 2^2} - \frac{9}{5} \cdot \frac{1}{(s + 1)^2 + 2^2}" border="0" /></a>

**Transformada inversa de Laplace**
Usamos identidades:

![image](https://github.com/user-attachments/assets/9ebda408-8cc3-4bf7-aa79-15f6d3d9255d)

**Aplicamos y resultado final**

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=x(t) = \frac{3}{5} - \frac{3}{5} e^{-t} \cos(2t) - \frac{9}{10} e^{-t} \sin(2t}"><img src="http://www.alciro.org/cgi/tex.cgi?x(t) = \frac{3}{5} - \frac{3}{5} e^{-t} \cos(2t) - \frac{9}{10} e^{-t} \sin(2t}" title="x(t) = \frac{3}{5} - \frac{3}{5} e^{-t} \cos(2t) - \frac{9}{10} e^{-t} \sin(2t}" border="0" /></a>

---

## 3️⃣ Ejercicios Adicionales

### 📚 Ejercicio 1

**Ecuación:**

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=\ddot{x} + 4x = 0, x(0) = 5,  \dot{x}(0) = 0"><img src="http://www.alciro.org/cgi/tex.cgi?\ddot{x} + 4x = 0, x(0) = 5,  \dot{x}(0) = 0" title="\ddot{x} + 4x = 0, x(0) = 5,  \dot{x}(0) = 0" border="0" /></a>

**Aplicar la transformada de Laplace**

![image](https://github.com/user-attachments/assets/895c11b7-5171-4acc-b2af-f8059797d5f1)

Sustituyendo:

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=s^2 X(s) - 5s + 4 X(s) = 0"><img src="http://www.alciro.org/cgi/tex.cgi?s^2 X(s) - 5s + 4 X(s) = 0" title="s^2 X(s) - 5s + 4 X(s) = 0" border="0" /></a>

**Factorizar y despejar X(s)**

Agrupamos términos con X(s):

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=X(s)(s^2 + 4) = 5s \\
= X(s) = \frac{5s}{s^2 + 4}"><img src="http://www.alciro.org/cgi/tex.cgi?X(s)(s^2 + 4) = 5s \\= X(s) = \frac{5s}{s^2 + 4}" title="X(s)(s^2 + 4) = 5s \\ = X(s) = \frac{5s}{s^2 + 4}" border="0" /></a>

**Transformada inversa de Laplace**
Sabemos que: 

![image](https://github.com/user-attachments/assets/b797632b-6513-497c-8dbc-9d782dde3769)

Entonces el resultado final es:  

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=x(t) = 5 \cos(2t)"><img src="http://www.alciro.org/cgi/tex.cgi?x(t) = 5 \cos(2t)" title="x(t) = 5 \cos(2t)" border="0" /></a>


---

### 📚 Ejercicio 2

**Ecuación:**

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=2\ddot{x} + 2\dot{x} + x = 1,  x(0) = 0, \dot{x}(0) = 2"><img src="http://www.alciro.org/cgi/tex.cgi?2\ddot{x} + 2\dot{x} + x = 1,  x(0) = 0, \dot{x}(0) = 2" title="2\ddot{x} + 2\dot{x} + x = 1,  x(0) = 0, \dot{x}(0) = 2" border="0" /></a>

**Aplicar la transformada de Laplace**

![image](https://github.com/user-attachments/assets/9a7b6513-12d4-4b3d-8646-df7867ba0a47)

Sustituyendo en la ecuación usando las condiciones:

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=2(s^2 X(s) - 2) + 2s X(s) + X(s) = \frac{1}{s}"><img src="http://www.alciro.org/cgi/tex.cgi?2(s^2 X(s) - 2) + 2s X(s) + X(s) = \frac{1}{s}" title="2(s^2 X(s) - 2) + 2s X(s) + X(s) = \frac{1}{s}" border="0" /></a>

**Agrupar términos y despejar X(s)**

![image](https://github.com/user-attachments/assets/5869f985-7572-4bd0-b7fe-63080cca6902)

Factorizamos:

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=X(s)(2s^2 + 2s + 1) = \frac{1}{s} + 4 \\=X(s) = \frac{\frac{1}{s} + 4}{2s^2 + 2s + 1}"><img src="http://www.alciro.org/cgi/tex.cgi?X(s)(2s^2 + 2s + 1) = \frac{1}{s} + 4 \\=X(s) = \frac{\frac{1}{s} + 4}{2s^2 + 2s + 1}" title="X(s)(2s^2 + 2s + 1) = \frac{1}{s} + 4 \\=X(s) = \frac{\frac{1}{s} + 4}{2s^2 + 2s + 1}" border="0" /></a>

**Expresamos como fracciones parciales**

la expresion: 

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=X(s) = \frac{\frac{1}{s} + 4}{2(s^2 + s + \frac{1}{2})}"><img src="http://www.alciro.org/cgi/tex.cgi?X(s) = \frac{\frac{1}{s} + 4}{2(s^2 + s + \frac{1}{2})}" title="X(s) = \frac{\frac{1}{s} + 4}{2(s^2 + s + \frac{1}{2})}" border="0" /></a>

Completa el cuadrado en el denominador:

![image](https://github.com/user-attachments/assets/a75ed074-1078-49e5-bf1a-9a8ec54e0398)

entonces: 

![image](https://github.com/user-attachments/assets/6d7ac87e-bbe0-4ed5-a456-5fa30f3354a1).


## **codigos de matlab** 

**ejemplo 1.**

![image](https://github.com/user-attachments/assets/b857fcb2-244b-4e9a-807d-1623baf609b7)

**ejemplo 2**

![image](https://github.com/user-attachments/assets/a46b21e4-db88-4bd8-98b6-085c66c5a623)


![image](https://github.com/user-attachments/assets/763c3aa7-8ba5-4399-916a-ef8188f9caf4)


**ejercicio 1**

![image](https://github.com/user-attachments/assets/499441fb-4265-4d0b-affc-8144d5d86883)

**ejercicio 2**

![image](https://github.com/user-attachments/assets/5395db1f-1b51-44ce-aa3d-15bf4f9c43e9)
----
**📌 Conclusiones**
* Las ecuaciones diferenciales son fundamentales para modelar sistemas que cambian con el tiempo en distintas áreas del conocimiento.

* Existen métodos analíticos y numéricos que permiten resolver estas ecuaciones según sus características.

* La solución de una ecuación diferencial ayuda a predecir y entender el comportamiento de un sistema real.

* Comprender estas herramientas es clave para analizar y controlar sistemas dinámicos de manera eficiente.












      
      




          




   
    




  





