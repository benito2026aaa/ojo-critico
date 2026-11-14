# Ojo Crítico — especial web interactivo

## Abrir la web

Abre `index.html` en Chrome, Edge o Firefox. No hay que instalar nada. Todas las imágenes ilustrativas de la maqueta están insertadas dentro del archivo; los gráficos, la tabla de datos y el mapa por UGEL funcionan sin conexión.

**Secciones:** Inicio / Videorreportajes / Entrevistas / Datos. La sección Datos integra las siete visualizaciones del HTML analizado: Lima vs. Perú, comparación de tres años, tipos de violencia, serie mensual, actor, nivel EBR y mapa de las siete UGEL metropolitanas. Incluye selectores de ámbito, cifras/porcentajes, mensual/acumulado, y exportación CSV.

**Estado editorial:** Las introducciones de videorreportajes y las entrevistas son propuestas visuales, no piezas grabadas. Las fotos que venían en la maqueta se identifican como ilustraciones generadas con IA, no personas ni hechos reales.

**Fuente de los datos:** Se conservaron los cálculos y advertencias tal como aparecían en `Ojo-Critico-Graficos-Analizados(1).html`, a partir del Excel previamente analizado, con corte al 31 de octubre de 2026. El panel muestra **7.198** registros para Lima Metropolitana; antes de publicar conviene contrastar esta cifra con el **7.187** señalado en la consulta pública de SíseVe. No modificar el dato sin revisar definición, fechas y cobertura.

## Animaciones

La web usa CSS y JavaScript estándar para transiciones, revelación gradual de tarjetas, barras y columnas, fotos con movimiento sutil y secuencias visuales. El botón **Pausar animaciones** respeta también la preferencia de accesibilidad de reducir movimiento. No depende de servicios externos.

## HyperFrames: intro de video opcional

El archivo `motion/index.html` es una **composición para HyperFrames** (1920 × 1080, 8 segundos), con la estructura y el registro de timeline descritos en la documentación oficial. Es opcional: no es parte del motor de la página web.

Repositorio: <https://github.com/heygen-com/hyperframes>
Documentación: <https://hyperframes.app/docs/1-startup/2-quickstart>

Para instalar el proyecto oficial cuando tengas conexión a Internet, desde una terminal con Node.js 22+ y FFmpeg:

```bash
npx hyperframes init mi-intro --non-interactive --example blank
cd mi-intro
# Reemplaza el index.html creado por el archivo motion/index.html incluido aquí.
npx hyperframes preview
npx hyperframes render --output ojo-critico-intro.mp4
```

El ejemplo usa GSAP desde jsDelivr; se necesita conexión o una copia local de GSAP. **No se ha descargado ni distribuido el repositorio completo de HyperFrames** dentro del ZIP debido a las restricciones de acceso de red del entorno. Se entrega una composición preparada para su instalación y edición.

## Publicación

Es una maqueta autónoma. Para ponerla en un dominio, publica `index.html` como sitio estático (por ejemplo, Cloudflare Pages). Antes de publicarla, revisa y completa las fuentes, créditos, cifras y material audiovisual.
