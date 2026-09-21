Ejercicio 2.E.2 03 - Consola Retro

Lógica del programa
Para resolver este tercer ejercicio, diseñé la clase `ConsolaRetro` con el objetivo de simular la transición de estados de un dispositivo. Le definí tres atributos: `modelo` (String), `numeroSerie` (String) y una variable booleana `encendida` para controlar su estado operativo.

Implementé un constructor parametrizado para inicializar el modelo y el número de serie al momento de instanciar el objeto. El atributo `encendida` no lo incluí en el constructor ya que, por defecto, Java inicializa los booleanos en `false` (representando que la consola arranca apagada).

Para definir su comportamiento, desarrollé tres métodos de tipo `void`:
1. `encender()` y `apagar()`: Se encargan de modificar directamente el valor de la variable booleana `encendida` (a `true` o `false` respectivamente). Además, imprimen un mensaje descriptivo que concatena el atributo `modelo` para indicar exactamente qué consola está cambiando de estado.
2. `mostrarEstado()`: Utiliza una estructura condicional `if/else` para evaluar el valor actual de la variable `encendida` y notifica por consola el estado actual del modelo en particular.

Dentro de la clase `Main`, desarrollé la siguiente lógica de prueba:
1. Instancié un objeto `ConsolaRetro` pasándole al constructor los valores "PSP" y "PSP-1000".
2. Ejecuté una secuencia de llamadas a los métodos del objeto para alterar y verificar su estado dinámicamente. Primero llamé a `mostrarEstado()` para comprobar el estado inicial apagado, luego usé `encender()`, volví a verificar el estado, la apagué con `apagar()` y realicé una comprobación final.

Ejecución en consola
<img width="1366" height="722" alt="{E83BAC05-49C4-4F38-9551-D985240406B8}" src="https://github.com/user-attachments/assets/bf5c510a-1fc1-4f76-888c-6090945738f5" />

