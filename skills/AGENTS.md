# Reglas generales de desarrollo

## 1. Antes de programar
- Inspeccionar la estructura existente, las instrucciones del proyecto y las dependencias.
- Identificar el framework, las convenciones y las pruebas disponibles.
- Proponer cambios pequeños y coherentes con la arquitectura existente.
- No reemplazar archivos ni reescribir módulos completos sin necesidad.
- Buscar código reutilizable antes de crear componentes, servicios o utilidades nuevos.

## 2. Calidad del código
- Aplicar principios SOLID, DRY y separación de responsabilidades cuando aporten valor.
- Evitar duplicación, funciones demasiado extensas y abstracciones prematuras.
- Usar nombres descriptivos y convenciones propias del lenguaje.
- Evitar dependencias innecesarias y código muerto.
- No dejar implementaciones incompletas, TODO ni placeholders en funcionalidades solicitadas.

## 3. Arquitectura
- Separar presentación, lógica de negocio y acceso a datos según la complejidad del proyecto.
- Mantener las reglas de negocio fuera de los controladores y componentes de interfaz.
- Organizar módulos por funcionalidad o dominio cuando resulte apropiado.
- No introducir microservicios ni capas adicionales sin una necesidad real.
- Reutilizar contratos, tipos y validadores existentes.

## 4. Seguridad
- Validar toda entrada no confiable en el servidor.
- Aplicar autorización en cada operación protegida.
- No exponer secretos, tokens, contraseñas ni datos privados en el cliente o los logs.
- Usar variables de entorno y mantener los archivos de secretos fuera del control de versiones.
- Aplicar las protecciones específicas del framework para CSRF, XSS, inyección y sesiones.
- No confiar en validaciones realizadas exclusivamente en el frontend.

## 5. Errores y observabilidad
- Gestionar los errores de forma consistente y comprensible.
- No ocultar excepciones ni devolver errores exitosos cuando una operación falla.
- Registrar información útil para depurar sin incluir credenciales ni datos sensibles.
- Diferenciar errores de validación, autorización, recursos inexistentes y fallos internos.

## 6. Pruebas y verificación
- Añadir pruebas para la lógica de negocio y los casos límite.
- Cubrir permisos, validaciones y errores relevantes.
- Ejecutar las pruebas y comprobaciones disponibles después de cambios significativos.
- No afirmar que una prueba pasó si no se ejecutó.
- Corregir regresiones antes de dar por terminada una tarea.

## 7. Dependencias y documentación
- Revisar las dependencias existentes antes de agregar otras.
- No actualizar paquetes ni cambiar versiones sin una razón.
- Documentar configuración, comandos de ejecución y decisiones arquitectónicas relevantes.
- Mantener los archivos de ejemplo de entorno libres de secretos reales.

## 8. Entrega
- Resumir qué se cambió y por qué.
- Indicar las pruebas ejecutadas y sus resultados.
- Declarar cualquier limitación o tarea pendiente de forma explícita.
- No modificar archivos ajenos a la tarea sin justificación.