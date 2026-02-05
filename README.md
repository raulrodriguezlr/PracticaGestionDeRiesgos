# 🎯 Motor de Stress Testing: Escenarios de Estrés y Cambios de Régimen

**Práctica B2-2 - Módulo de Gestión de Riesgos**  
**MIAX - Febrero 2026**

---

## 📋 Descripción

Motor de stress testing en Python que:
1. Detecta regímenes de mercado (calma/crisis) usando **Hidden Markov Models**
2. Captura dependencias extremas entre activos usando **Cópulas**
3. Simula escenarios realistas con **Monte Carlo** (10,000 trayectorias)
4. Cuantifica riesgo extremo: **VaR 99%** y **Expected Shortfall (CVaR)**

## 📁 Estructura del Proyecto

```
PracticaGestionDeRiesgos/
├── notebooks/
│   ├── main.ipynb        # Notebook principal (entregable)
│   └── dev.ipynb         # Notebook de desarrollo/pruebas
├── utils/
│   ├── notebook_writer.py    # Utilidad para modificar notebooks
│   ├── pdf_generator.py      # Convertir Markdown a PDF
│   └── __init__.py
├── scripts/
│   └── create_notebooks.py   # Script para crear notebooks
├── data/
│   ├── raw/              # Datos crudos descargados
│   └── processed/        # Datos procesados
├── docs/
│   └── informe_ejecutivo.md  # Plantilla del informe
├── output/
│   └── figures/          # Gráficos exportados
├── requirements.txt
└── README.md
```

## 🚀 Instalación

```bash
# Clonar/descargar el repositorio
cd PracticaGestionDeRiesgos

# Crear entorno virtual (opcional pero recomendado)
python -m venv venv
venv\Scripts\activate  # Windows

# Instalar dependencias
pip install -r requirements.txt
```

## 📊 Cartera Analizada

18 activos equiponderados (sin rebalanceo):
- **Tech:** AAPL, AMZN, GOOGL, MSFT, NVDA
- **Financieras:** BAC, JPM, BRK-B
- **Energía:** CVX, XOM, ENPH
- **Defensivas:** JNJ, PG
- **Especulativo:** GME
- **Oro:** GLD
- **Renta Fija:** IEF (Treasury 10Y), SHY (Treasury 2Y), HYG (High Yield)

## 📈 Fases del Proyecto

| Fase | Descripción | Estado |
|------|-------------|--------|
| 0 | Setup del proyecto | ✅ Completado |
| 1 | HMM - Detección de regímenes | 🔄 En progreso |
| 2 | Análisis marginal por estado | ⏳ Pendiente |
| 3 | Cópulas - Estructura de dependencia | ⏳ Pendiente |
| 4 | Motor de simulación Monte Carlo | ⏳ Pendiente |
| 5 | Escenarios de estrés | ⏳ Pendiente |

## 📚 Entregables

1. **Notebook Técnico** (`notebooks/main.ipynb`)
   - Código comentado
   - Gráficos interpretativos
   - Resultados numéricos

2. **Informe Ejecutivo** (máx. 3 páginas PDF)
   - Lenguaje de negocio
   - Para: CEO, CFO, CRO

## 🔧 Uso

```bash
# Ejecutar Jupyter
jupyter notebook notebooks/main.ipynb

# Generar PDF del informe (cuando esté listo)
python -c "from utils.pdf_generator import md_to_pdf; md_to_pdf('docs/informe_ejecutivo.md', 'output/informe_ejecutivo.pdf')"
```

---

**Autor:** Raúl Rodríguez  
**Fecha de entrega:** 15 de Febrero 2026
