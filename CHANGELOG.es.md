# Registro de cambios

## 0.5.0 - 14/04/2025

### Nuevas Funcionalidades
- Componente `DevilProgressBar` mejorado con efectos visuales avanzados:
  - Añadidos efectos de energía fluida para todos los estilos de variantes
  - Implementados efectos de brillo dinámicos que se mueven con el progreso
  - Añadidas animaciones de partículas y ondas de energía para la variante estilizada
  - Añadidos efectos de pulso receptivos para la variante royal

### Mejoras
- Animaciones de barras de progreso completamente rediseñadas:
  - Eliminados problemas visuales en las variantes stylized y royal
  - Mejorada la continuidad visual durante las transiciones de progreso
  - Mejorados los efectos específicos de cada tema (ej., efectos de fuego de Dante, estética de precisión de Vergil)
  - Añadidas capas de profundidad para una apariencia más profesional

### Mejoras Técnicas
- Sistema de animación CSS refactorizado para un mejor rendimiento:
  - Separado el seguimiento de progreso de los efectos visuales
  - Utilizadas técnicas adecuadas de capas para animaciones superpuestas
  - Implementadas animaciones aceleradas por hardware con propiedades transform
  - Keyframes optimizados para transiciones más suaves

## 0.4.0 - 12/04/2025

### Nuevas Funcionalidades
- Añadidas variantes de tamaño para el reproductor:
  - Cuatro tamaños disponibles: sm, md, lg, xl
  - Escalado responsivo de todos los elementos, incluyendo controles y fuentes
  - Espaciado y proporciones específicas para cada tamaño
- Añadidas opciones de posicionamiento central:
  - Nuevas posiciones top-center y bottom-center
  - Manejo especial para el estado minimizado centrado

### Mejoras
- Mejorado el contraste en todos los temas de personajes para una mejor accesibilidad

## 0.3.0 - 11/04/2025

### Nuevas Funcionalidades
- Añadidos temas de personajes de Devil May Cry con estilos visuales únicos:
  - Dante: Rojo con acentos dorados y efectos de fuego
  - Vergil: Azul con precisión y estética afilada
  - Nero: Azul brillante con energía roja del Devil Breaker
  - V: Púrpura con acentos turquesa y estilo poético
  - Trish: Dorado con detalles eléctricos en púrpura
  - Lady: Rojo oscuro con acentos negros
  - Nico: Naranja/marrón con estética mecánica
  - Sparda: Rojo oscuro con efectos legendarios dorados
- Implementadas opciones de personalización de fondo:
  - Soporte para color de fondo personalizado
  - Opacidad de fondo ajustable
  - Desenfoque de fondo configurable
- Añadido soporte de color de acento para elementos interactivos y animaciones

### Mejoras
- Refactorización completa de la arquitectura CSS para mejor mantenibilidad:
  - Estructura modular con archivos separados para estilos base, layouts, controles y animaciones
  - Archivos de tema individuales para cada personaje de DMC
  - Mejor organización de variables CSS
- Mejora del feedback visual para elementos interactivos
- Mejora del contraste y accesibilidad en todos los temas
- Añadidos efectos especiales y animaciones únicas para cada personaje
- Mejor documentación para todas las opciones de personalización

### Mejoras Técnicas
- División del código CSS para mejor mantenibilidad
- Sistema de temas mejorado con variables CSS
- Mejor validación y documentación de props
- Manejo mejorado del color con cálculos de valores RGB para efectos de opacidad

## 0.2.0 - 08/04/2025

### Mejoras
- Cambiado el valor predeterminado de `triggerWord` a `null`, evitando activaciones accidentales durante la escritura normal
- Mejorado el comportamiento del popup de control de volumen con cierre automático:
  - Se cierra al hacer clic fuera del popup
  - Se cierra al presionar la tecla ESC
  - Se cierra automáticamente cuando el ratón está fuera del área durante 2 segundos
- Limpieza adecuada de temporizadores y escuchadores de eventos para evitar fugas de memoria

### Correcciones
- Eliminada la duplicación de la interfaz `AudioDevilTriggerProps` utilizando una única fuente de verdad en `types/index.ts`

## 0.1.0 - 07/04/2025

- Lanzamiento inicial del módulo React Devil Trigger
- Componente de reproductor de audio React personalizable
- Detección de secuencias de teclado para Easter eggs y características ocultas
- Soporte para TypeScript y definiciones de tipos
- Sistema de construcción basado en Rollup para una distribución optimizada