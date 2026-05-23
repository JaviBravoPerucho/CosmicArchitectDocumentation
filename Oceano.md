## Ocean Component
Este componente permite que el planeta tenga un océano. El océano consiste en una malla estática esfera con material, tamaño y resolución configurable. A esta malla no se le puede aplicar ruido para el relieve al no ser un clipmap, las zonas de océano se consideran planas.

* **Has Ocean:** Booleano que permite activar y desactivar la malla de océano del planeta
* **Sea Level Km:** El nivel del mar en kilómetros, lo que cambia el tamaño de la malla esférica del océano. Se puede ajustar a un nivel similar al de la malla del clipmap para dar la impresión de tener orillas
* **Ocean Resolution:** Resolución de la malla esférica del océano. Afectará al rendimiento
* **Ocean Material:** Material aplicado a la malla de océano. Se puede el material que ofrecemos llamado `MI_CosmicOceanV2`, o se puede crear un material propio al que aplicar al océano.