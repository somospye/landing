# Guía de Contribución

¡Bienvenido a la guía de contribución de nuestra **Landing Page**!
Antes de comenzar, asegurate de leer y seguir todas las instrucciones de este documento para que tu colaboración pueda integrarse sin problemas.

---

## Preparar el entorno

1. **Haz un fork** del repositorio desde el botón `Fork` en la parte superior.

2. **Clona tu fork en local**:

```bash
git clone https://github.com/TU_USUARIO/landing
cd landing
```

3. **Instala las dependencias**:

```bash
bun install
```

4. **Configura lefthook**:

```bash
bun run prepare
```

Esto instala los hooks de Lefthook para validar commits, lint y formato automáticamente.

---

## Convenciones de Commits

Usamos [Conventional Commits](https://www.conventionalcommits.org/) para mantener un historial de cambios claro y estandarizado.

### Estructura del mensaje

```
tipo(ámbito): descripción corta

[cuerpo opcional]

[footer opcional]
```

### Tipos permitidos

- `feat`: Nueva funcionalidad
- `fix`: Corrección de bug
- `docs`: Cambios en documentación
- `style`: Formato, punto y coma, etc.
- `refactor`: Refactorización de código
- `perf`: Mejora de rendimiento
- `chore`: Cambios que no afectan al funcionamiento de la web

### Ejemplos

```
feat(navbar): add new navigation link

Add the new navigation link 'About' to the navbar.

BREAKING CHANGE: Added a new link to the navbar
```

---

## Linting y Formato

Antes de hacer commit, asegúrate de que tu código pase las validaciones de Biome:

```bash
# Verificar formato y errores
bun run format:check

# Corregir formato automáticamente
bun run format
```

---

## Pull Requests

1. Crea una rama:

```bash
git checkout -b feature/nueva-funcionalidad
```

2. Haz tus cambios y commits

3. Abre un PR hacia `main`

---

## ¡Gracias por contribuir!
