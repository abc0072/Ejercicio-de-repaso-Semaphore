¿Porque elegiste Semaphore?

# Descripción del proyecto
Este proyecto simula un aparcamiento con plazas limitadas usando hilos (Thread) en Java.  
Varios coches intentarán entrar al mismo tiempo a un aparcamiento, y si no hay plazas libres, deben esperar hasta que una plaza quede libre.  
Cada coche entra, permanece aparcado un tiempo aleatorio entre 1 y 4 segundos, y luego sale, liberando su plaza.  

# Reflexión sobre Semaphore
Elegí usar la clase "Semaphore" porque permite gestionar cuantos coches van a entrar al aparcamiento a la vez, lo que encaja perfectamente con el problema de plazas limitadas.  
A diferencia de "synchronized" o "ReentranLock", que solo permite el acceso a un hilo, "Semaphore" puede manejar varios hilos al mismo tiempo, no solo uno.  
Con "wait()/notify()" tendríamos que hacer manualmente el contador de plazas y la lógica para mostrar los mensajes, lo cual es más propenso a errores.  
Por eso, "Semaphore" es más eficiente y seguro para este tipo de proyectos.

# Resultados por consola
<img width="341" height="392" alt="image" src="https://github.com/user-attachments/assets/02324271-ba1a-49b8-914a-8808ba62b191" />
