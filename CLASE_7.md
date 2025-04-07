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
-------------------------------------------------------------------------------------------------------------------------------------------------------------

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
--------------------------------------------------------------------------------------------------------------------------------------------------------------
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

     * Expandimos:

       ![image](https://github.com/user-attachments/assets/2fc024e9-63a7-4deb-97f8-8c543c5820f9)


    * Juntamos todo:

      ![image](https://github.com/user-attachments/assets/931665e1-f774-4cc0-bc63-441764bac4a2)

    *Agrupamos: 

    ![image](https://github.com/user-attachments/assets/9b792c99-f7dd-4082-b380-d2e65b1e93ce)

     * Ahora:

       ![image](https://github.com/user-attachments/assets/eb1ca958-471e-4683-8e61-f4216346a37b)

    * Entonces:

      ![image](https://github.com/user-attachments/assets/bd5124b8-27f4-4945-ab7d-2527c6f063e5)

     * 3. segunda parte :

           ![image](https://github.com/user-attachments/assets/f5c3ccaa-5fd4-4189-b22f-e48b424cc096)

          *Esto lo podemos separar directamente:

          ![image](https://github.com/user-attachments/assets/c5daf2b0-0334-41fa-9bce-5710d328a6e3)

  -------------------------------------------------------------------------------------------------------------------------------------------        
    🧠 Ahora sumamos todo:

  ![image](https://github.com/user-attachments/assets/4a902abd-4f82-47c0-8b17-4584d5db0a6c)


  ![image](https://github.com/user-attachments/assets/0b0d75bd-33dc-428c-85f3-62e8923c14c6)


  * entonces:

    ![image](https://github.com/user-attachments/assets/fc871b90-dfb9-4f6a-9e7d-33ec8748b6f3)

  * 4. Aplicamos la transformada inversa de Laplace
       Usamos:: 

![image](https://github.com/user-attachments/assets/78098220-e90a-4501-bd71-93ffbf77f6ee)

* Entonces: Esta seri la solucion final 

  ![image](https://github.com/user-attachments/assets/a3293d01-453a-4b08-b8d9-d29dc5d22bd9)


  # codigo del ejemplo 1

 >* % Solución simbólica de la EDO
syms x(t)

% Definimos la ecuación diferencial
eqn = diff(x, t, 2) + 4*diff(x, t) + 4*x == 5;

% Condiciones iniciales
Dx = diff(x, t);      % Guarda la primera derivada
cond1 = x(0) == 1;
cond2 = Dx(0) == 0;

% Resolver con dsolve
sol = dsolve(eqn, [cond1, cond2]);

% Mostrar resultado
disp('Solución analítica:')
pretty(sol)

%% Solución numérica%%  
% Definimos el intervalo de tiempo
tspan = [0 10];

% Condiciones iniciales: [x(0); x'(0)]
x0 = [1; 0];

% Ecuación diferencial como sistema de primer orden
% x1 = x, x2 = dx/dt
% dx1/dt = x2
% dx2/dt = 5 - 4*x2 - 4*x1

f = @(t, x) [x(2); 5 - 4*x(2) - 4*x(1)];

% Resolver con ode45
[t, x] = ode45(f, tspan, x0);

% Graficar
plot(t, x(:,1), 'LineWidth', 2)
xlabel('Tiempo (t)')
ylabel('x(t)')
title('Solución numérica de la EDO: \ddot{x} + 4\dot{x} + 4x = 5')
grid on 


      
      




          




   
    




  





