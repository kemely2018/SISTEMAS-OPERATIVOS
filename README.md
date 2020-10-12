# Lab02 - Señales
Identifica y aplica los principios de creación de procesos (fork, exec y waitpid).
También se aplican los conocimientos de tratamiento de señales en el sistema
Linux.
## Integrantes 
- Castillo Caccire, Kemely Francis
- Chullunquía Rosas, Sharon Rossely
### Padre :man:
- Será responsable de crear un proceso hijo usando la llamada fork () .
```C
		
		
		
```
- Después de la creación de cada proceso hijo, por medio de la
llamada exec ( execlp ) reemplazará el código del programa hijo, para
ejecutar el programa hijo.c
```C
		
		
		
```
- El programa deberá esperar a que termine la ejecución de los
programas hijo.c y nieto.c . Usar waitpid ().
```C
		
		
		
```
### Hijo :adult:
- El programa hijo.c creará un proceso hijo, por medio de la llamada
fork () .
```C
		
		
		
```
- Después de la creación de cada proceso hijo, por medio de la
llamada exec ( execlp ) reemplazará el código del programa hijo, para
ejecutar el programa nieto.c
```C
		
		
		
```
- El programa hijo enviará al programa nieto (del cual conoce el
PID), cada una de las señales listadas en Señales soportadas.
```C
		
		
		
```
- Detectar si el proceso nieto muere (Hint: detectar la señal
respectiva), y lanzarlo de nuevo, hasta completar el envío de todas
las señales requeridas.
```C
		
		
		
```
### Nieto :boy:
- En este programa serán redefinidos los manejadores ( handlers ) de
las señales indicadas en la sección Señales soportadas.
```C
		
		
		
```
- El tratamiento de señales debe usar la función sigaction () . No usar
la función signal ().
```C
		
		
		
```
- Para cada señal recibida mostrar la siguiente información, obtenida
de siginfo_t (cuando esté disponible)
```C
		
		
		
```
