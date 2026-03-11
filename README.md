# 💰 Simulador de Préstamos · Loan Simulator

<div align="center">

![Banner](https://img.shields.io/badge/Sistema_Francés-Amortización-4A90D9?style=for-the-badge&logo=chart-bar&logoColor=white)
![Estado](https://img.shields.io/badge/Estado-Activo-2ECC71?style=for-the-badge)
![Curso](https://img.shields.io/badge/Curso-2025--2026-F39C12?style=for-the-badge)
![Licencia](https://img.shields.io/badge/Licencia-MIT-9B59B6?style=for-the-badge)

---

> **Herramienta interactiva para la simulación y análisis de préstamos bajo el sistema de amortización francés**  
> Desarrollada para la asignatura *Análisis y Valoración de Proyectos de Inversión* · Trabajo 1

---

</div>

## 📋 Tabla de Contenidos

- [¿Qué es este proyecto?](#-qué-es-este-proyecto)
- [¿Para qué sirve?](#-para-qué-sirve)
- [Requisitos de la práctica](#-requisitos-de-la-práctica)
- [Parámetros de entrada](#-parámetros-de-entrada)
- [Resultados generados](#-resultados-generados)
- [Sistema de amortización francés](#-sistema-de-amortización-francés)
- [Cómo usar el simulador](#-cómo-usar-el-simulador)
- [Tecnologías utilizadas](#-tecnologías-utilizadas)
- [Estructura del proyecto](#-estructura-del-proyecto)
- [Autor](#-autor)

---

## 🏦 ¿Qué es este proyecto?

Este proyecto es un **simulador de préstamos** desarrollado como herramienta práctica para la comprensión y análisis de una de las fuentes de financiación más utilizadas tanto por empresas como por particulares.

El simulador implementa el **Sistema de Amortización Francés** (cuota constante), permitiendo calcular de forma precisa el término amortizativo resultante y el coste efectivo real de la operación bajo distintas hipótesis y condiciones.

---

## 🎯 ¿Para qué sirve?

En el mundo financiero actual, la capacidad de **comparar y elegir la fuente de financiación más adecuada** es una habilidad crítica. Este simulador permite:

| Funcionalidad | Descripción |
|---|---|
| 📊 **Analizar préstamos** | Visualizar el impacto de distintas condiciones en el coste total |
| 🔄 **Comparar escenarios** | Contraste entre tipo fijo y variable con distintos plazos |
| 💡 **Tomar decisiones informadas** | Conocer el coste efectivo real más allá de la cuota mensual |
| 📈 **Obtener el cuadro de amortización** | Desglose completo de capital e intereses período a período |
| 🧮 **Calcular bonificaciones** | Impacto de la contratación de productos vinculados |

---

## 📐 Requisitos de la Práctica

> Trabajo 1 — *Análisis y Valoración de Proyectos de Inversión* · Curso 2025-26

El simulador cumple con todos los requisitos exigidos por la asignatura:

- ✅ Herramienta **accesible online** (web), utilizable por compañeros y profesores
- ✅ Implementa el **Sistema de Amortización Francés** con términos constantes
- ✅ Permite distintas **periodicidades** (mensual, trimestral, semestral, anual)
- ✅ Incorpora el **Euríbor a 12 meses vigente** en los cálculos de tipo de interés
- ✅ Calcula el **Coste Efectivo (TAE)** de la operación
- ✅ Genera el **cuadro de amortización completo**
- ✅ Desarrollado **sin IA generativa** · Código 100% original
- ✅ **No es una hoja de cálculo** (requisito expreso de la práctica)

---

## 🔧 Parámetros de Entrada

### ⏱️ Duración y Periodicidad
```
Duración máxima : 30 años
Periodicidad    : Mensual · Trimestral · Semestral · Anual
```

### 💶 Nominal del Préstamo
```
Mínimo : 100.000 €
Máximo : 200.000 €
```

### 📉 Tipo de Interés

El simulador diferencia entre dos modalidades:

| Modalidad | Fórmula aplicada |
|---|---|
| 🔒 **Tipo Fijo** | Euríbor 12m (mes actual) **+ 1,00%** |
| 🔀 **Tipo Variable** | Euríbor 12m **+ 0,50%** |

### 🎁 Bonificaciones y Gastos

```
Bonificación por productos vinculados : entre 0,10% y 0,25% sobre el tipo de interés
Gastos de estudio                     : 150,00 €  (coste único inicial)
Gastos de administración              : 1‰ sobre cada término amortizativo
```

---

## 📊 Resultados Generados

El simulador produce los siguientes outputs de forma automática:

### 1. 📋 Cuadro de Amortización Completo

> *Sin comisiones ni gastos adicionales*

| Período | Término Amortizativo | Intereses | Amortización | Capital Pendiente |
|:---:|:---:|:---:|:---:|:---:|
| 1 | — | — | — | — |
| … | … | … | … | … |
| n | — | — | — | — |

### 2. 📌 Indicadores Financieros Clave

```
✦ Tipo de Interés Nominal Inicial (TIN)
✦ Coste Efectivo de la Operación (TAE)
✦ Total intereses pagados
✦ Coste total de la operación
```

---

## 📐 Sistema de Amortización Francés

El sistema francés, también conocido como de **cuota constante**, es el más utilizado en préstamos hipotecarios e inmobiliarios en España y Europa.

### Fórmula del Término Amortizativo

$$a = C_0 \cdot \frac{i}{1 - (1+i)^{-n}}$$

Donde:
- `a` → Término amortizativo (cuota constante)
- `C₀` → Capital inicial del préstamo
- `i` → Tipo de interés por período
- `n` → Número total de períodos

### Características principales

- 💡 La **cuota es constante** durante toda la vida del préstamo
- 📈 Al principio se pagan **más intereses y menos capital**
- 📉 Con el tiempo, la **amortización de capital aumenta** progresivamente
- 🏠 Es el sistema estándar en **hipotecas y préstamos bancarios** en España

---

## 🚀 Cómo Usar el Simulador

1. **Accede** al simulador a través del enlace disponible en el aula virtual
2. **Introduce** el nominal del préstamo (entre 100.000 € y 200.000 €)
3. **Selecciona** la duración y periodicidad deseadas
4. **Elige** entre tipo fijo o variable
5. **Ajusta** la bonificación por productos vinculados (0,10% – 0,25%)
6. Pulsa **"Calcular"** y obtén al instante:
   - El cuadro de amortización completo
   - El TIN inicial
   - El coste efectivo (TAE)

---

## 🛠️ Tecnologías Utilizadas

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

---

## 📁 Estructura del Proyecto

```
📦 simulador-prestamos/
├── 📄 index.html          # Interfaz principal del simulador
├── 🎨 styles.css          # Estilos y diseño visual
├── ⚙️  script.js           # Lógica de cálculo financiero
├── 📋 README.md           # Documentación del proyecto
└── 📊 simulacion.pdf      # Ejemplo de simulación con hipótesis detalladas
```

---

## 📅 Plazos

| Hito | Fecha |
|---|---|
| 🟡 Disponible en aula virtual | Antes del **15 de abril de 2025** |
| 📄 Entrega PDF con simulación | Antes del **15 de abril de 2025** |

---

## 👤 Autor

<div align="center">

Desarrollado para la asignatura **Análisis y Valoración de Proyectos de Inversión**  
Universidad · Curso académico **2025-2026**

---

*"La comprensión del coste real de la financiación es el primer paso hacia una gestión financiera responsable."*

</div>
