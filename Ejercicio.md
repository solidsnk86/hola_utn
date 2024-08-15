# Tags

Añadir tags en Git Bash

Para añadir las tags debemos escribir el siguiente bash:
```bash
# Crear una nueva etiqueta
git tag v1.0

# Opcional: Añadir un mensaje a la etiqueta
git tag -a v1.0 -m "Versión 1.0"

# Enviar las etiquetas al remoto
git push --tags
```

### Para qué sirve:

- Compartir versiones: Las etiquetas se usan comúnmente para marcar versiones específicas de tu software (por ejemplo, v1.0, v2.1, etc.).
- Sincronización: Asegura que todas las etiquetas locales se compartan con el repositorio remoto.
- Colaboración: Permite a otros desarrolladores acceder a puntos específicos en la historia del proyecto.
- Releases: Facilita la gestión de releases y versiones en plataformas como GitHub o GitLab.

### Puntos importantes:
```bash
git push origin --tags
```
Este comando envía todas las etiquetas locales que no existen en el remoto.
No elimina etiquetas del remoto que ya no existen en local.
Es útil después de crear nuevas etiquetas localmente.