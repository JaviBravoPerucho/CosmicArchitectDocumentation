## Cosmic Planet
Es el actor que representa el planeta. Se añade a la escena y tiene todos los componentes necesarios para simular un planeta real.

**Atributos:**
* **RadiusKm:** El radio del planeta en kilómetros
* **NoiseClass:** Configuración del ruido
* **PlanetMainColor1, PlanetMainColor2, PlanetColdColor, PlanetHotColor, PlanetSlopeColor:** Colores de las distintas regiones del planeta
* **NoiseScaleSmall, NoiseScaleMedium, NoiseScaleLarge:** Escala de las distintas capas de ruido que se utilizan para el color

**Componentes:**
* **ClipmapComponent:** Actualización de malla de renderizado con LODs
* **CollisionComponent:** Actualización de malla de colisión dinámica
* **OceanComponent:** Permite instanciar una malla esférica que simula el océano del planeta, con su propio material
* **FoliageSpawnerComponent:** Generación de follaje procedimentalen forma de Asset Collections