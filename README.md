# Centralita CRM para Android

Identifica cada llamada entrante con los datos de tu CRM, incluso sin conexión. Cuando suena el teléfono, Centralita CRM muestra quién llama, de qué empresa es y en qué estado está su cuenta, antes de que descuelgues.

> Este repositorio contiene **solo la documentación pública** del producto: manual de uso, modelo de seguridad y gestión de incidencias. El código fuente es privado.

## Qué resuelve

| Problema | Cómo lo resuelve Centralita CRM |
| --- | --- |
| Atiendes llamadas sin saber quién es el cliente | Notificación con nombre, empresa y estado al sonar el teléfono |
| Buscar al cliente en el CRM durante la llamada te hace perder tiempo | Ficha disponible al instante, sin abrir el CRM |
| Sin cobertura no tienes datos | Caché local cifrada que funciona sin conexión |
| Las llamadas perdidas se olvidan | Tarjetas de llamadas pendientes con nota, llamada o WhatsApp en un toque |
| Los datos de clientes viajan y se almacenan en servidores de terceros | Cifrado de extremo a extremo: el servidor nunca ve los datos de tus clientes |

## Funcionalidades

- **Identificación de llamadas** entrantes y salientes con datos del CRM.
- **Funcionamiento sin conexión** con caché local cifrada y caducidad configurable.
- **Tarjetas de llamadas pendientes** con acciones rápidas: llamar, WhatsApp y añadir nota.
- **Búsqueda** por teléfono, nombre o empresa.
- **Historial de llamadas** y números ignorados.
- **Alta controlada de terminales**: cada dispositivo debe ser aprobado por el administrador.
- **Detección de llamadas en segundo plano**, también tras reiniciar el teléfono.

## Documentación

| Documento | Para quién |
| --- | --- |
| [Manual de uso](docs/manual-de-uso.md) | Personas que usan la app a diario |
| [Seguridad](docs/seguridad.md) | Responsables técnicos y de protección de datos |
| [Preguntas frecuentes](docs/preguntas-frecuentes.md) | Todos |

## Requisitos

- Teléfono Android con permisos de estado del teléfono, registro de llamadas y notificaciones.
- Una cuenta de CRM integrada y un terminal aprobado por el administrador de tu empresa.

## Incidencias y sugerencias

Abre una [incidencia](../../issues/new/choose) usando la plantilla correspondiente.

**Nunca incluyas en una incidencia** números de teléfono, nombres de clientes, capturas con datos reales, códigos de activación ni identificadores de tu terminal.
