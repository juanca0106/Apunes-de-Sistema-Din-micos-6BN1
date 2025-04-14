# CORTE 2 
## clase de Sistemas dinamicos 
### 📅 **Curso:** sistemas dinamicos 
### 👨‍🏫 **Profesor:** Ing. Jorge Eduardo Cote Ballesteros
### 🧑‍🎓 **Semestre:** Sexto (2025)
### 🧑‍🎓 ** estudiantes** juan camilo cruz quintana y daniel corredor peña 
---

## 1. Introducción a los Sistemas Dinámicos

Un sistema dinámico describe la evolución de variables físicas en función del tiempo, respondiendo a estímulos de entrada y condiciones iniciales.

**Clasificación de sistemas:**
- Mecánicos  
- Eléctricos  
- Hidráulicos  
- Neumáticos  
- Térmicos  
- Combinados

## 2. Principio General de Modelamiento

El modelado se basa en la conservación de masa o energía:

![image](https://github.com/user-attachments/assets/3ae81485-d016-40ad-abd9-1d010e8b47ac)

💡Ejemplos: 
* Masa: 
<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=\frac{dM}{dt} = M_{\text{in}} - M_{\text{out}}"><img src="http://www.alciro.org/cgi/tex.cgi?\frac{dM}{dt} = M_{\text{in}} - M_{\text{out}}" title="\frac{dM}{dt} = M_{\text{in}} - M_{\text{out}}" border="0" /></a>

* energia:
<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=\frac{dE}{dt} = E_{\text{in}} - E_{\text{out}}"><img src="http://www.alciro.org/cgi/tex.cgi?\frac{dE}{dt} = E_{\text{in}} - E_{\text{out}}" title="\frac{dE}{dt} = E_{\text{in}} - E_{\text{out}}" border="0" /></a>

## 3. Elementos Mecánicos Básicos
### 3.1 Resorte
Cumple la Ley de Hooke:

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=F_R = k x "><img src="http://www.alciro.org/cgi/tex.cgi?F_R = k x" title="F_R = k x" border="0" /></a>

- <a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=F_R
"><img src="http://www.alciro.org/cgi/tex.cgi?F_R" title="F_R" border="0" /></a> = Fuerza del resorte 
- <a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=k"><img src="http://www.alciro.org/cgi/tex.cgi?k" title="k" border="0" /></a> = Constante de elasticidad  
- <a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=x"><img src="http://www.alciro.org/cgi/tex.cgi?x" title="x" border="0" /></a>  = Desplazamiento

  ![image](https://github.com/user-attachments/assets/ffbf2f2f-a823-4c9d-a2e7-f11129eb7502)

### 3.2 Amortiguador 

Fuerza proporcional a la velocidad:

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=F_F = b \frac{dx}{dt}"><img src="http://www.alciro.org/cgi/tex.cgi?F_F = b \frac{dx}{dt}" title="F_F = b \frac{dx}{dt}
" border="0" /></a>

donde: 

- <a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=\( F_F \)"><img src="http://www.alciro.org/cgi/tex.cgi?\( F_F \)" title="\( F_F \)" border="0" /></a> = Fuerza de fricción viscosa

- <a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=\( b \)"><img src="http://www.alciro.org/cgi/tex.cgi?\( b \)" title="\( b \)" border="0" /></a> = Coeficiente de fricción
  
- <a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=\( \frac{dx}{dt} \) "><img src="http://www.alciro.org/cgi/tex.cgi?\( \frac{dx}{dt} \)" title="\( \frac{dx}{dt} \) " border="0" /></a> = Velocidad


### 3.3 Fricción en Seco
Tipos principales:
- Fricción estática:

  ![image](https://github.com/user-attachments/assets/e043a854-a4f2-4ac8-b9fe-858b8d987969)


- Fricción de deslizamiento

  ![image](https://github.com/user-attachments/assets/bb6d5bba-00ae-4d6c-b646-79e1643595da)

- Fricción de rodamiento

  ![image](https://github.com/user-attachments/assets/08ba0033-9457-444c-a09f-fba8a3e9286f)

> En general la fuerza se opone al movimiento, su modelo depende de la naturaleza de las superficies.

------

## 4. Sistema Masa-Resorte-Amortiguador

Modelo dinámico clásico:

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=m \frac{d^2y(t)}{dt^2} + b \frac{dy(t)}{dt} + k y(t) = u(t)"><img src="http://www.alciro.org/cgi/tex.cgi?m \frac{d^2y(t)}{dt^2} + b \frac{dy(t)}{dt}+k y(t) = u(t)" title="m \frac{d^2y(t)}{dt^2} + b \frac{dy(t)}{dt} + k y(t) = u(t)" border="0" /></a>

Donde:  
- \( m \) = Masa  
- \( b \) = Coeficiente de fricción viscosa  
- \( k \) = Constante de resorte  
- \( u(t) \) = Fuerza de entrada

![image](https://github.com/user-attachments/assets/c588a16d-6bb9-4a2b-8553-b81e3eb68ab7)

diagrama de cuerpo libre.

![image](https://github.com/user-attachments/assets/e45db963-875a-44ec-80be-e1fbb6bbb43d)

modelo matematico
![image](https://github.com/user-attachments/assets/925c0d5e-88d8-4ff0-a6ae-7110b96fa6a7)

💡 Ejemplo 1: Suspensión de un Automóvil
Encontrarel modelomatemáticopara el Sistema que representala suspensiónde un automóvil: 

![image](https://github.com/user-attachments/assets/abb0ec1f-e959-4480-bf45-53e806665cc7)

solucion:
diagrama de cuerpo libre: 

![image](https://github.com/user-attachments/assets/3305a90e-a41f-49a5-b0cc-8e47f9a7bbb5)

No se tiene en cuenta el efecto de la fuerza de gravedad, si se
considera el desplazamiento desde la posición de equilibrio
puesto que en ese caso:

𝑘𝛿 = 𝑚𝑔

Y si se considera la sustitución:

𝑦 = 𝑥 + 𝛿

El término correspondiente a la fuerza de gravedad desaparece

**Vibración libre**
-Aún aplicando entrada durante un intervalo de tiempo definido es posible provocar un comportamiento oscilatorio en la variable de salida del sistema

-Por ejemplo, en el caso de la suspensión si se aplica una fuerza constante durante un intervalo corto de tiempo y se retira dicho estímulo el sistema tiende a vibrar

-Este movimiento periódico se conoce como vibración libre

💡 Ejemplo 2: 
Simular la solución de este sistema sabiendo:

Parámetros:
- \( k = 22500 \, \frac{N}{m} \)  
- \( b = 2000 \, \frac{Ns}{m} \)  
- \( M = 300 \, kg \)

Si se suben dos personas de \( 80 \, kg \) cada una, la masa total es:

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=M_{\text{total}} = 300 + 2(80) = 460 \, kg"><img src="http://www.alciro.org/cgi/tex.cgi?M_{\text{total}} = 300 + 2(80) = 460 \, kg" title="M_{\text{total}} = 300 + 2(80) = 460 \, kg" border="0" /></a>

 ---------
 ## 5. Sistemas Acoplados

Dos masas unidas por resortes y amortiguadores.

![image](https://github.com/user-attachments/assets/60fe9faa-9584-4e3f-a490-9a38a7eb4f0f)

diagrama de cuerpo libre: 

![image](https://github.com/user-attachments/assets/7c03c3ee-f372-475a-ae8b-a319e196156c)


### Para la masa \( m_1 \):
𝑢 − 𝐹𝑅1 − 𝐹𝑅2 − 𝐹𝐹 = 𝑚1 ∗ 𝑎𝑚1

𝐿𝑎 𝑑𝑖𝑠𝑡𝑎𝑛𝑐𝑖𝑎 𝑑𝑒 𝑒𝑙𝑜𝑛𝑔𝑎𝑐𝑖ó𝑛 𝑑𝑒𝑙 𝑟𝑒𝑠𝑜𝑟𝑡𝑒 2 𝑑𝑒𝑝𝑒𝑛𝑑𝑒 𝑑𝑒𝑙 𝑚𝑜𝑣𝑖𝑚𝑖𝑒𝑡𝑜 𝑑𝑒 𝑎𝑚𝑏𝑎𝑠 𝑚𝑎𝑠𝑎𝑠 𝐿𝑎 𝑣𝑒𝑙𝑜𝑐𝑖𝑑𝑎𝑑 𝑑𝑒𝑙 𝑒𝑚𝑏𝑜𝑙𝑜 𝑑𝑒𝑙 𝑎𝑚𝑜𝑟𝑡𝑖𝑔𝑢𝑎𝑑𝑜𝑟 𝑑𝑒𝑙 𝑟𝑒𝑠𝑜𝑟𝑡𝑒 2 𝑑𝑒𝑝𝑒𝑛𝑑𝑒 𝑑𝑒𝑙 𝑚𝑜𝑣𝑖𝑚𝑖𝑒𝑡𝑜 𝑑𝑒 𝑎𝑚𝑏𝑎𝑠 𝑚𝑎𝑠𝑎𝑠

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=u(t) - k_1 x_1(t) - k_2(x_1(t) - x_2(t)) - b \frac{d(x_1(t) - x_2(t))}{dt} = m_1 \frac{d^2 x_1(t)}{dt^2}"><img src="http://www.alciro.org/cgi/tex.cgi?u(t) - k_1 x_1(t) - k_2(x_1(t) - x_2(t)) - b \frac{d(x_1(t) - x_2(t))}{dt} = m_1 \frac{d^2 x_1(t)}{dt^2}" title="u(t) - k_1 x_1(t) - k_2(x_1(t) - x_2(t)) - b \frac{d(x_1(t) - x_2(t))}{dt} = m_1 \frac{d^2 x_1(t)}{dt^2}" border="0" /></a>

  ### Para la masa \( m_2 \):

  𝐹𝑅2 + 𝐹𝐹 − 𝐹𝑅3 = 𝑚2 ∗ 𝑎𝑚2

𝐿𝑎 𝑑𝑖𝑠𝑡𝑎𝑛𝑐𝑖𝑎 𝑑𝑒 𝑒𝑙𝑜𝑛𝑔𝑎𝑐𝑖ó𝑛 𝑑𝑒𝑙 𝑟𝑒𝑠𝑜𝑟𝑡𝑒 2 𝑑𝑒𝑝𝑒𝑛𝑑𝑒 𝑑𝑒𝑙 𝑚𝑜𝑣𝑖𝑚𝑖𝑒𝑡𝑜 𝑑𝑒 𝑎𝑚𝑏𝑎𝑠 𝑚𝑎𝑠𝑎𝑠 𝐿𝑎 𝑣𝑒𝑙𝑜𝑐𝑖𝑑𝑎𝑑 𝑑𝑒𝑙 𝑒𝑚𝑏𝑜𝑙𝑜 𝑑𝑒𝑙 𝑎𝑚𝑜𝑟𝑡𝑖𝑔𝑢𝑎𝑑𝑜𝑟 𝑑𝑒𝑙 𝑟𝑒𝑠𝑜𝑟𝑡𝑒 2 𝑑𝑒𝑝𝑒𝑛𝑑𝑒 𝑑𝑒𝑙 𝑚𝑜𝑣𝑖𝑚𝑖𝑒𝑡𝑜 𝑑𝑒 𝑎𝑚𝑏𝑎𝑠 𝑚𝑎𝑠𝑎𝑠

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=k_2(x_1(t) - x_2(t)) + b \frac{d(x_1(t) - x_2(t))}{dt} - k_3 x_2(t) = m_2 \frac{d^2 x_2(t)}{dt^2}"><img src="http://www.alciro.org/cgi/tex.cgi?k_2(x_1(t) - x_2(t)) + b \frac{d(x_1(t) - x_2(t))}{dt} - k_3 x_2(t) = m_2 \frac{d^2 x_2(t)}{dt^2}" title="k_2(x_1(t) - x_2(t)) + b \frac{d(x_1(t) - x_2(t))}{dt} - k_3 x_2(t) = m_2 \frac{d^2 x_2(t)}{dt^2}" border="0" /></a>
----------

## 6. Sistemas Rotacionales
Movimiento angular análogo al traslacional:

- Torsión (Resorte):  

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=T_R = k \theta"><img src="http://www.alciro.org/cgi/tex.cgi?T_R = k \theta" title="T_R = k \theta" border="0" /></a>

- Amortiguador:

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=T_F = b \frac{d\theta}{dt}"><img src="http://www.alciro.org/cgi/tex.cgi?T_F = b \frac{d\theta}{dt}" title="T_F = b \frac{d\theta}{dt}" border="0" /></a>

- Dinámica:  

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=T(t) - T_R - T_F = J \frac{d^2\theta}{dt^2}"><img src="http://www.alciro.org/cgi/tex.cgi?T(t) - T_R - T_F = J \frac{d^2\theta}{dt^2}" title="T(t) - T_R - T_F = J \frac{d^2\theta}{dt^2}" border="0" /></a> 

Donde:

- \( \theta \) = Ángulo de rotación  
- \( J \) = Momento de inercia  
- \( T(t) \) = Par aplicado

-----------

## 7. Grados de Libertad (DOF)

Número mínimo de coordenadas independientes para definir la posición de un sistema.

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=DOF = N_{\text{mov}} - N_{\text{restric}}"><img src="http://www.alciro.org/cgi/tex.cgi?DOF = N_{\text{mov}} - N_{\text{restric}}" title="DOF = N_{\text{mov}} - N_{\text{restric}}" border="0" /></a>

Ejemplo:  

Un sistema de suspensión que solo se desplaza verticalmente tiene 1 grado de libertad.
---------------

📚 Ejercicio 1 — Sistema Masa-Resorte-Amortiguador

Un sistema masa-resorte-amortiguador está compuesto por:

![image](https://github.com/user-attachments/assets/8e297a6d-332d-446e-826d-a5407822deb2)


- Masa: 𝑚 = 5kg
- Constante de resorte k=100 N/m
- Coeficiente de amortiguamiento b= 20 Ns/m

El sistema parte desde reposo  y(0)=0 y se le aplica una fuerza escalón de u(t)=10N a partir de t=0.

Plantea la ecuación diferencial y determina la respuesta libre del sistema.

📌 Ecuación diferencial del sistema:ç

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=m\frac{d^2y(t)}{dt^2} + b \frac{dy(t)}{dt} + k y(t) = u(t)"><img src="http://www.alciro.org/cgi/tex.cgi?m \frac{d^2y(t)}{dt^2} + b \frac{dy(t)}{dt} + k y(t) = u(t)" title="m \frac{d^2y(t)}{dt^2} + b \frac{dy(t)}{dt} + k y(t) = u(t)" border="0" /></a>

Sustituyendo valores:

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=2 \frac{d^2\theta(t)}{dt^2} + 5 \frac{d\theta(t)}{dt} + 50 \theta(t) = 20"><img src="http://www.alciro.org/cgi/tex.cgi?2 \frac{d^2\theta(t)}{dt^2} + 5 \frac{d\theta(t)}{dt} + 50 \theta(t) = 20" title="2 \frac{d^2\theta(t)}{dt^2} + 5 \frac{d\theta(t)}{dt} + 50 \theta(t) = 20" border="0" /></a>

📌 Conclusiones
- Los sistemas mecánicos, como masa-resorte y rotacionales, se modelan mediante ecuaciones diferenciales que describen su comportamiento dinámico.

- Los parámetros físicos m,b, k controlan la estabilidad y respuesta del sistema, determinando si la respuesta es oscilante o amortiguada.

- Los diagramas de cuerpo libre son esenciales para identificar correctamente las fuerzas y plantear ecuaciones de movimiento de forma clara.

- Comprender estas bases es fundamental para aplicar técnicas de control digital sobre sistemas físicos reales.



​
​
 

​
 





