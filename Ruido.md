## Noise Settings (Configuración de Ruido)
El sistema de ruido controla la generación del relieve y la apariencia visual del terreno.

**Clases Base:**
* **CosmicNoiseClass** (ej. CosmicDefaultNoiseSettings): Almacena los parámetros de las capas de ruido.
* **CosmicNoiseStrategy:** Procesa el ruido y evalúa la altura y el color de cada punto. Permite definir lógicas personalizadas para el terreno.
* Para tener clases de ruido propias, se pueden crear clases que hereden de CosmicNoiseClass y CosmicNoiseStrategy y configurar las capas de ruido y parámetros que se quieran. Por ejemplo la herramienta contiene un tipo Cosmic Earth Settings que contiene capas de ruido para los continentes, las montañas y demás para replicar el planeta Tierra.

**CosmicNoiseLayer:**
Define las propiedades matemáticas de una capa de ruido individual.
* **Noise Type:** Algoritmo base (Perlin, Simplex, Cellular, Value o Ridged).
* **Fractal Type:** Patrón fractal aplicado (FBM, Ridged o PingPong).
* **Frequency:** Nivel de vibración o escala del ruido.
* **Octaves:** Número de capas de detalle superpuestas.
* **Lacunarity:** Controla la heterogeneidad y distinción del patrón.
* **Persistence:** Define la pérdida de amplitud por octava (valores bajos = más rocoso; valores altos = más suave).
* **Amplitude:** Intensidad y contraste del relieve generado.

**CosmicNoise Biome Parameters:**
Parámetros que permiten variar el terreno según regiones geográficas.
* **TemperatureFrequency:** Frecuencia del ruido que define zonas frías o cálidas.
* **HumidityFrequency/Octaves:** Configuración del ruido que define la humedad del terreno.
* **Latitude Effect:** Influencia de la latitud en la temperatura (ej. polos fríos vs. ecuador cálido).
* **Altitude Temperature Penalty:** Reducción de temperatura en función de la elevación.
* **HumidityContrast/Offset:** Ajustes de intensidad y desplazamiento para el mapa de humedad.

**Crater Settings:**
Configuración específica para la generación de impactos mediante el ruido Cosmic Crater Settings.
* **Crater Frequency:** Densidad de cráteres en la superficie.
* **Crater Depth:** Profundidad de las cavidades de impacto.
* **Crater Radius Multiplier:** Escala general del tamaño de los cráteres.
* **Crater Rim Height:** Altura de la cresta o borde exterior.
* **Crater Rim Sharpness:** Definición del borde (Suave vs. Afilado).
* **Crater Floor Height:** Elevación de la base interna del cráter.