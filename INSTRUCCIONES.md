# TDM Landing Page - Instrucciones de Instalación

## Requisitos previos
- Node.js 18+ instalado (https://nodejs.org)
- npm o yarn

## Pasos para ejecutar

1. Abre la terminal en la carpeta `tdm-landing`
2. Instala dependencias:
   ```
   npm install
   ```
3. Inicia el servidor de desarrollo:
   ```
   npm run dev
   ```
4. Abre en el navegador: http://localhost:3000

## Para producción
```
npm run build
npm start
```

## Personalización rápida

### Cambiar número de WhatsApp
Buscar en todos los archivos: `18097888434`
Reemplazar con el número en formato internacional (sin espacios ni guiones).

### Cambiar textos
Los textos están en cada componente dentro de `components/`:
- `Hero.tsx` - Sección principal
- `Stats.tsx` - Estadísticas
- `Problems.tsx` - Sección de problemas
- `Services.tsx` - Servicios
- `Compare.tsx` - Comparador renta vs compra
- `SavingsCalculator.tsx` - Calculadora de ahorro
- `Testimonials.tsx` - Testimonios
- `AIChatPreview.tsx` - Asistente virtual
- `FAQ.tsx` - Preguntas frecuentes
- `MapSection.tsx` - Ubicación
- `FinalCTA.tsx` - Llamada a acción final
- `FloatingWhatsApp.tsx` - Botón flotante
- `Footer.tsx` - Pie de página

### Agregar mapa real de Google Maps
En `MapSection.tsx`, reemplaza el SVG placeholder con:
```tsx
<iframe
  src="TU_URL_DE_GOOGLE_MAPS_EMBED"
  width="100%"
  height="360"
  style={{ border: 0 }}
  allowFullScreen
  loading="lazy"
/>
```

### Cambiar estadísticas
En `Stats.tsx`, editar el array `stats` con los valores reales de tu empresa.

### Cambiar testimonios
En `Testimonials.tsx`, editar el array `testimonials` con testimonios reales.
