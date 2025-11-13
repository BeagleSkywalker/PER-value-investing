[b]Descripción General del Indicador[/b]
El indicador "PE Ratio Capa Investing" es una herramienta esencial para el análisis fundamental, que proporciona una visión clara del Ratio Precio/Beneficio (PER) histórico de un activo financiero dentro de una ventana de tiempo configurable.

El PER es una métrica de valoración fundamental que compara el precio de mercado de una acción con sus ganancias por acción (EPS). Este indicador va más allá del simple cálculo del PER actual, mostrando dinámicamente el PER Mínimo, PER Promedio y PER Máximo observados durante el período seleccionado, lo que permite a los inversores contextualizar la valoración actual del activo.

[b]Características Clave y Componentes[/b]
[i]1. Cálculo del PER (Price-Earnings Ratio)[/i]
Fuentes de Datos: Utiliza la función request.financial de TradingView para obtener las Ganancias por Acción (EPS) bajo el método "Trailing Twelve Months" (TTM), asegurando que el cálculo del PER se base en datos financieros recientes y estandarizados.

Fórmula: Calcula el PER dividiendo el Precio de Cierre (close) de la acción entre el EPS (TTM).

[i]2. Análisis Histórico de la Ventana de Tiempo[/i]
Ventana Configurable: Incluye una entrada de usuario (input.int) llamada "Cantidad de Semanas" con un valor predeterminado de 260 semanas (aproximadamente 5 años). Este ajuste es crucial para adaptarlo al gráfico semanal, aunque puede modificarse para periodos más cortos o largos (ej. 156 semanas para 3 años).

[i]Líneas de Referencia Clave:[/i] Calcula y traza tres líneas horizontales dinámicas basadas en el PER dentro de la ventana seleccionada:

🟢 PER Mínimo : La valoración más baja (más "barata") observada, trazada en verde.
🔴 PER Máximo: La valoración más alta (más "cara") observada, trazada en rojo.
⚪ PER Promedio : El promedio simple de todos los valores de PER dentro de la ventana, trazado en blanco (línea discontinua).

[i]3. Visualización y Usabilidad[/i]
PER Actual: El valor del PER en cada barra se traza con una línea amarilla, pero se restringe su visibilidad para mostrarse únicamente dentro de la ventana de tiempo definida, manteniendo el gráfico limpio y enfocado.

[i]Línea de Inicio de Ventana[/i]: Se utiliza una Línea Vertical Blanca para marcar con precisión el punto exacto en el tiempo donde comienza el cálculo de la ventana histórica (ej. el inicio de las 260 semanas).

[i]Etiquetas de Valores[/i]: En la barra más reciente (barstate.islast), se añaden etiquetas (label.new) a la derecha del gráfico para mostrar los valores numéricos exactos del PER Mínimo, Promedio y Máximo con dos decimales de precisión.

[b]Cómo Utilizar el Indicador[/b]
Este indicador es ideal para el análisis de regresión a la media y la identificación de zonas de valoración extrema.

Configuración del Gráfico: Para el uso predeterminado de 260 semanas, se recomienda utilizar el gráfico semanal (W). Si se ajusta la entrada de semanas a un período más corto (ej. 52 semanas), puede ser útil cambiar a un marco de tiempo diario (D) para una vista más detallada, aunque la métrica TTM se actualiza con la frecuencia de los reportes financieros.

[b]Identificación de Oportunidades:[/b]
- Cuando el PER Actual se acerca o cruza la Línea de PER Mínimo (Verde), podría indicar que el activo está históricamente subvalorado, sugiriendo una posible oportunidad de compra.

- Cuando el PER Actual se acerca o cruza la Línea de PER Máximo (Rojo), podría indicar que el activo está históricamente sobrevalorado, sugiriendo una posible oportunidad de venta o de toma de ganancias.

- Contextualización: El PER Promedio (Blanco) sirve como punto de referencia central para evaluar si la valoración actual es superior o inferior a su norma histórica reciente.

[b]Parámetros de Configuración[/b]
Cantidad de Semanas por defecto: 260

Realizado por Claudio Hernán Caparroz 
Youtube : Capa Investing 
[url=https://www.youtube.com/@CapaInvesting]https://www.youtube.com/@CapaInvesting[/url]
