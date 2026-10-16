COLOMBIA EXPLORADORES — VERSIÓN PROFESIONAL INICIAL
===================================================

CONTENIDO
- index.html: página principal.
- assets/styles.css: estilos y diseño adaptable.
- assets/app.js: mapa, voz, juegos, puntuación y progreso.
- data/departments.json: datos educativos de los territorios.
- README.txt: instrucciones.

ABRIR LOCALMENTE
1. Descomprime Colombia_Exploradores_Profesional.zip.
2. Abre la carpeta Colombia_Exploradores_Profesional.
3. Para una prueba rápida, abre index.html en Chrome o Edge.
4. Para cargar correctamente archivos JSON y servicios del mapa, es preferible ejecutar un servidor local:
   - Si tienes Python instalado, abre una terminal en esta carpeta y ejecuta:
     python -m http.server 8000
   - Abre en el navegador: http://localhost:8000
   - Para detenerlo, vuelve a la terminal y pulsa Ctrl+C.

PUBLICAR GRATIS EN GITHUB PAGES
1. Crea un repositorio nuevo en GitHub.
2. Sube index.html, la carpeta assets y la carpeta data (mantén esa estructura).
3. En el repositorio, entra en Settings > Pages.
4. En Build and deployment, selecciona Deploy from a branch.
5. Selecciona la rama main y la carpeta /(root), y guarda.
6. Espera la publicación y abre el enlace que GitHub Pages te muestre.

CARACTERÍSTICAS
- Interfaz adaptable a computador, tableta y celular.
- Búsqueda por departamento y capital y filtro por región.
- Fichas educativas y lectura en voz alta del navegador.
- Retos de capitales con corrección y explicación.
- Puntos, niveles, insignias y progreso local.
- Mapa Leaflet/OpenStreetMap con intento de carga de GeoJSON departamental.
- Listado alternativo si el mapa no está disponible.

LIMITACIONES IMPORTANTES
- Los límites geográficos se obtienen de fuentes externas. Si cambian o no responden, el listado seguirá disponible, pero puede no mostrarse el mapa departamental.
- La base educativa contiene información general y algunas cantidades administrativas aproximadas. La población se marca para consulta de DANE y no se presenta como cifra actual verificada.
- Antes de usar en producción educativa, verificar todos los datos administrativos con fuentes oficiales.
- Leaflet, las teselas de OpenStreetMap y la fuente GeoJSON requieren conexión a internet.
- SpeechSynthesis depende del navegador y de las voces instaladas.
- No hay backend ni cuentas de estudiantes; el progreso queda en el navegador del dispositivo.
