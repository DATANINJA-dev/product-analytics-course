# Contexto del Curso: Clases Particulares Data Analytics

## Información del Profesor
- **Profesor**: DATANINJA-dev (Alfons)
- **Experiencia**: Profesor de Data Analytics en Ironhack
- **Repositorio principal**: `C:\Users\alfons.marques\OneDrive - Schwarz IT\Documentos\github_repo_dataninja\Ironhack-data-sept-2023`

## Alumno
- **Nombre**: Diogo Barros
- **Background**: Tech Trainer & CEO | Cloud Computing | DevOps | Web | Data Science
- **Objetivo**: 8 clases particulares de 1.5 horas cada una (12 horas totales)
- **Primera clase**: 5 de septiembre, 3:00-4:30 PM CET
- **Frecuencia**: Viernes semanalmente
- **Tarifa**: €120 por sesión (1h30)
- **Idioma**: **INGLÉS** (confirmado en conversación)
- **Nivel**: Previo conocimiento de Data Science (fue alumno anterior)
- **Objetivos específicos**: 
  - **Product Data Analytics** (foco principal)
  - **Data Science** aplicado
  - **Casos reales de trabajo**
  - **"When to use X model"** - aplicaciones prácticas
- **Contexto**: Quiere aplicar conceptos a escenarios reales de su trabajo

## Análisis del Curso Base (Ironhack)

### Estructura del Curso Original
- **Duración**: 20 semanas part-time
- **Formato**: Lunes/Miércoles/Sábados
- **Metodología**: Teoría + Labs + Business Cases
- **Recursos**: 50+ datasets, notebooks detallados, casos reales

### Progresión Temática Identificada

#### **Semanas 1-3: Python Fundamentals**
- Tipos de datos, control de flujo
- Funciones, OOP, manejo de errores
- NumPy, Pandas básico
- **Material clave**: `Week 01/01 - Monday/01. Intro Python - Data types.ipynb`

#### **Semanas 4-10: Data Analysis & Manipulation**
- Visualización (matplotlib, seaborn, plotly)
- SQL comprehensivo (8-9 semanas)
- Power BI, regex
- Business cases (BLING, Vueling)
- **Material clave**: `Week 08/01 - Monday/first_database_session.md`

#### **Semanas 11-15: Statistics & Advanced Analytics**
- Estadística computacional
- Análisis exploratorio avanzado
- Calidad de datos
- **Material clave**: `Week 15/01 - computational_statistics/`

#### **Semanas 17-20: Machine Learning**
- Unsupervised Learning
- Supervised Learning (clasificación/regresión)
- Deep Learning básico
- Proyectos end-to-end
- **Material clave**: `week 19/Machine Learning I.ipynb`

### Metodología Pedagógica Observada
1. **Notebooks teóricos** con explicaciones detalladas
2. **Labs prácticos** con ejercicios estructurados
3. **Business cases** aplicando conceptos
4. **Progresión gradual** de básico a avanzado
5. **Énfasis en herramientas reales** (pandas, scikit-learn, SQL)

## Propuesta para Curso Condensado (8 sesiones)

### **Sesión 1: Python + Data Structures**
- Fundamentos Python para análisis de datos
- Estructuras de datos esenciales
- **Material base**: Week 1-2 condensado

### **Sesión 2: NumPy + Pandas**
- Manipulación de datos
- DataFrame operations
- **Material base**: Week 3

### **Sesión 3: EDA + Visualización**
- Análisis exploratorio
- matplotlib/seaborn
- **Material base**: Week 5

### **Sesión 4: SQL Analítico**
- Queries esenciales
- Joins y agregaciones
- **Material base**: Week 8-9 condensado

### **Sesión 5: Estadística + Data Quality**
- Estadística descriptiva
- Calidad y limpieza de datos
- **Material base**: Week 15

### **Sesión 6: ML Fundamentos**
- Supervised learning básico
- Scikit-learn
- **Material base**: Week 19

### **Sesión 7: ML Avanzado + Unsupervised**
- Clustering, dimensionalidad
- Evaluación de modelos
- **Material base**: Week 17

### **Sesión 8: Proyecto End-to-End**
- Caso de negocio completo
- Presentación de resultados
- **Material base**: Business cases adaptados

## Material Reutilizable Identificado

### **Datasets Disponibles**
- 50+ datasets curados en `00 - datasets/`
- Casos de negocio reales (BLING, Vueling, etc.)
- Variedad de dominios (e-commerce, finanzas, etc.)

### **Notebooks Clave para Adaptar**
- Python fundamentals (Week 1-2)
- Pandas essentials (Week 3)
- Visualización (Week 5)
- SQL training (Week 8-9)
- Statistics (Week 15)
- ML notebooks (Week 17, 19, 20)

### **Business Cases Adaptables**
- BLING cohort analysis (Week 4)
- Vueling analytics challenge (Week 10)
- Proyectos end-to-end (Week 20)

## Investigación Product Analytics (2024)

### **Frameworks Consolidados Identificados**

#### **1. AARRR Framework (Pirate Metrics)**
- **Acquisition**: Cómo conseguir usuarios
- **Activation**: Primera interacción clave (signup, first task)
- **Retention**: Usuarios que vuelven repetidamente  
- **Referral**: Usuarios compartiendo el producto
- **Revenue**: Generación e escalabilidad de ingresos
- **Herramientas**: PostHog, Amplitude, Mixpanel

#### **2. HEART Framework (Google)**
- **Happiness**: Satisfacción/attitudes (NPS, surveys)
- **Engagement**: Nivel de uso (time in-app, sessions, shares)
- **Adoption**: % usuarios que adoptan producto/features
- **Retention**: Tasa usuarios que retornan (churn analysis)
- **Task Success**: Capacidad completar tareas (error rates, completion %)
- **Proceso**: Goals → Signals → Metrics

#### **3. North Star Metrics**
- Métrica única que raliza todo el equipo
- Enfoque en valor repetible ligado al objetivo principal
- Ejemplo: "workouts completed", "messages sent"

### **Metodologías Analíticas Clave**

#### **Cohort Analysis**
- **Time-based**: Usuarios agrupados por período (signups en enero)
- **Behavior-based**: Agrupados por acciones (completed tutorial, made referral)
- **Uso**: Retention analysis, conversion optimization
- **Herramientas**: Python/Hex, Mixpanel segmentation

#### **Funnel Analysis**
- **Stages**: Acquisition → Activation → Retention
- **Implementación**: User journey mapping, drop-off identification
- **Optimización**: A/B testing en cada stage

#### **A/B Testing + Feature Flags**
- **Feature Flags**: Control binario (on/off) con governance
- **Experiments**: Comprensión profunda del comportamiento
- **KPIs**: Growth/revenue related vs velocity/performance
- **Herramientas**: Statsig, PostHog, Optimizely

### **KPIs y Métricas Críticas**
- **Development KPIs**: Eficiencia del proceso de desarrollo
- **Product Analytics**: Comportamiento usuario, performance features
- **Business Impact**: Revenue, growth, user satisfaction
- **Decision Framework**: Objetivos → KPIs → Impacto UX/Business

### **Integración Python + Product Analytics**
- **Notebooks como vehículo**: Teoría + implementación práctica
- **Casos reales**: Aplicación de frameworks a escenarios de trabajo
- **Herramientas Python**: pandas, matplotlib, seaborn para analysis
- **Conexión con plataformas**: APIs de Mixpanel, Amplitude, PostHog

## Propuesta Programa 8 Sesiones - Product Analytics

### **Session 1: Product Analytics Foundations**
- **Teoría**: AARRR vs HEART vs North Star - cuándo usar cada uno
- **Práctica**: Setup analytics tracking simulation (Python)
- **Case Study**: Defining North Star for a SaaS product

### **Session 2: User Acquisition & Activation Analysis**  
- **Teoría**: Acquisition channels, activation patterns
- **Práctica**: Funnel analysis implementation (pandas)
- **Case Study**: Optimizing onboarding flow

### **Session 3: Retention & Cohort Analysis**
- **Teoría**: Retention patterns, cohort methodologies  
- **Práctica**: Cohort analysis with Python (time-based & behavior-based)
- **Case Study**: Subscription product retention analysis

### **Session 4: Engagement & Feature Analytics**
- **Teoría**: Engagement metrics, feature adoption tracking
- **Práctica**: Feature usage analysis, engagement scoring
- **Case Study**: Feature flag impact analysis

### **Session 5: Revenue & Business Impact Analytics**
- **Teoría**: Revenue attribution, LTV analysis
- **Práctica**: Revenue cohorts, monetization funnels (Python)
- **Case Study**: Freemium to paid conversion optimization

### **Session 6: A/B Testing & Experimentation**
- **Teoría**: Experiment design, statistical significance
- **Práctica**: A/B test analysis framework (scipy, statsmodels)
- **Case Study**: Feature release experimentation

### **Session 7: Advanced Analytics & Predictive Models**
- **Teoría**: Churn prediction, user scoring models
- **Práctica**: ML for product analytics (scikit-learn)
- **Case Study**: Predictive user lifecycle modeling

### **Session 8: Product Analytics Strategy & Frameworks**
- **Teoría**: Building analytics culture, decision frameworks
- **Práctica**: End-to-end dashboard creation (plotly/dash)
- **Case Study**: Full product analytics implementation

## Material Desarrollo
- **Estructura**: `/notebooks` para cada sesión
- **Datasets**: Simulados + casos reales anonimizados
- **Código**: Reproducible, documented, English
- **Formato**: Jupyter notebooks con teoría + práctica integrada

## Próximos Pasos
1. ✅ Contexto del curso base completado
2. ✅ Investigación Product Analytics completada
3. ✅ Programa 8 sesiones diseñado
4. ⏳ Crear índice detallado para primera clase
5. ⏳ Desarrollar Notebook Session 1
6. ⏳ Setup GitHub repository estructura

## Notas de la Sesión
[Espacio para notas durante las conversaciones con Diogo]