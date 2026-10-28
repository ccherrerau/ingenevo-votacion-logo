# Votación del logo INGENEVO

Página pública para votar por la nueva imagen de INGENEVO. Se elige un tipo de letra y luego un color en una de dos versiones: un color o dos colores.

- **Votar:** https://ccherrerau.github.io/ingenevo-votacion-logo/
- **Solo resultados:** https://ccherrerau.github.io/ingenevo-votacion-logo/?ver=resultados

## Cómo funciona

- El voto se guarda en una base de datos (Supabase, tabla `votacion_logo`) en el momento en que se pulsa **Votar**.
- Cada voto exige un correo, y la base acepta un solo voto por correo, sin distinguir mayúsculas ni espacios. El correo no se verifica y nunca se publica.
- La página pide la lista completa de votos (número, letras, versión y color) y calcula los conteos en el navegador. La lista se puede ver en «Ver todos los votos».
- **Cierre: jueves 29 de octubre de 2026 a las 12:00 m. (hora de Colombia).** Lo impone la propia base de datos: desde esa hora rechaza cualquier voto nuevo, aunque alguien tenga la página abierta. Después del cierre la página solo muestra el resultado final.
- Todo el código está en `index.html`. No hay otro servidor ni otro código.

## Qué permite la llave pública de la página

| Acción | Permitida |
|---|---|
| Agregar un voto, con valores válidos y un correo no usado, antes del cierre | Sí |
| Ver letras, versión y color de cada voto | Sí |
| Ver correos, nombres, comentarios u hora del voto | No |
| Modificar o borrar votos | No |
