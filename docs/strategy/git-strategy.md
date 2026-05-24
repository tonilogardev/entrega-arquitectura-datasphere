# Estrategia de Control de Versiones (DataSphere)

**Archivo:** `strategy/git-strategy.md`

Esta estrategia define las directrices del repositorio para garantizar la trazabilidad y limpieza del proyecto:

1. **Nomenclatura de commits:** Aplicación estricta del estándar *Conventional Commits* (ej. `docs(auth): add JWT flow`) para mantener un historial semántico, predecible y automatizable.
2. **Estructura de carpetas:** Organización modular por dominios (`/architecture`, `/auth`, `/http`, `/strategy`), garantizando que cada pieza de documentación esté aislada en su contexto lógico.
3. **Reglas de exclusión (.gitignore):** Queda terminantemente prohibido versionar credenciales (API Keys, archivos `.env`), dependencias locales y ficheros masivos de datos (archivos ZIP o SAFE de Copernicus).
4. **Separación de entregables:** Cada tarea de la actividad se empaqueta en *commits* atómicos e independientes. Esto permite aislar los cambios y facilita la auditoría o la ejecución de reversiones (`git revert`) si una funcionalidad falla.