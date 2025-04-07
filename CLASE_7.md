# CORTE 2 
## CLASE 7
## 10/03/2025
### **Solución ecuaciones diferenciales**

>* 🔑 **Solución ecuaciones diferenciales**:
Un sistema dinámico es cualquier cosa que evoluciona con el tiempo y cuyo comportamiento puede describirse con ecuaciones (usualmente diferenciales).

💡 Ejemplos:
* Un resorte con masa (sistema masa-resorte-amortiguador)

  ![image](https://github.com/user-attachments/assets/4c5b5ece-787e-4149-ba5f-9912b63fdff2)

* El voltaje y corriente en un circuito RLC

![image](https://github.com/user-attachments/assets/4e0c3a40-15e3-449c-9a3b-dff242a68ef4)

* El movimiento de un robot

![image](https://github.com/user-attachments/assets/80ad7ec3-9b67-4f98-aefa-a0940f7c1f55)

>* 🧠 **¿Por qué usamos ecuaciones diferenciales?**
 Porque describen cómo cambia una cantidad respecto al tiempo. En sistemas dinámicos, usamos estas ecuaciones para modelar:

![image](https://github.com/user-attachments/assets/53bb8dca-1345-44e5-9372-9ae948ab1b68)

donde:
* x(t): estado del sistema (posición, velocidad, temperatura, etc.)
* u(t): entrada o control (fuerza, voltaje, etc.)
* f: describe la dinámica del sistema

>*  🧰 Herramientas que usamos para resolver
* Métodos analíticos: separación de variables, transformada de Laplace, etc.
* Métodos numéricos: Euler, Runge-Kutta (para computadora)
* Transformadas: pasar al dominio de s para trabajar con algebra en lugar de derivadas

### **Metodología de solución**
* Aplicar tansformada de LaPlace a toda la ecuación (término a término), de tal manera que se obtenga una ecuación algebráica en el dominio de s
* Despejar la variable que representa la salida de la ecuación
* Aplicar transformada inversa de LaPlace a la expression obtenida para obtener la solución en el dominio del tiempo

💡 Ejemplo 1 : 

![image](https://github.com/user-attachments/assets/f9b3d49a-becb-4020-9970-ea2cc47e6cd9)



