# Tema 1.2: Entorno portable y ligero de Dart y Flutter



## Mi equipo

- Sistema: Windows 11

- RAM: 16 GB

- Procesador: AMD Ryzen 9 3900X (12 núcleos)

- Espacio libre en disco: unos 286 GB en C:

- Virtualización: habilitada

- Permisos de administrador: sí

- Conclusión: el equipo permite incluso un entorno pesado, pero para el curso trabajo con un entorno ligero (consola y Chrome).



## Versiones

- Flutter 3.47.8 (canal stable)

- Dart 3.13.7



## Ruta del entorno

Todo el kit está en `C:\dev` (no tengo unidad D:), con las carpetas `flutter`, `vscode` (con `data`), `pub-cache` y `proyectos`.



## Destinos de ejecución que puedo usar

- Consola Dart

- Chrome (web)

- También aparecen Windows (escritorio) y Edge en `flutter devices`.



## Notas sobre el PATH

Mi equipo ya tenía otro Flutter (3.29.3) en el PATH del sistema, que tiene prioridad sobre el del usuario. Por eso no agregué el Flutter portable al PATH permanente. Lo activo solo en cada ventana con `set PATH` o con `iniciar.bat`.



## Problema que resolví

Al ejecutar con F5 en VS Code, salió el error "The language version 3.13 specified for the package is too high. The highest supported language version is 3.7". La causa fue que abrí `Code.exe` con doble clic, y esa ventana no heredó mi PATH: usó el Dart del Flutter viejo. Lo resolví abriendo VS Code desde una ventana de CMD con el PATH del Flutter portable ya configurado.



## Contenido de esta carpeta

- `iniciar.bat`: abre el entorno portable.

- `doctor.txt`: salida de `flutter doctor -v`.

- `evidencias/`: capturas de pantalla.

- `hola_entorno/`: proyecto de consola, con `.vscode/launch.json`.

- `hola_flutter/`: app Flutter ejecutada en Chrome.

