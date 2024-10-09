# Ajustes de Configuración del Juego

Este archivo describe los ajustes de configuración para optimizar y personalizar el rendimiento gráfico y de juego en los archivos `GameUserSettings.ini` y `Engine.ini`. A continuación se detallan los parámetros más importantes que puedes modificar.

---

## GameUserSettings.ini

### [ScalabilityGroups]

- **`sg.ResolutionQuality=50`**  
  Ajusta la calidad de la resolución interna.  
  **Rango:** 0 a 100.  
  **Valor recomendado:** 100 (máxima calidad) para la mejor experiencia visual. Si necesitas mejorar el rendimiento, puedes reducirlo a un valor más bajo como 50.

- **`sg.ViewDistanceQuality=1`**  
  Controla la distancia a la que los objetos son visibles.  
  **Rango:** 0 a 3.  
  **Valor recomendado:** 1 (baja distancia) si necesitas mejorar el rendimiento, 3 para máxima calidad visual.

- **`sg.AntiAliasingQuality=1`**  
  Ajusta el suavizado de bordes.  
  **Rango:** 0 a 3.  
  **Valor recomendado:** 3 (máxima calidad). Si necesitas más rendimiento, ponlo a 0 (desactivado).

- **`sg.ShadowQuality=1`**  
  Controla la calidad de las sombras.  
  **Rango:** 0 a 3.  
  **Valor recomendado:** 3 (alta calidad), si prefieres más rendimiento, ponlo a 1 o 0.

- **`sg.GlobalIlluminationQuality=1`**  
  Ajusta la calidad de la iluminación global.  
  **Rango:** 0 a 3.  
  **Valor recomendado:** 3 (alta calidad). Si necesitas más rendimiento, ponlo en 0.

- **`sg.ReflectionQuality=1`**  
  Ajusta la calidad de las reflexiones.  
  **Rango:** 0 a 3.  
  **Valor recomendado:** 3 para reflejos detallados, o 0 si quieres mejorar el rendimiento.

- **`sg.PostProcessQuality=1`**  
  Controla la calidad de los efectos post-procesamiento.  
  **Rango:** 0 a 3.  
  **Valor recomendado:** 3 para la mejor calidad visual. Si necesitas más rendimiento, ponlo en 0.

- **`sg.TextureQuality=1`**  
  Ajusta la calidad de las texturas.  
  **Rango:** 0 a 3.  
  **Valor recomendado:** 3 para texturas de alta calidad. Ponlo a 0 para obtener un mejor rendimiento.

- **`sg.EffectsQuality=1`**  
  Ajusta la calidad de los efectos visuales.  
  **Rango:** 0 a 3.  
  **Valor recomendado:** 3 para efectos detallados, o 0 para mayor rendimiento.

- **`sg.FoliageQuality=1`**  
  Controla la calidad de la vegetación.  
  **Rango:** 0 a 3.  
  **Valor recomendado:** 3 para vegetación detallada, o 0 para obtener más rendimiento.

- **`sg.ShadingQuality=1`**  
  Ajusta la calidad de los sombreadores.  
  **Rango:** 0 a 3.  
  **Valor recomendado:** 3 para mayor calidad en sombreado, o 0 para un rendimiento más rápido.

---

### [/Script/Engine.GameUserSettings]

- **`bUseVSync=False`**  
  Desactiva la sincronización vertical (V-Sync).  
  **Valor recomendado:** `True` para evitar tearing (desgarro de pantalla) o `False` si prefieres rendimiento.

- **`bUseDynamicResolution=False`**  
  Desactiva la resolución dinámica.  
  **Valor recomendado:** `True` para un ajuste automático de la resolución o `False` para mayor control manual.

- **`ResolutionSizeX=1920`**  
  Ajusta el ancho de la resolución de pantalla.  
  **Valor recomendado:** 1920 para pantallas 1080p, o ajusta según la resolución de tu pantalla.

- **`ResolutionSizeY=1080`**  
  Ajusta la altura de la resolución de pantalla.  
  **Valor recomendado:** 1080 para pantallas 1080p, o ajusta según tu pantalla.

- **`FullscreenMode=0`**  
  Establece el modo de pantalla.  
  **Valor recomendado:** `1` para pantalla completa o `0` para ventana.

- **`FrameRateLimit=60.000000`**  
  Limita la cantidad de fotogramas por segundo.  
  **Valor recomendado:** 60 para una experiencia fluida.

- **`AudioQualityLevel=0`**  
  Ajusta la calidad del audio.  
  **Rango:** 0 a 3.  
  **Valor recomendado:** 3 para audio de alta calidad, o 0 si necesitas mejorar el rendimiento.

- **`bUseHDRDisplayOutput=False`**  
  Desactiva el soporte HDR.  
  **Valor recomendado:** `True` si tu monitor soporta HDR, o `False` para evitar el uso de recursos adicionales.

---

## Engine.ini

### [SystemSettings]

- **`r.LODDistanceFactor=3.0`**  
  Ajusta la distancia a la que se aplican los niveles de detalle (LOD).  
  **Valor recomendado:** 3.0 para una calidad alta, o valores más bajos si necesitas rendimiento.

- **`r.LODGroup=2`**  
  Determina qué grupo de LOD se usa.  
  **Valor recomendado:** 2 para un buen equilibrio, 0 para calidad máxima o 3 para rendimiento.

- **`r.TextureStreaming=1`**  
  Habilita el streaming de texturas.  
  **Valor recomendado:** `1` para activarlo, `0` para desactivarlo.

- **`r.Streaming.PoolSize=1024`**  
  Establece el tamaño de la memoria para las texturas (en MB).  
  **Valor recomendado:** 1024 MB si tienes suficiente memoria, o menor si necesitas optimización.

- **`r.ShadowQuality=1`**  
  Ajusta la calidad de las sombras.  
  **Rango:** 0 a 3.  
  **Valor recomendado:** 3 para sombras de alta calidad, o 0 para mejorar el rendimiento.

- **`r.MaterialQualityLevel=1`**  
  Ajusta la calidad de los materiales.  
  **Rango:** 0 a 2.  
  **Valor recomendado:** 2 para alta calidad, o 0 para mayor rendimiento.

- **`r.Shadow.CSM.MaxDistance=1000`**  
  Establece la distancia máxima para sombras en cascada (CSM).  
  **Valor recomendado:** 1000 para una calidad alta, o reduce el valor para mejorar el rendimiento.

- **`r.FidelityFX.FI.Enabled=1`**  
  Activa FidelityFX para mejorar el rendimiento gráfico.  
  **Valor recomendado:** `1` para activarlo, `0` para desactivarlo.

- **`r.MotionBlurQuality=0`**  
  Desactiva la calidad del "motion blur".  
  **Valor recomendado:** `0` para desactivarlo, `1` para activarlo si prefieres la calidad visual.

- **`r.HZBOcclusion=1`**  
  Activa la oclusión de hardware.  
  **Valor recomendado:** `1` para activarlo, `0` para desactivarlo.

- **`r.ReflectionsQuality=0`**  
  Desactiva las reflexiones en la escena.  
  **Valor recomendado:** `0` para desactivarlas, `1` o `2` para activarlas si prefieres mejor calidad.

- **`r.SSR.Quality=0`**  
  Desactiva las reflexiones en el espacio de pantalla (SSR).  
  **Valor recomendado:** `0` para desactivarlas, `1` para activarlas.

- **`r.ReflectionQuality=0`**  
  Desactiva las reflexiones en la escena.  
  **Valor recomendado:** `0` para desactivarlas, `1` para activarlas.

- **`r.MotionBlur=0`**  
  Desactiva el "motion blur".  
  **Valor recomendado:** `0` para desactivarlo, `1` para activarlo.

- **`r.AntiAliasing=0`**  
  Desactiva el Anti-Aliasing.  
  **Rango:** 0 a 3.  
  **Valor recomendado:** `3` para máxima calidad, o `0` para desactivarlo y mejorar el rendimiento.

---

Este archivo contiene una descripción detallada de los parámetros más comunes para optimizar el rendimiento o mejorar la calidad gráfica de los juegos. Ajusta estos valores según tu hardware y preferencias personales.
