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
### Nieto :boy:
