# MowZone Scalping 5m (EMA+MACD+ATR+SSL)

> **Para TradingView - Pine Script™**

## 🔥 Descripción
Estrategia de scalping diseñada para operar en temporalidad de 5 minutos, combinando 4 indicadores técnicos para filtrar operaciones de alta probabilidad. Su enfoque multidivergente (tendencia + momentum + volatilidad) busca capturar movimientos rápidos del precio con un ratio riesgo/recompensa favorable.

## 📊 Indicadores Utilizados
- **EMA 200:**
  - Filtro de tendencia principal.
  - Operaciones largas solo por **ENCIMA** de la EMA.
  - Operaciones cortas solo por **DEBAJO** de la EMA.
- **SSL Hybrid (12 periodos):**
  - Identifica cambios de tendencia con cruces de sus líneas.
  - Confirma dirección del mercado junto a la EMA 200.
- **MACD (12-26-9):**
  - Gatillo de entrada en zonas extremas:
    - **Largas:** Cruce alcista en zona de sobreventa (valores ≤ -50).
    - **Cortas:** Cruce bajista en zona de sobrecompra (valores ≥ 50).
- **ATR (14 periodos):**
  - Gestiona riesgo con **Stop Loss (1.5x ATR)** y **Take Profit (3x ATR)**.
  - Niveles dinámicos adaptados a la volatilidad del mercado.

## ⚡ Cómo Funciona
### 🔹 Filtro de Tendencia
- Precio y SSL deben estar ambos del mismo lado de la **EMA200**.

### 🔹 Señal de Entrada
- Cruce de líneas **SSL + MACD en zona extrema**.

### 🔹 Gestión de Riesgo
- **SL y TP automáticos** basados en **ATR**.
- **Máximo 1 operación abierta simultáneamente**.

## 📈 Rendimiento (Backtest)
- **Temporalidad Óptima:** 5 minutos.
- **Operaciones/Día:** 1-2 señales claras.
- **Tasa de Acierto:** ~50% (equilibrado riesgo/recompensa **3:1**).
- **Estadísticas en Tiempo Real:** Tabla con resultados acumulados (ganancias/pérdidas).

## 🛠 Instalación
1. Copiar código en editor de **Pine Script™** (TradingView).
2. Ajustar parámetros según instrumento (ver sección de inputs).
3. Activar alertas para señales de entrada/salida.

## ⚠️ Advertencia
- ❌ **NO** es un sistema infalible (requiere gestión activa).
- 📊 Probada principalmente en índices y forex (**EUR/USD, NAS100**).
- 🛑 **Operar siempre con stop loss**.
- ⚠️ **¡Usar bajo su propio riesgo!**

## 📌 Características Visuales
- 📍 Señales de compra/venta con iconos.
- 📊 Líneas de **SL/TP en gráfico**.
- 🔆 **EMA200 resaltada en amarillo**.
- 🟥🟩 Zonas **SSL coloreadas** (rojo/verde).

## 🔧 Parámetros Personalizables
- **ATR:** Multiplicadores de **SL/TP**.
- **Tipos de MA para SSL** (*SMA, EMA, HMA, TEMA, etc*).
- **Umbrales MACD**.
- **Mostrar/ocultar elementos visuales**.

---

📜 **Código sujeto a licencia MPL 2.0**

🛠 **Última actualización:** 12/02/2025

🚀 **Desarrollado por [@mowgl1ph](https://tradingview.com/u/jelvys_triana) - [GitHub](https://github.com/mowgl1ph)**

🌟 **¡Importante!**
> Esta estrategia funciona mejor en mercados con tendencia. En laterales, reducir tamaño de posición o evitar operar.
> Siempre combine con **análisis de precio y gestión de capital**. 🚀📈
