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

* 1: Aplicamos transformada de Laplace.

![image](https://github.com/user-attachments/assets/7c63f985-39d7-4161-be82-e1a7716631dc)

recordando que:tranformada de derivadas.

![image](https://github.com/user-attachments/assets/45c88648-be7e-4135-a9ec-b80ed4b313a0)

* 2: Sustituimos condiciones iniciale.

  ![image](https://github.com/user-attachments/assets/608f93fe-c749-469c-83eb-06c296c6db51)


* 3: Agrupamos términos.

  ![image](https://github.com/user-attachments/assets/2c9de97a-72f9-43c1-970d-a8311f04171b)

  * 4: Despejamos X(s)

    ![image](https://github.com/user-attachments/assets/ecc3730f-d8ee-4c30-b6f3-e29974490eb0)

  * 5: resolvemos para implementar tranformada de laplace
    * 1. Separar en fracciones parciales:

         ![image](https://github.com/user-attachments/assets/58879c6c-2614-4bdf-a3c4-3f9d6960cc0e)

    * 2. Primera parte:

         ![image](https://github.com/user-attachments/assets/0b723156-2ba5-4149-99c6-70e35f858624)

         Esta se resuelve con fracciones parciales. Sea:
    
    * ![image](https://github.com/user-attachments/assets/ca3fb782-2590-4a53-8fd2-9f755e2a5129)
   
    * Multiplicamos todo por :  ![image](https://github.com/user-attachments/assets/bbf775cb-6382-4e7b-bbfe-72535d7efc23)
   
      ![image](https://github.com/user-attachments/assets/49c9e6a9-b612-4a9d-ae29-0b4f0bd445fb)

   
   
    




  





