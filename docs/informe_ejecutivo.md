# Informe Ejecutivo: Escenarios de Estrés y Cambios de Régimen

**Para:** Comité de Riesgos (CEO, CFO, CRO)  
**De:** Departamento de Riesgos  
**Fecha:** [FECHA]  
**Clasificación:** Confidencial

---

## Resumen Ejecutivo

[Breve resumen de 2-3 líneas sobre los hallazgos principales y recomendaciones clave]

---

## 1. Contexto y Metodología

### Problema
Los modelos de riesgo tradicionales fallaron en 2022 al no capturar la caída simultánea de acciones y bonos.

### Enfoque
Hemos desarrollado un motor de stress testing basado en:
- **Detección de regímenes** mediante Hidden Markov Models
- **Modelado de dependencias** con cópulas
- **Simulación Monte Carlo** para escenarios extremos

---

## 2. Hallazgos Principales

### Estados del Mercado Identificados

| Métrica | Estado Calma | Estado Crisis |
|---------|-------------|---------------|
| Volatilidad (anualizada) | X% | Y% |
| Correlación promedio | X | Y |
| % del tiempo histórico | X% | Y% |

### Comportamiento en Crisis
- La diversificación **desaparece**: correlaciones pasan de X a Y
- Volatilidad **aumenta** en promedio un X%
- El oro (GLD) [funciona/no funciona] como refugio

---

## 3. Resultados de Escenarios de Estrés

### Métricas de Riesgo por Escenario (Horizonte: 6 meses)

| Escenario | VaR 99% | CVaR 99% | Max Drawdown |
|-----------|---------|----------|--------------|
| Base | X% | Y% | Z% |
| Estanflación 2022 | X% | Y% | Z% |
| Crisis Crediticia 2008 | X% | Y% | Z% |
| [Escenario Alternativo] | X% | Y% | Z% |

---

## 4. Recomendaciones

1. **Revisión de límites de riesgo**: Considerar VaR/CVaR condicional a regímenes
2. **Cobertura dinámica**: Implementar detección de cambio de régimen en tiempo real
3. **Diversificación real**: Reducir exposición a activos con alta correlación en crisis

---

*Nota: Este análisis utiliza datos históricos desde 2006. Los escenarios de estrés son hipotéticos pero económicamente coherentes.*
