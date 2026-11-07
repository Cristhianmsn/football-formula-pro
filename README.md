# FOOTBALL FORMULA PRO — Proyecto Android

App Android nativa contenedora de una interfaz local (WebView), funciona sin cuenta y no necesita internet.

## Abrir y compilar
1. Descomprime el ZIP.
2. Abre la carpeta `football-formula-pro` con Android Studio.
3. Espera la sincronización de Gradle (requiere internet la primera vez para descargar Android Gradle Plugin).
4. Conecta un teléfono Android o inicia un emulador y pulsa **Run**.
5. Para generar el APK: **Build > Build Bundle(s) / APK(s) > Build APK(s)**. Android Studio mostrará la ruta del APK.

Requisitos: Android Studio reciente, JDK 17 y Android SDK 35; soporta Android 6.0 (API 23) o posterior. El proyecto contiene la aplicación completa y su fuente.

## Funcionamiento y datos
- Fórmula sin cambios: `Form Points + (2 × GS Avg) − GC Avg`.
- Victoria 3 puntos, empate 1 y derrota 0 en los últimos cinco encuentros ingresados.
- Estimated Goals: promedio simple de goles a favor propios y goles recibidos del rival.
- Indicador X experimental: `máximo(0, 10 − diferencia absoluta de Team Strength Score)`; es una métrica heurística distinta de la fórmula original.
- Los puntajes y el ranking NO son probabilidades ni garantías.
- Los análisis y resultados se guardan en localStorage dentro del dispositivo. Exportación de historial a CSV.
- Sin conexión a servidor, sincronización o carga automática de estadísticas.

Firma visible del creador: **MartinezCh. Cristhian**.
