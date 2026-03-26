# Reflexión Actividad 6.5

## 1. ¿Para qué sirve git rebase -i?

El comando `git rebase -i` (rebase interactivo) sirve para modificar el historial de los commits para controlarlos. esto permite cambiar mensajes, combinar commits, eliminarlos o reordenarlos.

Su principal ventaja es que permite mantener un historial limpio, organizado y facil de entender, en lugar de tener muchos commits pequeños.

## 2. Ejemplos de uso

### reword
Se usa cuando se quiere cambiar el mensaje de un commit sin cambiar su contenido.
Ejemplo: cambiar "wip" por "Añade funcionalidad de login".

### squash
Se usa para combinar varios commits en uno solo.
Ejemplo: unir varios commits pequeños de pruebas en un unico commit final mas claro.

### drop
Se usa para eliminar un commit del historial.
Ejemplo: eliminar un commit que añade codigo innecesario o que no funciona.

---

## 3. Riesgos de usar git rebase -i

El principal riesgo es que reescribe el historial de commits. Si se usa en ramas que ya han sido compartidas con otros puede causar conflictos y problemas.

Por eso, se recomienda usarlo solo en ramas locales o antes de hacer push.