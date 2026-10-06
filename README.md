# Breixo A. Herrera

**Sistemas y desarrollo en turismo.** Construyo y mantengo la tecnología que hay detrás de la venta de entradas y tours: integraciones con plataformas de reserva, automatización en Salesforce, OCR de documentos, extensiones para el equipo de operaciones e infraestructura.

> *Systems & software for a tour operator: booking-platform integrations, Salesforce automation, document OCR, internal tooling and infrastructure.*

## Lo que hago

- **Integraciones**: Regiondo, FareHarbor, Turitop, Ventrata, HubSpot, Google Things To Do, Google Places, OCI Document Understanding.
- **Salesforce**: Apex (triggers, Queueable, Batch, REST, webhooks OCTO), Custom Metadata, Named Credentials y Visualforce, además de facturación REAV con Holded.
- **Backend y herramientas**: Node.js/Express, Python, extensiones de Chrome (MV3), PHP/WordPress y PowerShell.
- **Infraestructura**: Linux, nginx/Caddy, systemd, Docker, Oracle Cloud y AWS, además de backups, VPN y DNS.

Desde 2025 he cerrado **más de 130 proyectos** internos, de incidencias de un día a sistemas que usan a diario el equipo de operaciones y los clientes.

## Proyectos destacados

| | Proyecto | Stack | En una línea |
|---|---|---|---|
| 🎟️ | [**reserva-checker**](https://github.com/BreixoHR/reserva-checker) | Chrome MV3 · Apex REST | Antes de comprar entradas en la web oficial, comprueba contra el CRM que la fecha coincide con la reserva. Funciona en 10 webs con 3 estrategias de adaptador. |
| 📄 | [**ticket-date-ocr**](https://github.com/BreixoHR/ticket-date-ocr) | Node · OCI OCR · Apex | Lee la fecha de visita de las entradas en PDF, en 4 idiomas, y la contrasta con la reserva. Incluye circuit breaker, cola, fallback a la capa de texto y extracción de fechas por etiquetas. |
| 📥 | [**ticket-delivery-addon**](https://github.com/BreixoHR/ticket-delivery-addon) | Node · Express · SQLite | Entrega de entradas sin exponer el origen, con tokens de un solo uso y caché. Clona el header y el footer de cualquier web anfitriona. |
| ☁️ | [**salesforce-booking-ops**](https://github.com/BreixoHR/salesforce-booking-ops) | Apex | Conciliación diaria entre la plataforma de venta y el CRM, enrutado de incidencias por producto y migración de ficheros. |
| 🗺️ | [**things-to-do-feed-builder**](https://github.com/BreixoHR/things-to-do-feed-builder) | Node · JS | Editor de feeds para Google Things To Do con validación de la especificación. Arregla una condición de carrera que perdía 49 de cada 50 altas simultáneas. |
| 🛡️ | [**booking-captcha-gate**](https://github.com/BreixoHR/booking-captcha-gate) | WordPress · PHP | Frena las reservas falsas hechas por bots: el widget de reservas solo se entrega tras verificar reCAPTCHA en el servidor. |
| 🧾 | [**salesforce-reav-invoicing**](https://github.com/BreixoHR/salesforce-reav-invoicing) | Apex · Holded API | Facturación en régimen especial de agencias de viajes (IVA solo sobre el margen), con rectificativas y varias empresas emisoras. Corrige bugs de la versión en producción: rectificativas con totales positivos y categorías sobrescritas. |
| 🐍 | [**booking-catalog-export**](https://github.com/BreixoHR/booking-catalog-export) | Python (stdlib) | Catálogo y tarifas de Regiondo (HMAC) y TuriTop (OAuth) exportados a JSON, CSV y Things To Do, con clasificación multilingüe de tipos de cliente. |
| 🏗️ | [**systems-case-studies**](https://github.com/BreixoHR/systems-case-studies) | Infra · Node | 8 casos reales: contingencia en OCI, auditoría de rendimiento, migración SEO, QA de integraciones, red, sala de servidores, Google Tag Gateway y archivado. Incluye 2 herramientas testeadas. |
| ⚙️ | [**tourism-automation-scripts**](https://github.com/BreixoHR/tourism-automation-scripts) | PowerShell · Pester | Datos de Google Places para Things To Do, locuciones de audioguías con TTS y reinicio ordenado de servicios. |

Todos los proyectos tienen tests automatizados y CI, y su README explica el problema real, las decisiones de diseño y **qué fallaba en la versión anterior y cómo se corrigió**.

## Cómo trabajo

- **Cada proyecto es una "obra" documentada**: requisitos, correos, versiones y releases, y documentación técnica. Así cualquiera puede retomar un sistema sin depender de mí.
- **Primero que funcione, después que sea robusto**: muchos de estos sistemas nacieron como una solución urgente y crecieron con los incidentes. Las versiones publicadas aquí son la consolidación de esas lecciones: tests, gestión de secretos y resiliencia.
- **La seguridad, por defecto**: nada de credenciales en el código, mínimos privilegios y verificación en el servidor.

