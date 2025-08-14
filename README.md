# proyecto_13_machine_learning
Machine Learning | Pronósticos y predicciones | Sklearn  | Algoritmos | Regresión Logística | Árbol de decisión: Bosque aleatorio (random forest) y Gradiente boosting |  Clustering K-Means | Supervisado - No Supervisado | Clasificación | División Aleatoria y Temporal

# ESTRATEGIA DE RETENCIÓN DE CLIENTES PARA MODEL FITNESS

## RESUMEN DEL PROYECTO
Análisis del comportamiento de clientes en la cadena de gimnasios Model Fitness para:
1. Predecir probabilidad de cancelación (churn)
2. Identificar segmentos clave de clientes
3. Desarrollar estrategias de retención basadas en datos

## OBJETIVO
1. Reducir la tasa de cancelación mensual (actualmente 26.5%)
2. Mejorar la retención de clientes mediante intervenciones personalizadas
3. Optimizar estrategias de marketing y fidelización

## METODOLOGÍA DE ANÁLISIS

### 1. DESCRIPCIÓN DE LOS DATOS
- Dataset: 4,000 clientes con 14 características
- Variables clave:
  - Demográficas: edad, género
  - Comportamiento: frecuencia de visitas, gastos adicionales
  - Contrato: tipo, tiempo restante
  - Churn: cancelación en el mes siguiente (26.5% tasa base)

### 2. PREPROCESAMIENTO DE DATOS
- Limpieza: sin valores nulos
- Estandarización: escalado para modelos
- División: 80/20 train-test split
- Codificación: variables categóricas binarias

### 3. PRUEBA DE HIPÓTESIS
#### Modelos predictivos:
| Métrica         | Regresión Logística | Bosque Aleatorio |
|-----------------|---------------------|------------------|
| Exactitud       | 92.25%              | 91.50%           |
| Recall          | 82.83%              | 81.31%           |
| ROC AUC         | 97.06%              | 96.80%           |

#### Segmentación (5 clústeres):
| Clúster | Tasa Churn | Perfil |
|---------|------------|--------|
| 0       | 2.8%       | Leales largo plazo |
| 1       | 26.8%      | Activos corto plazo |
| 2       | 44.4%      | Bajo compromiso |
| 3       | 51.4%      | Alto riesgo |
| 4       | 6.8%       | Estables |

## CONCLUSIONES PRINCIPALES
1. **Factores clave de churn**:
   - Contratos cortos (1 mes) tienen 5x mayor riesgo
   - Clientes nuevos (<2 meses) son 3x más propensos a cancelar
   - Baja frecuencia de visitas actual predice cancelación

2. **Segmentos críticos**:
   - Clúster 3: 51% churn - Lejanía + contrato corto
   - Clúster 2: 44% churn - Bajo uso + sin beneficios adicionales

3. **Oportunidades**:
   - Programas de fidelización para contratos largos
   - Incentivos para aumentar frecuencia de visitas
   - Enfoque en clientes durante primeros 60 días

## RECOMENDACIONES ESTRATÉGICAS
1. **Paquetes de compromiso**:
   - Ofrecer descuentos en contratos de 6/12 meses
   - Bonificación por renovación anticipada

2. **Programa de onboarding**:
   - Sesiones introductorias para nuevos miembros
   - Retos de 30 días con seguimiento personalizado

3. **Intervenciones segmentadas**:
   - Clúster 3: Ofertas de transporte/estacionamiento
   - Clúster 2: Paquetes de clases grupales incluidos

4. **Sistema de alertas**:
   - Monitorear disminución en frecuencia de visitas
   - Activación automática de ofertas de retención

## TECNOLOGÍAS UTILIZADAS
- Python (Pandas, NumPy)
- Scikit-learn (Regresión Logística, Random Forest, K-Means)
- Matplotlib/Seaborn (Visualización)
- SciPy (Análisis estadístico)
- Jupyter Notebooks (Análisis interactivo)
