Ejercicio 2.E.2 03 - Consola Retro

Lógica del programa
Para resolver este tercer ejercicio, diseñé la clase `ConsolaRetro` con el objetivo de simular la transición de estados de un dispositivo. Le definí tres atributos: `modelo` (String), `numeroSerie` (String) y una variable booleana `encendida` para controlar su estado operativo.

Implementé un constructor parametrizado para inicializar el modelo y el número de serie al momento de instanciar el objeto. El atributo `encendida` no lo incluí en el constructor ya que, por defecto, Java inicializa los booleanos en `false` (representando que la consola arranca apagada).

Para definir su comportamiento, desarrollé tres métodos de tipo `void`:
1. `encender()` y `apagar()`: Se encargan de modificar directamente el valor de la variable booleana `encendida` (a `true` o `false` respectivamente) e imprimen un mensaje descriptivo de la acción.
2. `mostrarEstado()`: Utiliza una estructura condicional `if/else` para evaluar el valor actual de la variable `encendida` y notificar si el dispositivo se encuentra prendido o apagado.

Dentro de la clase `Main`, desarrollé la siguiente lógica de prueba:
1. Instancié un objeto `ConsolaRetro` pasándole al constructor los valores "PSP" y "PSP-1000".
2. Ejecuté una secuencia de llamadas a los métodos del objeto para alterar y verificar su estado dinámicamente. Primero llamé a `mostrarEstado()` para comprobar el estado inicial apagado, luego usé `encender()`, volví a verificar el estado, la apagué con `apagar()` y realicé una comprobación final.

Ejecución en consola
<img width="1366" height="718" alt="{993BC6AA-616B-4A4A-8607-0A4CC143BA0A}" src="https://github.com/user-attachments/assets/079a6d91-a3af-45c8-be5d-a353c255ca96" />
