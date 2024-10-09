Al cambiar ajustes dentro del juego, se pueden eliminar algunos ajustes dentro de Engine.ini y de GameUserSettings.ini por lo que pongo una guia para que puedas modificarlo a tu gusto, no necesitas directamente usar los mios. 

GameUserSettings.ini
[ScalabilityGroups]
sg.ResolutionQuality=50
Ajusta la calidad de la resolución interna. (Rango: 0 a 100. 100 es máxima calidad, 0 es mínima).

sg.ViewDistanceQuality=1
Controla la distancia a la que los objetos son visibles. (Rango: 0 a 3. 0 es baja distancia, 3 es máxima).

sg.AntiAliasingQuality=1
Ajusta el suavizado de bordes. (Rango: 0 a 3. 0 es desactivado, 3 es calidad máxima).

sg.ShadowQuality=1
Controla la calidad de las sombras. (Rango: 0 a 3. 0 es desactivado o baja calidad, 3 es alta calidad).

sg.GlobalIlluminationQuality=1
Ajusta la calidad de la iluminación global. (Rango: 0 a 3. 0 es desactivado, 3 es alta calidad).

sg.ReflectionQuality=1
Ajusta la calidad de las reflexiones. (Rango: 0 a 3. 0 es desactivado o baja calidad, 3 es alta calidad).

sg.PostProcessQuality=1
Controla la calidad de los efectos post-procesamiento. (Rango: 0 a 3. 0 es desactivado, 3 es máxima calidad).

sg.TextureQuality=1
Ajusta la calidad de las texturas. (Rango: 0 a 3. 0 es baja calidad, 3 es alta calidad).

sg.EffectsQuality=1
Ajusta la calidad de los efectos visuales. (Rango: 0 a 3. 0 es desactivado o baja calidad, 3 es alta calidad).

sg.FoliageQuality=1
Controla la calidad de la vegetación. (Rango: 0 a 3. 0 es baja calidad, 3 es alta calidad).

sg.ShadingQuality=1
Ajusta la calidad de los sombreadores. (Rango: 0 a 3. 0 es baja calidad, 3 es alta calidad).

[/Script/Engine.GameUserSettings]
bUseVSync=False
Desactiva la sincronización vertical (V-Sync). Para activarla, cambia el valor a True.

bUseDynamicResolution=False
Desactiva la resolución dinámica. Para activarla, cambia el valor a True.

ResolutionSizeX=1920
Ajusta el ancho de la resolución de pantalla. (Ejemplo: 1280, 1600, 1920, etc.).

ResolutionSizeY=1080
Ajusta la altura de la resolución de pantalla. (Ejemplo: 720, 1080, etc.).

FullscreenMode=0
Establece el modo de pantalla. (0 = ventana, 1 = pantalla completa). Para pantalla completa, ponlo en 1.

FrameRateLimit=60.000000
Limita la cantidad de fotogramas por segundo. Puedes ponerlo a 30 o 60 dependiendo del rendimiento deseado.

AudioQualityLevel=0
Ajusta la calidad del audio. (Rango: 0 a 3. 0 es baja calidad, 3 es alta calidad).

bUseHDRDisplayOutput=False
Desactiva el soporte HDR. Para activarlo, cambia el valor a True.


Engine.ini
[SystemSettings]
r.LODDistanceFactor=3.0
Ajusta la distancia a la que se aplican los niveles de detalle (LOD). (Rango: 0 a 10. Aumentar el valor mejora la calidad de los objetos distantes).

r.LODGroup=2
Determina qué grupo de LOD se usa. (Rango: 0 a 3. 0 es mayor detalle, 3 es menor detalle).

r.TextureStreaming=1
Habilita el streaming de texturas. (1 para activar, 0 para desactivar).

r.Streaming.PoolSize=1024
Establece el tamaño de la memoria para las texturas. (Valor en MB, por ejemplo, 1024 MB).

r.ShadowQuality=1
Ajusta la calidad de las sombras. (Rango: 0 a 3. 0 es desactivado, 3 es alta calidad).

r.MaterialQualityLevel=1
Ajusta la calidad de los materiales. (Rango: 0 a 2. 0 es baja calidad, 2 es alta calidad).

r.Shadow.CSM.MaxDistance=1000
Establece la distancia máxima para sombras en cascada (CSM). Puedes reducir este valor para mejorar el rendimiento (por ejemplo, 500).

r.FidelityFX.FI.Enabled=1
Activa FidelityFX para mejorar el rendimiento gráfico. (1 para activar, 0 para desactivar).

r.MotionBlurQuality=0
Desactiva la calidad del "motion blur". Para activarlo, ponlo en 1.

r.HZBOcclusion=1
Activa la oclusión de hardware. (1 para activar, 0 para desactivar).

r.ReflectionsQuality=0
Desactiva la calidad de las reflexiones. Para activarlas, ponlo en 1 o 2.

r.SSR.Quality=0
Desactiva las reflexiones en el espacio de pantalla (SSR). Para activarlas, ponlo en 1.

r.ReflectionQuality=0
Desactiva las reflexiones en la escena. Para activarlas, ponlo en 1.

r.MotionBlur=0
Desactiva el "motion blur". Para activarlo, ponlo en 1.

r.AntiAliasing=0
Desactiva el Anti-Aliasing. Para activarlo, ponlo en 1 (FXAA), 2 (TAA) o en 3 para la máxima calidad.
