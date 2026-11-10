# UNINCCA Tracker

Panel de seguimiento académico (GitHub Pages) con actividades pendientes por materia, grabaciones y resúmenes de clase.
Sitio: https://vaocantod-creator.github.io/unincca-tracker/

## Cómo funciona hoy
- Un cron (10:00 y 22:00, hora de Colombia) revisa Moodle, regenera la tabla de pendientes y publica.
- Desde el 5 de noviembre de 2026 el cron también transcribe las clases grabadas y publica un resumen por clase en el panel de cada materia.
- Con una cuenta **@unincca.edu.co** (Google) cada estudiante guarda **su propio estado** («Hecho/Pendiente») y **sus propias notas** por actividad; solo él las ve.
  Sin sesión, se guardan únicamente en el navegador.
- Los datos de Moodle (pendientes, grabaciones, resúmenes) salen de la cuenta del propietario y son **compartidos**: todos los estudiantes ven los mismos.

## Próximas mejoras
1. **Secciones por materia y resúmenes detrás de login.** Hoy viajan dentro del HTML público; ocultarlas con la interfaz no es una barrera real.
   Plan: mover ese contenido a una tabla de Supabase con acceso solo para cuentas @unincca.edu.co, y que la página lo pida tras iniciar sesión.
2. Seguimiento verdaderamente personal (entregas y notas de cada estudiante en Moodle): requiere el consentimiento y el acceso de cada persona; sin diseñar todavía.
