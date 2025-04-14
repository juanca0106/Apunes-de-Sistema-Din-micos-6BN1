# CORTE 2 
## clase de Sistemas electricos
### 📅 **Curso:** sistemas dinamicos 
### 👨‍🏫 **Profesor:** Ing. Jorge Eduardo Cote Ballesteros
### 🧑‍🎓 **Semestre:** Sexto (2025)
### 🧑‍🎓 ** estudiantes** juan camilo cruz quintana y daniel corredor peña 
---
## **🔌 Circuito RLC**
El comportamiento del circuito se describe usando las leyes de Kirchhoff:

![image](https://github.com/user-attachments/assets/75956def-d9d3-4025-a17f-1b28ce028bb6)

>- <a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=R = \frac{v(t)}{i(t)} "><img src="http://www.alciro.org/cgi/tex.cgi?R = \frac{v(t)}{i(t)}" title="R = \frac{v(t)}{i(t)} " border="0" /></a> : Ley de Ohm
  
>- <a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=i(t) &= C \frac{dv(t)}{dt}"><img src="http://www.alciro.org/cgi/tex.cgi?i(t) &= C \frac{dv(t)}{dt}" title="i(t) &= C \frac{dv(t)}{dt}" border="0" /></a> : Carga de un condensador

>- <a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=v(t) &= L \frac{di(t)}{dt}"><img src="http://www.alciro.org/cgi/tex.cgi?v(t) &= L \frac{di(t)}{dt}" title="v(t) &= L \frac{di(t)}{dt}" border="0" /></a> : Carga de un inductor

💡ejemplo 1 :

![image](https://github.com/user-attachments/assets/858051e8-be04-4048-a982-d9a6c86a815a)

Aplicandoley de Kirchoff:

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=- u + v_R + v_L + v_C &= 0 \\- u(t) + i(t) * R + L \frac{di(t)}{dt} + y(t)= 0"><img src="http://www.alciro.org/cgi/tex.cgi?- u + v_R + v_L + v_C &= 0 \\- u(t) + i(t) * R + L \frac{di(t)}{dt} + y(t)= 0" title="- u + v_R + v_L + v_C &= 0 \\- u(t) + i(t) * R + L \frac{di(t)}{dt} + y(t)= 0" border="0" /></a>

La ecuación diferencial resultante es:

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=-u(t) + RC \frac{dy(t)}{dt} + LC \frac{d^2y(t)}{dt^2} + y(t) = 0"><img src="http://www.alciro.org/cgi/tex.cgi?-u(t) + RC \frac{dy(t)}{dt} + LC \frac{d^2y(t)}{dt^2} + y(t) = 0" title="-u(t) + RC \frac{dy(t)}{dt} + LC \frac{d^2y(t)}{dt^2} + y(t) = 0" border="0" /></a>

##**Aplicandonodos**

![image](https://github.com/user-attachments/assets/19e35ace-957b-4578-ab78-3dc5c74f7afb)

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=i_u - i_1 - i_c = 0 \\i_u(t) - \frac{V_{AB}}{0.5} - 2 \frac{dy(t)}{dt} &= 0 \\"><img src="http://www.alciro.org/cgi/tex.cgi?i_u - i_1 - i_c = 0 \\i_u(t) - \frac{V_{AB}}{0.5} - 2 \frac{dy(t)}{dt} &= 0 \\" title="i_u - i_1 - i_c = 0 \\i_u(t) - \frac{V_{AB}}{0.5} - 2 \frac{dy(t)}{dt} &= 0 \\" border="0" /></a>

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=V_{AB} &= i_c \cdot 1 + y(t)"><img src="http://www.alciro.org/cgi/tex.cgi?V_{AB} &= i_c \cdot 1 + y(t)" title="V_{AB} &= i_c \cdot 1 + y(t)" border="0" /></a>

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=V_{AB} = 2 \frac{dy(t)}{dt} + y(t)"><img src="http://www.alciro.org/cgi/tex.cgi?V_{AB} = 2 \frac{dy(t)}{dt} + y(t)" title="V_{AB} = 2 \frac{dy(t)}{dt} + y(t)" border="0" /></a>

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=u(t) - \frac{2}{0.5} \frac{dy(t)}{dt} - \frac{1}{0.5} y(t) - 2 \frac{dy(t)}{dt} = 0"><img src="http://www.alciro.org/cgi/tex.cgi?u(t) - \frac{2}{0.5} \frac{dy(t)}{dt} - \frac{1}{0.5} y(t) - 2 \frac{dy(t)}{dt} = 0" title="u(t) - \frac{2}{0.5} \frac{dy(t)}{dt} - \frac{1}{0.5} y(t) - 2 \frac{dy(t)}{dt} = 0" border="0" /></a>

ecuacion resultante:

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq={u(t) - 6 \frac{dy(t)}{dt} - 2y(t) = 0}"><img src="http://www.alciro.org/cgi/tex.cgi?{u(t) - 6 \frac{dy(t)}{dt} - 2y(t) = 0}" title="{u(t) - 6 \frac{dy(t)}{dt} - 2y(t) = 0}" border="0" /></a>

## **Circuitoscon amplificadoresoperacionales**

**amplificador no inversor**

Se utilizanleyesde Kirchoffy el modelosimplificadodel amplificadoroperacional

![image](https://github.com/user-attachments/assets/ba9e5ba5-a2e8-4f3f-97e1-8bcd7f04b0eb)

La tension enambas entradas del amplificadorson igualesV+ = V- La corrientea las entradas del amplificadores 0, La impedanciade entrada es muygrande y La impedanciade salidaes muypequeña

![image](https://github.com/user-attachments/assets/8c0b0f23-a3e8-4222-81a1-521b9dc25849)

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=i_1 - i_2 &= 0 \\\frac{e_o - e_i}{R_2} - \frac{e_i}{R_1} &= 0 \\\frac{e_o}{R_2} &= e_i \left( \frac{1}{R_2} + \frac{1}{R_1} \right) \\e_o &= e_i \left( 1 + \frac{R_2}{R_1} \right)"><img src="http://www.alciro.org/cgi/tex.cgi?i_1 - i_2 &= 0 \\\frac{e_o - e_i}{R_2} - \frac{e_i}{R_1} &= 0 \\\frac{e_o}{R_2} &= e_i \left( \frac{1}{R_2} + \frac{1}{R_1} \right) \\e_o &= e_i \left( 1 + \frac{R_2}{R_1} \right)" title="i_1 - i_2 &= 0 \\\frac{e_o - e_i}{R_2} - \frac{e_i}{R_1} &= 0 \\\frac{e_o}{R_2} &= e_i \left( \frac{1}{R_2} + \frac{1}{R_1} \right) \\e_o &= e_i \left( 1 + \frac{R_2}{R_1} \right)" border="0" /></a>

Con elementosalmacenadoresde energía

![image](https://github.com/user-attachments/assets/55697610-dbfc-418e-b1b5-0c2c8a3d7745)

![image](https://github.com/user-attachments/assets/9fcdb924-31a5-42e1-8c20-8ac74f2427aa)

--------
 📚 ejercici 1: Modelo usando nodos
 
![image](https://github.com/user-attachments/assets/4b91612e-5c1f-454f-a210-7b5f55699d42)


 Aplicando LKC:

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=i_u - \frac{V_{AB}}{0.5} - 2 \frac{dy(t)}{dt} = 0
"><img src="http://www.alciro.org/cgi/tex.cgi?i_u - \frac{V_{AB}}{0.5} - 2 \frac{dy(t)}{dt} = 0" title="i_u - \frac{V_{AB}}{0.5} - 2 \frac{dy(t)}{dt} = 0" border="0" /></a>

Con:
<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=V_{AB} = 2 \frac{dy(t)}{dt} + y(t)"><img src="http://www.alciro.org/cgi/tex.cgi?V_{AB} = 2 \frac{dy(t)}{dt} + y(t)" title="V_{AB} = 2 \frac{dy(t)}{dt} + y(t)" border="0" /></a>

Se obtiene:

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=u(t) - 6 \frac{dy(t)}{dt} - 2y(t) = 0"><img src="http://www.alciro.org/cgi/tex.cgi?u(t) - 6 \frac{dy(t)}{dt} - 2y(t) = 0" title="u(t) - 6 \frac{dy(t)}{dt} - 2y(t) = 0" border="0" /></a>

 📚 ejercici 2: Amplificador no inversor con capacitor

![image](https://github.com/user-attachments/assets/33aac3ef-fa44-4c7f-b550-e6f04e3cb693)

Condiciones del circuito:

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=\frac{e_i}{R_1} = -\frac{e_o}{R_2} - C \frac{de_o}{dt}"><img src="http://www.alciro.org/cgi/tex.cgi?\frac{e_i}{R_1} = -\frac{e_o}{R_2} - C \frac{de_o}{dt}" title="\frac{e_i}{R_1} = -\frac{e_o}{R_2} - C \frac{de_o}{dt}" border="0" /></a>

Modelo matemático:

<a href="http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp?eq=\frac{e_i}{R_1} + \frac{e_o}{R_2} + C \frac{de_o}{dt} = 0"><img src="http://www.alciro.org/cgi/tex.cgi?\frac{e_i}{R_1} + \frac{e_o}{R_2} + C \frac{de_o}{dt} = 0" title="\frac{e_i}{R_1} + \frac{e_o}{R_2} + C \frac{de_o}{dt} = 0" border="0" /></a>

-----------------------------

✅ Conclusiones
- La aplicación de las leyes de Kirchhoff permite modelar matemáticamente circuitos eléctricos complejos mediante ecuaciones diferenciales.

- El uso de componentes como resistencias (R), inductancias (L) y capacitores (C) define el comportamiento dinámico del sistema, representado por ecuaciones de segundo orden en muchos casos.

- Los modelos obtenidos son esenciales para el análisis de estabilidad, respuesta en frecuencia, y control de sistemas eléctricos.

- Herramientas como la modelación nodal y el análisis de amplificadores operacionales permiten entender mejor la interacción entre variables de entrada y salida en un circuito.

- La representación en LaTeX y el uso de esquemas claros facilita la documentación técnica y la comprensión por parte de otros ingenieros o estudiantes.



