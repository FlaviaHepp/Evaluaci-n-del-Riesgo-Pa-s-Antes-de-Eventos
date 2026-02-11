# 📈Evaluación del Riesgo País Antes de Eventos

Kurtosis pre-Ganancias como termómetro macro y regulatorio

## 📌Descripción General

Este proyecto analiza el riesgo estadístico de cola (kurtosis) de las acciones justo antes de un anuncio de Ganancias, comparando dicho riesgo entre países.

La hipótesis es que el riesgo percibido por el mercado antes de un evento clave no es homogéneo globalmente, y refleja:
- estabilidad macroeconómica,
- calidad regulatoria,
- transparencia informativa,
- madurez del mercado de capitales.

## 📍Insight Clave

- ¿Las acciones de ciertos países (por ejemplo USA) presentan menor riesgo de cola antes de anunciar Ganancias, comparadas con el promedio global?

Un kurtosis bajo previo al evento sugiere:
- menor probabilidad de shocks extremos,
- expectativas más ordenadas,
- mayor eficiencia informacional.

## 💼Valor de Negocio

- Permite comparar riesgo país desde el mercado, no desde ratings externos.

Útil para:
- asignación geográfica de capital,
- modelos de riesgo macro,
- estrategias event-driven internacionales.
- Identifica mercados donde los anuncios de Ganancias son:
- más predecibles,
- o más propensos a sorpresas extremas.

Fuentes de Datos: 
- eventos_corporativos
- ticker_id
- fecha
- tipo_evento
- tickers
- ticker_id
- bolsa_mercado
- indicadores_tecnicos
- ticker_id
- fecha
- kurtosis

## 🧠Lógica del Análisis

Se filtran eventos corporativos del tipo Ganancias.

Para cada ticker:
- Se toma el kurtosis del día anterior al anuncio.
- Se agrupan los datos por país / mercado.
- Se calcula:
  kurtosis promedio pre-evento,
  número de observaciones por país.

- Se descartan países con baja muestra estadística.

## 📊Interpretación de Resultados

Kurtosis pre-Ganancias baja
→ Menor riesgo de movimientos extremos.
→ Mercado estable y bien anticipado.

Kurtosis alta
→ Mayor riesgo de sorpresas violentas.
→ Posible opacidad informativa o fragilidad macro.

Alta dispersión entre países
→ Evidencia de primas de riesgo estructurales.

## 🧩Casos de Uso

- Comparación objetiva de riesgo país basada en datos de mercado.
- Ajuste de exposición internacional antes de earnings season.
- Input para modelos de volatilidad y estrés macro.
- Validación empírica de ratings soberanos.

## 🚀Posibles Extensiones

- Comparar kurtosis pre vs. post-Ganancias.
- Normalizar por sector para aislar efecto país.
- Analizar ventanas de 3 y 5 días pre-evento.
- Combinar con skewness para evaluar dirección del riesgo.
- Estudiar cambios a lo largo del tiempo (crisis vs. calma).

## Nota Final

Este insight responde una pregunta potente:
¿Dónde el mercado teme sorpresas… incluso antes de que ocurra el evento?

Porque a veces, el riesgo país no se lee en informes macro,
sino en la cola estadística de los retornos 📉📊

## 👤Autora
Flavia Hepp Proyecto de SQL aplicó un análisis de riesgo basado en eventos.
