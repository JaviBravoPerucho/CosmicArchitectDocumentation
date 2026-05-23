## Foliage Spawner Component
Responsable de la generación procedimental de vegetación en el planeta. Se define una estructura de datos llamada Foliage Collection con los grupos de meshes (modelos de plantas o cualquier tipo de objeto) que se instanciarán. Para cada grupo se puede definir el rango de altura, temperatura, humedad, y curvatura en la que se instancian esos modelos. También, para cada modelo se pueden definir los rangos de rotación aleatoria que se aplican al instanciarlos, el rango de escala y la cantidad de instancias por kilómetro cuadrado.

El Foliage Spawner Component gestiona 3 capas de instanciación: una cercana, una mediana y una lejana. Los modelos de la capa cercana pueden ser piedras, césped o hierbas y se instanciarán en una zona cercana al jugador. La capa mediana y la capa lejana pueden ser para árboles y rocas que se instancien menos a menudo.

* **Foliage Collection:** Data Asset que contiene la información de los modelos que instanciará el spawner. Se puede crear uno propio o utilizar el que viene con el plugin llamado Earth Foliage, que contiene modelos de plantas y rocas obtenidos de Fab de forma gratuita.
* **Near Layer Radius Km:** Radio de la capa cercana de generación de follaje
* **Medium Layer Radius Km:** Radio de la capa mediana de generación de follaje
* **Far Layer Radius Km:** Radio de la capa lejana de generación de follaje
* **Max Instances Per Frame:** Número máximo de instancias que se generarán por frame. Afecta mucho al rendimiento

