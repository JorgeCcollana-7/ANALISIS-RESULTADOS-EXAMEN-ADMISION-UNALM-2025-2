# 🎓 UNALM Admission Results - Web Scraping & Dashboard

## 📋 Descripción del Proyecto

Este proyecto automatiza la extracción de datos de resultados de admisión de la Universidad Nacional Agraria La Molina (UNALM) 2025-II y los transforma en un dashboard interactivo para análisis de datos.

## 🎯 Objetivo

Convertir el proceso manual de consulta de resultados de admisión carrera por carrera en una solución automatizada que genere insights visuales sobre el proceso de admisión universitaria.

## 🔧 Tecnologías Utilizadas

- **Python 3.12**
- **Selenium WebDriver** - Automatización web
- **Pandas** - Procesamiento de datos
- **Power BI** - Visualización de datos
- **CSV** - Formato de intercambio de datos

## 📊 Proceso de Extracción

### Sitio Web Fuente
El scraping se realizó sobre el portal oficial de resultados: `https://resultados.lamolina.edu.pe/resultados`

**Características del sitio:**
- Navegación por carreras individuales
- Información estructurada por modalidad de ingreso
- Datos de ingresantes con OMG (Orden de Mérito General)
- 12 carreras disponibles para consulta

### Flujo de Navegación Automatizada

1. **Página inicial**: Acceso al portal de resultados
2. **Selección de modalidad**: Click en "Buscar por carreras"
3. **Navegación por carreras**: Automatización de selección de cada carrera
4. **Extracción de datos**: Captura de información estructurada
5. **Cambio de carrera**: Uso del botón "Elegir otra carrera"

## 📈 Datos Extraídos

### Estructura de Datos
```
- INGRESANTE: Nombre completo del estudiante
- MODALIDAD: Tipo de ingreso (Concurso Ordinario, Traslados Externos, etc.)
- OMG: Orden de Mérito General
- CARRERA: Programa académico
```


## 🚀 Instalación y Uso

### Prerrequisitos
```bash
pip install selenium pandas
```

### Configuración
1. Descargar ChromeDriver
2. Configurar PATH del navegador
3. Instalar dependencias de Python

### Ejecución
```bash
python webscraping_unalm.py
```

### Salida
- `todos_ingresantes.csv` - Dataset crudo
- `ingresantes_UNALM_2025_II.csv` - Dataset procesado para Power BI

## 📊 Insights Clave

- **Carrera más demandada**: Agronomía con 22.6% de los ingresos
- **Principal vía de ingreso**: Concurso Ordinario (71.3%)
- **Tasa de éxito general**: 23.2% de postulantes logran ingresar
- **Distribución equilibrada** entre modalidades especiales

## 🔄 Automatización Implementada

**Beneficios logrados:**
- ✅ Reducción de tiempo: De horas a minutos
- ✅ Eliminación de errores manuales
- ✅ Datos estructurados y listos para análisis
- ✅ Proceso escalable y reutilizable
- ✅ Dashboard actualizable automáticamente

## 📁 Estructura del Proyecto

```
├── WEBSCRAPING_RESULTADOS_UNALM.ipynb
├── todos_ingresantes.csv
├── ingresantes_UNALM_2025_II.csv
├── dashboard_unalm.pbix
└── README.md
```

## 🎯 Casos de Uso

- **Análisis institucional**: Tendencias de admisión por programa
- **Planificación académica**: Capacidad por carrera
- **Estudios comparativos**: Modalidades de ingreso
- **Reportes ejecutivos**: KPIs automatizados

---

**Desarrollado por**: Jorge Ccollana Orosco  
**Fecha**: Proceso de Admisión 2025-II  
**Examen**: 13 de julio de 2025
