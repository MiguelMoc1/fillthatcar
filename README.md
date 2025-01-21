# ✨ Llena Ese Carrito 🎨

## Introducción
Instacart es una plataforma de entregas de comestibles donde los clientes pueden realizar pedidos y recibirlos en casa, similar a Uber Eats o DoorDash. Este proyecto utiliza un conjunto de datos adaptado para facilitar el análisis, incluyendo modificaciones como valores ausentes y duplicados, pero conservando la distribución original.

## Objetivo
El objetivo de este proyecto es explorar los datos proporcionados, realizar preprocesamiento y análisis exploratorio para entender los patrones de compra de los usuarios y encontrar oportunidades para optimizar la experiencia del cliente.

---

## Diccionario de Datos

### Archivos y Columnas Principales
1. **`instacart_orders.csv`**
   - `order_id`: ID único de cada pedido.
   - `user_id`: ID único del cliente.
   - `order_number`: Número de pedido del cliente.
   - `order_dow`: Día de la semana (0: domingo).
   - `order_hour_of_day`: Hora del pedido.
   - `days_since_prior_order`: Días desde el pedido anterior.

2. **`products.csv`**
   - `product_id`: ID único del producto.
   - `product_name`: Nombre del producto.
   - `aisle_id`: ID del pasillo.
   - `department_id`: ID del departamento.

3. **`order_products.csv`**
   - `order_id`: ID del pedido.
   - `product_id`: ID del producto.
   - `add_to_cart_order`: Orden de agregado al carrito.
   - `reordered`: 0 si el producto es nuevo, 1 si es reordenado.

4. **`aisles.csv`**
   - `aisle_id`: ID del pasillo.
   - `aisle`: Nombre del pasillo.

5. **`departments.csv`**
   - `department_id`: ID del departamento.
   - `department`: Nombre del departamento.

---

## Etapas del Proyecto

### 1. Preprocesamiento de Datos
#### Acciones Clave
- **Verificación de Tipos de Datos:** Conversión y limpieza para asegurar coherencia.
- **Detección y Eliminación de Duplicados:** Reducción de redundancias.
- **Manejo de Valores Ausentes:** Relleno de valores nulos según el contexto de cada columna.

#### Resultados
- Los nombres de productos faltantes fueron reemplazados por `Unknown`.
- Los valores nulos en `days_since_prior_order` se dejaron como están, ya que corresponden al primer pedido del usuario.
- La columna `add_to_cart_order` se rellenó con un valor especial (999) para productos con datos ausentes.

### 2. Análisis Exploratorio
#### Principales Hallazgos
1. **Patrones de Tiempo:**
   - Las horas pico para pedidos son de 10:00 a.m. a 4:00 p.m.
   - Los domingos y lunes son los días con más actividad.

2. **Productos Más Populares:**
   - Plátanos y productos orgánicos como fresas y espinaca son los más vendidos.

3. **Comportamiento de Reorden:**
   - Aproximadamente el **59%** de los productos en un pedido ya fueron comprados anteriormente.

4. **Hábitos de Compra:**
   - La mayoría de los clientes realiza pedidos pequeños, de entre 0 y 10 productos.

---

## Tecnologías Utilizadas
- **Lenguajes:** Python
- **Librerías Principales:** `pandas`, `matplotlib`, `seaborn`
- **Visualización:** Gráficos de barras, histogramas y diagramas de dispersión

---

## Conclusiones Generales
Este proyecto proporciona una visión profunda de los patrones de compra en la plataforma Instacart, destacando:
- La importancia de los productos frescos y orgánicos en los pedidos.
- La fidelidad de los clientes al reordenar productos previamente comprados.
- Las oportunidades para personalizar recomendaciones basadas en patrones de compra.

Estas observaciones pueden guiar estrategias para optimizar la experiencia del cliente y aumentar la retención en la plataforma.

---

## Estructura del Repositorio
- **`notebooks/`**: Código fuente y análisis detallado.
- **`data/`**: Conjuntos de datos utilizados (no incluidos por restricciones de tamaño).
- **`visualizations/`**: Gráficos generados durante el análisis.

---

## Contacto
Para más información sobre este proyecto, contáctame en:
- **Email:** [tucorreo@dominio.com](mailto:tucorreo@dominio.com)
- **LinkedIn:** [Tu Perfil](https://linkedin.com)
- **Portafolio GitHub:** [Tu Usuario](https://github.com)
