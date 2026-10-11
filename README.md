# 🧰 p_skills

**Mi colección personal de skills, reglas y estándares reutilizables para desarrollo de software.**

Este repositorio centraliza las skills de agentes de programación que utilizo, las reglas que definen mi forma de trabajar y las configuraciones que puedo reutilizar al iniciar nuevos proyectos.

La idea es evitar repetir instrucciones, mantener una calidad consistente y adaptar las herramientas a cada tecnología sin mezclar arquitecturas ni convenciones incompatibles.

Aunque el repositorio es público, su propósito principal es servirme como biblioteca personal de desarrollo.

---

## 🎯 Objetivos

- Centralizar las skills recopiladas de [skills.sh](https://skills.sh/).
- Organizar las skills por tecnología, especialidad y tipo de proyecto.
- Mantener reglas propias para backend, frontend, móvil, seguridad y testing.
- Reutilizar configuraciones entre proyectos sin duplicar trabajo.
- Documentar cómo instalar, actualizar y utilizar las skills.
- Registrar las herramientas, convenciones y decisiones que funcionan en mis proyectos.
- Mantener un catálogo organizado, fácil de consultar y ampliar.

## 🧱 Estructura del repositorio

```text
p_skills/
├── README.md
└── skills/
    ├── ...
    └── ...
```

La carpeta `skills/` contiene las skills organizadas y gestionadas en el repositorio. Su estructura interna puede evolucionar conforme incorpore nuevas tecnologías.

Las reglas generales y específicas de cada stack se irán documentando y organizando progresivamente.

## 🛠️ Tecnologías y perfiles

### Backend

| Perfil | Tecnologías | Uso |
|---|---|---|
| Django monolítico | Python, Django, Templates | Aplicaciones web tradicionales |
| Django + Vue CDN | Django, Vue 3, JavaScript | Monolito con interactividad progresiva |
| Django REST | Django REST Framework | APIs REST |
| FastAPI | Python, FastAPI, Pydantic | APIs y servicios |
| Express | Node.js, Express, TypeScript | APIs ligeras |
| NestJS | Node.js, NestJS, TypeScript | Backends modulares |

### Frontend

| Perfil | Tecnologías | Uso |
|---|---|---|
| React | React, JavaScript | Aplicaciones interactivas |
| React + TypeScript | React, TypeScript | Aplicaciones con tipado estático |
| Next.js | React, TypeScript, Next.js | Aplicaciones web full stack |
| Astro | Astro, HTML, CSS, JavaScript | Sitios de contenido y páginas rápidas |

### Desarrollo móvil

| Perfil | Tecnologías | Uso |
|---|---|---|
| Dart | Dart | Lenguaje y herramientas del ecosistema |
| Flutter | Flutter, Dart | Aplicaciones multiplataforma |

Los perfiles son independientes y se pueden combinar cuando la arquitectura lo requiera. No todas las skills deben instalarse en todos los proyectos.

## 📚 Categorías de skills

La colección puede organizarse en las siguientes categorías:

- **General:** buenas prácticas, código limpio y reutilización.
- **Backend:** arquitectura, APIs, autenticación, validación y acceso a datos.
- **Frontend:** componentes, estado, accesibilidad, rendimiento y experiencia de usuario.
- **Mobile:** arquitectura de aplicaciones, navegación, estado y rendimiento.
- **Database:** SQL, modelado, transacciones, índices y optimización.
- **Security:** autorización, protección de datos, gestión de secretos y dependencias.
- **Testing:** pruebas unitarias, integración y regresión.
- **DevOps:** Docker, CI/CD, despliegues y configuración de entornos.
- **Documentation:** documentación técnica, decisiones arquitectónicas y guías de uso.

## 📏 Mis principios de desarrollo

1. **Entender antes de modificar.** Revisar la estructura y las convenciones existentes antes de cambiar código.
2. **Simplicidad primero.** Evitar complejidad y abstracciones innecesarias.
3. **Separar responsabilidades.** Mantener clara la relación entre presentación, lógica de negocio y acceso a datos.
4. **Reutilizar con criterio.** Buscar implementaciones existentes antes de crear otras y evitar duplicación.
5. **Seguridad por defecto.** Validar entradas, verificar permisos y proteger credenciales y datos sensibles.
6. **Probar los cambios.** Ejecutar las comprobaciones disponibles y no asumir que el código funciona sin verificarlo.
7. **Documentar lo necesario.** Mantener instrucciones reproducibles para instalar, ejecutar y mantener los proyectos.
8. **Respetar el contexto.** No imponer una arquitectura, dependencia o tecnología que el proyecto no necesite.
9. **Mantener compatibilidad.** Revisar las versiones y las dependencias antes de proponer cambios.
10. **Entregar con transparencia.** Informar de los cambios realizados, las pruebas ejecutadas y las limitaciones pendientes.

## ⚙️ Uso de skills.sh

La CLI de skills.sh permite consultar, instalar y gestionar skills para agentes de programación compatibles.

### Consultar skills disponibles

```bash
npx skills find django
npx skills find react
npx skills find fastapi
npx skills find flutter
```

### Consultar un repositorio antes de instalar

```bash
npx skills add <repositorio> --list
```

### Instalar una skill para un proyecto

```bash
npx skills add <repositorio> --skill <nombre-skill>
```

### Instalar una skill globalmente

```bash
npx skills add <repositorio> --skill <nombre-skill> -g
```

### Consultar las skills instaladas

```bash
npx skills list
```

### Actualizar las skills

```bash
npx skills update
```

Los nombres de las skills y los repositorios deben comprobarse en el catálogo antes de instalarlos. No todas las skills están disponibles para todos los agentes.

Catálogo: https://skills.sh/

Documentación de la CLI: https://github.com/vercel-labs/skills

## 🔄 Flujo de trabajo para nuevos proyectos

1. Identificar el stack y el objetivo del proyecto.
2. Seleccionar las skills generales necesarias.
3. Añadir las skills específicas del framework.
4. Revisar las instrucciones de cada skill antes de utilizarla.
5. Incorporar las reglas generales y las específicas del proyecto.
6. Verificar que no existan instrucciones contradictorias.
7. Implementar y probar las funcionalidades.
8. Actualizar las reglas cuando se identifiquen mejoras reutilizables.

### Ejemplo

Para iniciar una aplicación monolítica con Django y Vue por CDN:

- Skills generales de Python y seguridad.
- Skills específicas de Django.
- Skills de Vue adaptadas al uso de CDN.
- Reglas para templates, formularios, CSRF y separación de lógica.
- Pruebas de modelos, vistas, permisos y funcionalidades críticas.

No es necesario instalar skills de React, Next.js o Flutter para este perfil.

## 🔐 Seguridad y mantenimiento

Antes de incorporar una skill:

- Revisar su documentación e instrucciones.
- Comprobar los scripts, comandos y dependencias que incluya.
- Evitar ejecutar código desconocido sin revisarlo.
- No incluir tokens, claves privadas, contraseñas ni archivos `.env` reales.
- Comprobar las licencias y condiciones de redistribución antes de publicar contenido de terceros.
- Mantener identificadas las skills originales y las reglas creadas personalmente.

Las skills pueden cambiar con el tiempo. Conviene revisar las actualizaciones y comprobar que sigan siendo compatibles con las herramientas utilizadas.

## 🌱 Mejoras futuras

- [ ] Crear un archivo `AGENTS.md` con mis reglas generales.
- [ ] Definir reglas reutilizables para backend, frontend y móvil.
- [ ] Organizar las skills por perfiles de proyecto.
- [ ] Documentar los comandos de instalación de cada perfil.
- [ ] Crear plantillas para nuevos proyectos.
- [ ] Añadir convenciones de nombres y estructura de carpetas.
- [ ] Definir estándares de testing, seguridad y documentación.
- [ ] Registrar las skills verificadas y las que requieren revisión.
- [ ] Automatizar las comprobaciones de calidad cuando sea conveniente.

## 📌 Filosofía

Este repositorio no busca acumular skills indiscriminadamente, sino construir una biblioteca útil, mantenible y coherente.

**Menos instrucciones repetidas, más reutilización, mejores proyectos y una forma de trabajar consistente.**

---

Repositorio personal de desarrollo. Abierto para consulta, aprendizaje y colaboración.