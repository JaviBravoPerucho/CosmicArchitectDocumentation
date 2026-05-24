# Gravity

### Gravity Component

Guarda información sobre las interacciones físicas gravitacionales que tiene el planeta o el objeto con el entorno, y el Gravity Subsystem se dedica a actualizar la posición y velocidad de los planetas en función de esta información. Este componente no lo tienen los Cosmic Planet por defecto y hay que añadirlo si se desean interacciones gravitatorias.

* **Gravity Mode:**
  * **Nearest Planet:** El cuerpo será atraído por el planeta más cercano.
  * **Specific Planet:** Será atraído un cuerpo designado. Al marcar esta opción, aparece una nueva opción para asignar el objeto al que se atrae.
  * **All Planets:** Influencia de todos los planetas del sistema.
  * **N-body:** Simulación de atracción mutua entre múltiples cuerpos.
* **Is Planet:** Si es True, calcula fuerza gravitacional mediante Radio y Aceleración superficial del planeta. Si es False, calcula fuerza gravitacional mediante Masa.
* **Affects Others:** Determina si el objeto ejerce fuerza de gravedad sobre otros.
* **Is Affected by Others:** Determina si el objeto responde a la gravedad externa.

### Orbit Component

Permite añadir una órbita a un objeto. Controla el movimiento orbital de un objeto alrededor de un punto de referencia.

* **Semi Major Axis (Km):** Radio mayor de la elipse orbital.
* **Eccentricity:** Nivel de deformación de la órbita (0 es circular, valores mayores estiran la elipse).
* **Initial Position:** Punto de inicio del objeto dentro de su trayectoria.
* **Orbital Period:** Tiempo en segundos requerido para completar una revolución total.
* **Inclinación XYZ:** Orientación del plano orbital en los tres ejes del espacio.
