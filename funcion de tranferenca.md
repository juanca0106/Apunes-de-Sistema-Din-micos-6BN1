# CORTE 3 
## clase de Función de transferencia
### 📅 **Curso:** sistemas dinamicos 
### 👨‍🏫 **Profesor:** Ing. Jorge Eduardo Cote Ballesteros
### 🧑‍🎓 **Semestre:** Sexto (2025)
### 🧑‍🎓 ** estudiantes** juan camilo cruz quintana,daniel corredor peña,Joan Sebastian Rojas.
------------------------------------------------------------------------
>* 🔑 **Función de transferencia**:
Una función de transferencia es una herramienta matemática usada principalmente en ingeniería y sistemas de control para describir cómo un sistema responde a una entrada.

**Definición básica:**
Una función de transferencia es la relación entre la salida y la entrada de un sistema lineal e invariante en el tiempo, expresada en el dominio de Laplace. Se representa como:

![image](https://github.com/user-attachments/assets/8c5ecb96-de0d-4918-81b1-d73b3a0ae806)

Donde:
G(s): es la función de transferencia.
Y(s): es la transformada de Laplace de la salida.
U(s): es la transformada de Laplace de la entrada.
s: es la variable compleja de Laplace.

**¿Para qué se usa?**
* Para analizar el comportamiento dinámico de un sistema (respuestas en el tiempo y en frecuencia).

* Para diseñar controladores (como PID).

* Para estudiar la estabilidad del sistema.

>* 🔑𝑇𝑜𝑑𝑎𝑠 𝑙𝑎𝑠 𝑐𝑜𝑛𝑑𝑖𝑐𝑖𝑜𝑛𝑒𝑠 𝑖𝑛𝑖𝑐𝑎𝑙𝑒𝑠 𝑑𝑒 𝑙𝑎 𝑒𝑐𝑢𝑎𝑐𝑖ó𝑛 𝑑𝑖𝑓𝑒𝑟𝑒𝑛𝑐𝑖𝑎𝑙 𝑠𝑜𝑛 𝑖𝑔𝑢𝑎𝑙𝑒𝑠 𝑎 0.
>* 𝑂𝐽𝑂: 𝐸𝑠𝑡𝑜 𝑠ó𝑙𝑜 𝑎𝑝𝑙𝑖𝑐𝑎 𝑐𝑢𝑎𝑛𝑑𝑜 𝑠𝑒 𝑣𝑎𝑛 𝑎 ℎ𝑎𝑐𝑒𝑟 𝑓𝑢𝑛𝑐𝑖𝑜𝑛𝑒𝑠 𝑑𝑒 𝑡𝑟𝑎𝑛𝑠𝑓𝑒𝑟𝑒𝑛𝑐𝑖𝑎, 𝑒𝑛 𝑒𝑙 𝑐𝑎𝑠𝑜 𝑑𝑒 𝑞𝑢𝑒𝑟𝑒𝑟 𝑠𝑜𝑙𝑢𝑐𝑖𝑜𝑛𝑎𝑟 𝑙𝑎 𝑒𝑐𝑢𝑎𝑐𝑖ó𝑛 𝑑𝑖𝑓𝑒𝑟𝑒𝑛𝑐𝑖𝑎𝑙 𝑠𝑖 𝑠𝑜𝑛 𝑛𝑒𝑐𝑒𝑠𝑎𝑟𝑖𝑎𝑠 𝑙𝑎𝑠 𝑐𝑜𝑛𝑑𝑖𝑐𝑖𝑜𝑛𝑒𝑠 𝑖𝑛𝑖𝑐𝑖𝑎𝑙𝑒𝑠 𝑦 𝑛𝑜 𝑛𝑒𝑐𝑒𝑠𝑎𝑟𝑖𝑎𝑚𝑒𝑛𝑡𝑒 𝑠𝑜𝑛 0.

### Clasificación de las funciones de transferencia

* Una función de transferencia se puede expresar como:

![image](https://github.com/user-attachments/assets/4bc7ee32-7dca-4667-b830-2ccd1bea86c4)

* Donde N(s) Y D(s) son polinomios en la variable “s”
* Si denominamos n al grado del polinomio del numerador
* Si denominamos m al grado del polinomio del denominador
* Se tienen 3 casos posibles:
1. n>m impropia
2. m>n estrictamente propia
3. n=m bipropia

💡Ejemplo 1:

* impropia
  
$$
s^2 + 1
$$

* Estrictamente propia
  
$$
\frac{1}{s + 1} 
$$

* bipropia
  
$$
2 
$$

* impropia
  
$$
\frac{s^2 - 1}{s + 1}
$$


* bipropia
  
$$
\frac{s - 1}{s + 1}
$$

---------------------

### Zeros de una función de transferencia

* Si se iguala N(s) a 0 se obtienen los valores de “s” que cumplen con la condición
* Si el numerador se hace 0 toda la función de
transferencia se vuelve cero de ahí el nombre para estos valores de “s”
* Estos valores pueden ser reales o complejos por lo tanto se pueden ubicar en un plano cartesiano

**Hallar los zeros de una función de transferencia** 

$$
F(s) = \frac{Y(s)}{B(s)} = \frac{3s - 1}{s^2 + 3s + 2} = \frac{A(s)}{D(s)} 
$$

>* 🔑 **F= G, A=N, U=B**

A(s)=0 

D(S) ---> 3s+1 = 0

$$
s= \frac{1}{3}
$$

>* s es un numero complejo

**Ubicación de zeros**

![image](https://github.com/user-attachments/assets/6edd122a-3adc-41f2-81f5-b0ff76af9640)

----------------------------------------

💡Ejemplo 2: Hallar los zeros para la siguiente función de transferencia:

$$
G(s) = \frac{s^2 + 4s + 1}{s^4 + 3s^3 + 3s^2 + s + 2}
$$

**Para encontrar los ceros, resolvemos la ecuación del numerador:**

$$
s^2 + 4s + 1 = 0
$$

**Usamos la fórmula general para ecuaciones cuadráticas:**

$$
s = \frac{-4 \pm \sqrt{4^2 - 4(1)(1)}}{2(1)} = \frac{-4 \pm \sqrt{16 - 4}}{2} = \frac{-4 \pm \sqrt{12}}{2}
$$

$$
s = \frac{-4 \pm 2\sqrt{3}}{2} = -2 \pm \sqrt{3}
$$

**Por lo tanto, los ceros de la función de transferencia son:**

$$
s_1 = -2 + \sqrt{3}, \quad s_2 = -2 - \sqrt{3}
$$

**graficado en un plano complejo**

![image](https://github.com/user-attachments/assets/225f32b8-3dcc-4ebd-8d6c-63aae630077b)

Aquí tienes la gráfica con solo los ceros de la función de transferencia. Los ceros están ubicados en el eje real en:

$$
s_1 = -2 + \sqrt{3}, \quad s_2 = -2 - \sqrt{3}
$$

-----------------------------------------------------------------------

### Polos de una función de transferencia

* Si se iguala D(s) a 0 se obtienen los valores de “s” que cumplen con la condición
* Si el denominador se hace 0 toda la función de transferencia se vuelve infinito de ahí el nombre para estos valores de “s”
* Estos valores pueden ser reales o complejos por lo tanto se pueden ubicar en un plano cartesiano

**Hallar los polos de una función de transferencia**

$$
F(s) = \frac{Y(s)}{B(s)} = \frac{3s - 1}{s^2 + 3s + 2} = \frac{A(s)}{D(s)} 
$$

>* 🔑 **F= G, A=N, U=B**

**Identificamos el denominador:**

$$
A(s)= 0
$$

$$
D(s) = s^2 + 3s + 2
$$

**Resolviendo**

$$
D(s) = s^2 + 3s + 2 = 0 
$$

**Factorizando:**

$$
(s + 1)(s + 2) = 0
$$

**Por lo tanto, las raíces son:**

$$
s = -1, \quad s = -2
$$

**Ubicación de polosos**

![image](https://github.com/user-attachments/assets/2d626915-61ff-40da-9ef7-65506f465dd5)


**En general la ubicación de polos y zeros**

![image](https://github.com/user-attachments/assets/3eaddcdf-2a4c-4aa1-a8ed-b41a497badbe)


----------------------------------------

💡Ejemplo 2:
**Hallar los polos de la siguiente función de transferencia:**

$$
F(s) = \frac{s + 2}{(s + 3)(s^2 + 0.5s + 1)}
$$

**Para encontrar los polos, igualamos el denominador a cero:**

$$
(s + 3)(s^2 + 0.5s + 1) = 0
$$

**De aquí obtenemos dos partes:**
Polos reales:

$$
s + 3 = 0 \Rightarrow s = -3
$$

**Y:**
Polos complejos:

$$
s^2 + 0.5s + 1 = 0
$$

**Aplicamos la fórmula general:**

$$
s = \frac{-0.5 \pm \sqrt{(0.5)^2 - 4(1)(1)}}{2(1)} = \frac{-0.5 \pm \sqrt{-3.75}}{2}
$$

$$
s = -0.25 \pm j\frac{\sqrt{15}}{4}
$$

**Por lo tanto, los polos de la función son:**

$$
s = -3, \quad s = -0.25 \pm i\frac{\sqrt{15}}{4}
$$

**polos de la función de transferencia en el plano complejo**

![image](https://github.com/user-attachments/assets/9dc0a3b6-6bab-4fe7-9aa0-ffe7635d4317)





