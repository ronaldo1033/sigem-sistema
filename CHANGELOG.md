# Historial de versiones

## [v3.0.0] - 2026-10-22

- Módulo de pagos y cobranzas: Ventas registra pagos en efectivo, transferencia, depósito, Yape, Plin o tarjeta (POS) con su número de operación y emite recibos en PDF; el cliente ve el saldo de sus contratos y reporta sus pagos desde *Mis pagos*; Ventas los confirma o rechaza y solo ADMIN anula recibos.
- Estado de pago (pendiente, parcial, pagado) en el listado y el detalle de contratos; reporte de cobranzas en Excel y PDF.
- Importación de repuestos desde Excel con plantilla descargable.
- Respaldos automáticos y a pedido de la base de datos (pg_dump o JDBC).
- Correcciones: error 500 en *Mis cotizaciones* y *Mis contratos* del portal cliente; rechazo de cotizaciones por POST con token CSRF; la página de acceso denegado acepta POST.
- 63 pruebas automatizadas (17 nuevas del módulo de pagos).

> SIGEM no procesa cobros: registra y valida los pagos hechos por los medios habituales.

## [v1.0.0] - 2026-10-21

Primera versión integrada de SIGEM (Sistema Integral de Gestión de Flotas y Maquinaria).

- Se incorpora el proyecto Spring Boot/Maven y su configuración de ejecución.
- Se incluye la implementación existente de los módulos, vistas, recursos estáticos y pruebas.
- Se conserva la documentación técnica, inventario documental y evidencias incluidas en el proyecto entregado.
- Se agregan instrucciones de colaboración y publicación para el repositorio.

> Esta etiqueta identifica la primera versión publicada del contenido recibido. No representa una auditoría independiente de todas las funcionalidades.
