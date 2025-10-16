# Invitación de Boda Digital

Una invitación de boda elegante y responsive diseñada para ser hospedada en GitHub Pages.

## Configuración del formulario RSVP

### Opción 1: Formspree (Recomendado - Fácil configuración)

1. Ve a [formspree.io](https://formspree.io)
2. Crea una cuenta gratuita
3. Crea un nuevo formulario
4. Copia el ID del formulario que te proporcionen
5. En `invitaciones_boda.html`, busca la línea:
   ```html
   <form id="rsvpForm" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```
6. Reemplaza `YOUR_FORM_ID` con tu ID real de Formspree

**Ventajas:**
- Gratuito hasta 50 envíos por mes
- Fácil configuración
- Recibes emails automáticamente
- Panel de administración web

### Opción 2: Google Forms + Google Sheets

1. Crea un Google Form con los campos necesarios
2. Configura las respuestas para que se guarden en Google Sheets
3. Reemplaza el action del formulario con la URL de tu Google Form

### Opción 3: Netlify Forms (Si cambias el hosting)

Si decides usar Netlify en lugar de GitHub Pages:
1. Sube tu proyecto a Netlify
2. Agrega `netlify` al atributo del formulario
3. Netlify manejará automáticamente los envíos

## Configuración de GitHub Pages

1. Sube todos los archivos a un repositorio de GitHub
2. Ve a Settings → Pages en tu repositorio
3. Selecciona la rama principal como fuente
4. Tu invitación estará disponible en: `https://tuusuario.github.io/nombre-repositorio`

## Personalización

### Cambiar colores
Los colores principales están definidos en las variables CSS:
- Verde principal: `#a8b8a0`
- Verde oscuro: `#8ea085`
- Verde texto: `#5a6b52`

### Agregar fotos reales
Reemplaza los elementos `.photo-placeholder` con:
```html
<img src="ruta-a-tu-foto.jpg" alt="Descripción" style="width: 100%; border-radius: 10px;">
```

### Modificar información
Edita directamente el HTML para cambiar:
- Nombres de los novios
- Fecha y hora
- Direcciones
- Información de contacto

## Estructura de archivos

```
InvitacionesBoda/
├── invitaciones_boda.html     # Invitación principal
├── invitaciones_boda_1.html   # Versiones alternativas
├── invitaciones_boda_2.html
├── invitaciones_boda_3.html
├── invitaciones_boda_4.html
├── invitaciones_boda_5.html
└── README.md                  # Este archivo
```

## Funcionalidades incluidas

- ✅ Diseño responsive (móvil y desktop)
- ✅ Contador regresivo automático
- ✅ Formulario de confirmación de asistencia
- ✅ Secciones para información completa de la boda
- ✅ Diseño elegante con tipografías web
- ✅ Compatible con GitHub Pages

## Soporte

El plan gratuito de Formspree permite 50 confirmaciones por mes. Si esperas más invitados, considera:
- Upgrading a un plan paid de Formspree ($10/mes)
- Usar Google Forms (ilimitado y gratuito)
- Implementar una solución con WhatsApp para confirmaciones

## Vista previa

Para ver la invitación localmente, simplemente abre `invitaciones_boda.html` en tu navegador web.
