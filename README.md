# Taller Práctico 03 — Ecosistema Odoo  
Autor: Daniel Ortiz Jiménez  
Centro: Campus Cámara de Comercio – Sevilla  

---

## Resumen del proyecto
Este taller implementa un entorno funcional de Odoo mediante contenedores Docker y desarrolla un flujo completo de trabajo: instalación de módulos, carga de datos, personalización de informes y exportación de información.

---

## Fase 1 — Integración de módulos
En esta fase se instalan los módulos de **Inventario** y **Facturación**, observando cómo Odoo modifica el esquema de PostgreSQL en tiempo real.  
También se importan los clientes iniciales mediante la herramienta de importación, generando automáticamente los registros en la tabla `res_partner`.

---

## Fase 2 — Personalización de informes
Se activa el modo desarrollador y se localiza la plantilla base del informe de ventas.  
Mediante una **vista heredada** se añade un bloque XML con el texto legal y el CIF, que aparecerá en los PDFs generados desde los presupuestos.

---

## Fase 3 — Exportación de información
Se seleccionan los clientes desde la vista de lista y se exportan en formato **CSV compatible con importación**, incluyendo campos simples y relaciones Many2one.  
El archivo resultante puede reutilizarse en herramientas externas o para actualizaciones masivas.

---

## Archivos añadidos al repositorio


capturasTaller03/ - Carpeta con capturas del proceso completo.
Contacto (res.partner).csv - CSV exportado tras finalizar la Fase 3.
DanielOrtizJimenezTallerPractico03.pdf - Guía completa del taller y pasos realizados.
clientes_mock.csv - CSV con los clientes iniciales para la importación.
docker-compose.yml - Archivo para desplegar Odoo con Docker.
---

## Notas finales
Este repositorio documenta el ciclo completo de trabajo en Odoo: instalación, carga de datos, personalización y exportación.  
Permite reproducir el entorno y comprender cómo interactúan los módulos internos del ERP.

