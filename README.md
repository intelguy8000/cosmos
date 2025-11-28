# Cosmo Schools Demo - Propuesta Agentes IA

Demo interactivo para presentar a Cosmo Schools la propuesta de reemplazar su bot actual con agentes de IA conversacionales.

## URLs

- **Demo en producción:** https://cosmo-schools-demo.vercel.app/
- **Repositorio GitHub:** https://github.com/intelguy8000/cosmos

## Problema que resuelve

El bot actual de Cosmo Schools tiene:
- 24 preguntas antes de saber si hay cupo
- +15 minutos de proceso
- Sin alternativas cuando no hay cupo exacto
- Experiencia frustrante para los padres

**Resultado actual:** 7,282 inscripciones → 1,003 matrículas (13.7% conversión)

## Solución propuesta

Sistema de 4 agentes IA especializados:

| Agente | Rol | Descripción |
|--------|-----|-------------|
| **María** | Asesora | Asesora de registro, logra que las personas ingresen al proceso y filtra |
| **Tati** | Agenda | Gestiona el agendamiento y pago de inmersión |
| **Sara** | FAQ | Responde preguntas y te lleva al siguiente paso |
| **Juli** | Closer | La closer, logra que se cierren nuevas matrículas |

**Meta:** Alcanzar +25% de conversión

## Estructura del Demo

El demo es un archivo HTML único (`index.html`) que incluye:

### Secciones visibles:
1. **Header** - Logos Loopera + Cosmo Schools
2. **Stats Bar** - Métricas actuales (rosa Cosmo)
3. **Hero** - Propuesta de valor principal
4. **Chat Comparador** - Bot actual vs Agentes IA (lado a lado)
5. **Métricas** - Cards con KPIs de mejora
6. **Diagrama de Etapas** - Funnel de conversión
7. **Comparación Multi-Agente** - Diagrama SVG interactivo
8. **Problemas Actuales** - 3 cards con soluciones
9. **Principios de Diseño** - Framework agnóstico + Base reutilizable
10. **Infraestructura Técnica** - Diagrama de capas (Canales → Agentes → Modelos → Datos)
11. **Arquitectura Propuesta** - Flujo simple WhatsApp → María → Tati → CRM
12. **Alcance de Implementación** - Timeline vertical con 2 fases
13. **Modelo de Implementación** - Timeline horizontal de 4 etapas
14. **CTA** - Llamado a acción final

### Secciones ocultas:
- **Quick Win** - Mejora del botón WhatsApp (oculta con `display: none`)

## Stack Técnico

- **Frontend:** HTML + CSS + JavaScript (vanilla)
- **Fuentes:** Space Grotesk (Google Fonts)
- **Hosting:** Vercel
- **Repositorio:** GitHub

## Comandos útiles

```bash
# Ver cambios locales
open index.html

# Deploy a producción
vercel --prod

# Commit y push
git add . && git commit -m "mensaje" && git push
```

## Colores principales

```css
--cosmo-pink: #E91E63;      /* Rosa Cosmo - color principal */
--cosmo-blue: #1e3a5f;      /* Azul oscuro - textos */
--success-green: #22c55e;   /* Verde - éxito/positivo */
--whatsapp-green: #25D366;  /* Verde WhatsApp */
--bg-cream: #faf8f5;        /* Fondo crema */
```

## Cambios recientes

- Nombres de agentes: María, Tati, Sara, Juli
- Logo WhatsApp real (SVG verde) en todas las secciones
- Dashboard Loopera en vez de Looker
- Sin Botpress en capa de mensajería
- Sección Quick Win oculta

## Para mostrar Quick Win nuevamente

En el CSS, buscar `.quickwin-section` y quitar `display: none;`

```css
/* Quick Win Section - HIDDEN */
.quickwin-section {
    display: none;  /* <-- Quitar esta línea */
    padding: 4rem 2rem;
    ...
}
```

## Contacto

Proyecto desarrollado por Loopera para Cosmo Schools.
