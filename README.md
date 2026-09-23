# Taller Integrador — Buenas Prácticas de Desarrollo de Software

**Hernán Santiago Alvarino Ríos**

## Auditoría y corrección

| Defecto encontrado | Por qué era un problema | Cómo lo corrigió |
|---|---|---|
| Nombres de archivo con espacios y mayúsculas (`Mi Pagina De Notas.HTML`, `Estilos Del Sitio.CSS`) | Los espacios y mayúsculas en nombres de archivo generan errores en servidores sensibles a mayúsculas/minúsculas y no siguen la convención estándar | Se renombraron a `index.html` y `styles.css` |
| Título de la pestaña `<title>pagina</title>` | No describe el contenido de la página | Se cambió a `Calculadora de Promedio` |
| Variables de una sola letra (`a`, `b`, `c`) | No indican qué almacenan; obligan a leer todo el código para entenderlas | Se renombraron a `nota1`, `nota2`, `nota3` |
| Variable `x = 3` como número mágico | El significado de `3` no es evidente sin contexto | Se reemplazó por la constante `CANTIDAD_NOTAS` |
| Variable `TempValue2` | Nombre genérico que no comunica su propósito | Se renombró a `promedio` |
| Variable `data1 = []` sin uso en el código | Código muerto que confunde a quien lee el archivo | Se eliminó por no cumplir ninguna función |
| Función `calc()` | Nombre poco descriptivo de lo que hace la función | Se renombró a `calcularPromedio()` |
| IDs del HTML (`n1`, `n2`, `n3`, `r`, `r2`) | No describen qué representa cada elemento | Se renombraron a `nota1`, `nota2`, `nota3`, `resultado`, `resultadoEstado` |
| Evento `onclick="calc()"` en línea dentro del HTML | Mezcla el manejo del evento directamente en el atributo HTML, dificultando el mantenimiento | Se reemplazó por `addEventListener` dentro del `<script>` |
| Bloque de código comentado (`calcularAntiguo`) | Código muerto que no aporta nada y ensucia el archivo | Se eliminó |
| Sentencias `console.log` de depuración dejadas en el código | No deben quedar en código listo para producción | Se eliminaron |

## Enlaces

- Repositorio en GitHub: `https://github.com/hernansantiagoalvarinorios-hue/taller-integrador-ALVARINO-HERNAN/tree/main`
- Sitio publicado en Netlify: `https://unrivaled-choux-bb5917.netlify.app/`
