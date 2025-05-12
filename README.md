# Historial de Compras en Monedas (USD/MXN) - Módulo Odoo 17

### Desarrollado por: Ing. Christian Padilla Muñiz  
**Compañía:** SAFI

---

## 📦 Descripción

Este módulo está diseñado para **gestionar el historial de compras de productos** en Odoo 17, diferenciando entre compras realizadas en **USD** y **MXN**, y generando un resumen consolidado con conversión de moneda.

El sistema está optimizado para compañías que operan con proveedores en múltiples monedas y requieren **visibilidad clara y conversiones automáticas** para análisis y comparación de precios.

---

## ⚙️ Funcionalidades

- **Registro separado de compras en USD y MXN**, con sus respectivos precios unitarios.
- Permite **marcar** fácilmente si una compra se realizó en **USD** o **MXN**.
- Genera una **tercera vista consolidada**, combinando ambos historiales y filtrando por la compra más reciente de cada producto.
- Muestra **precios convertidos automáticamente a MXN** usando la tasa definida por el usuario (`res.users.valor_dollar`).
- Incluye un **botón de conversión manual** que permite aplicar la conversión de USD a MXN en la vista consolidada.
- Posibilidad de **crear listas de precios** directamente desde el historial consolidado para uso interno de ventas.
- Permite Generar un reporte excel como lista de precios actualizada y convertida

---

## 🏗 Estructura técnica

El módulo incluye:

- Modelos SQL (`_auto = False`) para combinar datos históricos.
- Campos calculados (`compute`) para realizar la conversión sin almacenar datos.
- Botones de acción para ejecutar conversiones y generar listas de precios.
- Uso de la vista `purchase.product.history.combined` como resumen final con la conversión aplicada.

---

## 📥 Instalación

1. **Descargar o clonar** este módulo en tu carpeta de addons personalizada:
   ```bash
   /odoo/custom_addons/purchase_currency_history



👨‍💻 Autor
Ing. Christian Padilla Muñiz
Desarrollado para: SAFI

Este módulo fue construido con el objetivo de facilitar la gestión de precios y compras internacionales, mejorando la eficiencia en empresas que operan con múltiples monedas.
