# XOCOCAD - Aplicación de Diseño Asistido por Computadora

XOCOCAD es una aplicación completa de CAD (Computer-Aided Design) que funciona directamente en el navegador web. Esta herramienta permite a los usuarios crear y manipular diseños técnicos 2D con precisión profesional, sin necesidad de instalar software adicional.


https://xococode.github.io/xoxocad/

## Características Principales

### Herramientas de Dibujo Geométrico
- **Líneas**: Creación de segmentos rectos entre dos puntos
- **Círculos**: Definición mediante centro y radio
- **Arcos**: Dos métodos distintos:
  - Arco por 3 puntos (inicio, punto intermedio, fin)
  - Arco por centro, inicio y fin (con dirección configurable)
- **Splines**: Curvas suaves con múltiples opciones de interpolación:
  - Cardinal (por defecto)
  - Lineal (segmentos rectos)
  - Bezier (con puntos de control)
  - Catmull-Rom
- **Puntos**: Colocación de puntos individuales
- **Rectángulos**: Creación mediante esquinas opuestas
- **Elipses**: Definición mediante centro y radios X/Y
- **Polígonos Regulares**:
  - Hexágonos
  - Estrellas (con número de puntas configurable)

### Herramientas de Edición y Transformación
- **Selección**: Selección individual o múltiple de objetos
- **Edición de Puntos**: Modificación directa de los puntos de control de cualquier objeto
- **Rotación**: Rotación precisa de objetos alrededor de un centro definido
- **Escala**: Cambio de tamaño proporcional de objetos
- **Equidistancia (Offset)**: Creación de copias paralelas (líneas) o concéntricas (círculos)
  - Opciones para lado izquierdo, derecho o ambos
  - Distancia configurable
- **Recortar (Trim)**: Eliminación de partes de objetos usando otros como límites
- **Alargar (Extend)**: Extensión de líneas hasta su intersección con otros objetos

### Acotación
- **Cotas Horizontales**: Medición de distancias horizontales
- **Cotas Verticales**: Medición de distancias verticales
- **Cotas de Radio**: Medición del radio de círculos con líneas directrices

### Ayudas al Dibujo
- **Snap a Objetos**: Referencias automáticas a puntos significativos:
  - Puntos finales
  - Puntos medios
  - Centros
  - Cuadrantes
  - Intersecciones
  - Tangentes
  - Puntos cercanos
- **Snap a Rejilla**: Alineación con una cuadrícula regular
- **Modo Ortogonal**: Restricción a movimientos horizontales y verticales
- **Indicadores Visuales**: Símbolos y textos que muestran el tipo de snap activo

### Navegación y Visualización
- **Zoom**: Ampliación/reducción mediante rueda del ratón
- **Paneo**: Desplazamiento de la vista (botón central o Alt+clic)
- **Interfaz Ajustable**: Modo compacto/completo para optimizar el espacio de trabajo

## Interfaz de Usuario

La interfaz está diseñada siguiendo patrones familiares de aplicaciones CAD profesionales:

- **Barra Superior**: Contiene todas las herramientas organizadas por categorías
- **Controles Específicos**: Aparecen dinámicamente según la herramienta seleccionada
- **Panel de Referencias**: Permite activar/desactivar distintos tipos de snap a objetos
- **Área de Dibujo**: Lienzo principal con rejilla opcional
- **Indicador de Estado**: Muestra información contextual sobre la herramienta actual
- **Indicadores Visuales**: Para snap, transformaciones y operaciones en curso

## Implementación Técnica

La aplicación está desarrollada en JavaScript puro y utiliza el elemento Canvas de HTML5 para el renderizado, sin dependencias externas. Implementa:

- Sistema de coordenadas con transformación entre espacio de pantalla y mundo
- Cálculos geométricos precisos para intersecciones y operaciones
- Gestión de estado para herramientas multi-paso
- Sistema de selección y manipulación de objetos
- Detección de puntos significativos para snap
- Previsualización en tiempo real de operaciones
- Modo de edición de puntos con manipuladores visuales
- Soporte para dispositivos de alta resolución (HiDPI/Retina)

## Ventajas

- **Sin Instalación**: Funciona directamente en el navegador
- **Ligera**: No requiere plugins ni bibliotecas externas
- **Interfaz Familiar**: Similar a software CAD profesional
- **Completamente Interactiva**: Previsualización en tiempo real
- **Precisa**: Herramientas de snap y ayudas para dibujo exacto
- **Responsive**: Se adapta a diferentes tamaños de pantalla

XOCAD representa una implementación web sofisticada de conceptos de CAD tradicionales, ofreciendo gran parte de la funcionalidad que se esperaría en aplicaciones de escritorio, pero con la ventaja de accesibilidad inmediata que proporciona el navegador web.
