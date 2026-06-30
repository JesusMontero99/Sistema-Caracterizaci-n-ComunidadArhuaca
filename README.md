# 📊 Sistema de Censo Poblacional — Comunidad Arhuaca
> Herramienta de caracterización y análisis de información comunitaria con enfoque de género, juventud y fortalecimiento territorial, en el marco de procesos de gestión de información con comunidades indígenas Arhuacas del Caribe colombiano.

## 🌿 Contexto
La comunidad Arhuaca, ubicada en el departamentos del Magdalena, requiere mecanismos propios de sistematización de información que respeten su identidad cultural y respondan a sus necesidades de planificación territorial, gestión ante entidades gubernamentales y fortalecimiento comunitario.

Este sistema fue desarrollado para centralizar, organizar y analizar datos cuantitativos generados en actividades comunitarias, garantizando la trazabilidad de la información y facilitando la toma de decisiones por parte del cabildo, equipos pedagógicos y actores institucionales.

---

## 🎯 Objetivo
Diseñar e implementar un sistema de captura, estructuración y análisis de datos censales comunitarios que permita:

- Caracterizar sociodemográficamente a los integrantes de las familias registradas
- Analizar indicadores clave con enfoque de **género**, **juventud** y **territorialidad**
- Generar reportes y visualizaciones para informes técnicos y presentaciones ante financiadores
- Facilitar la gestión predial y el uso del territorio ancestral
---

## ⚙️ Funcionalidades Principales

### 📋 Formulario de Registro (Excel VBA)
- Captura estructurada de datos en 6 secciones: Información General, Familiar, Demográfica, Social, Educación y Ocupación, y Predial
- Validaciones en tiempo real (campos numéricos, fechas, duplicados)
- Herencia automática de datos del predio desde la cabeza de familia a todos los integrantes
- Búsqueda por N° de identificación, N° de familia + orden, o ID interno
- Operaciones CRUD completas: Guardar, Buscar, Editar, Eliminar, Limpiar
- Listas desplegables dinámicas cargadas desde hoja de configuración
- Gestión de selección múltiple (usos del predio, espacios culturales)

### 🗄️ Base de Datos Estructurada
- Tabla estructurada con 40+ columnas organizada en TablaCenso
- Columnas calculadas: Grupo Edad (clasificación ICBF), Clave Familia (comunidad + N° familia)
- Compatibilidad con Power Query y Power Pivot para análisis avanzado

### 📊 Dashboard Analítico Interactivo
- **6 tarjetas KPI**: Total Personas, Total Familias, Total Predios, Total Comunidades, Promedio y Máximo de personas por familia
- **7 segmentadores** interactivos: Departamento, Municipio, Cuenca, Comunidad, Sexo, Grupo Edad, Seguridad Social
- **Indicadores demográficos**: distribución por sexo, tipo identificación, rangos de edad, lengua materna, personas por departamento/municipio
- **Indicadores sociales**: seguridad social en salud, asistencia escolar, nivel educativo, ocupación principal y secundaria
- **Indicadores territoriales**: años promedio en territorio por comunidad, distribución de áreas por predio, tipo de vivienda, adquisición del predio
- **Usos del predio**: análisis de uso agrícola, cría de animales, conservación, vivienda y espacios culturales
- Actualización automática al registrar, editar o eliminar datos

---

## 📈 Indicadores con Enfoque Diferencial

| Indicador | Enfoque |
|-----------|---------|
| Distribución por sexo | Género |
| Rangos de edad  | Juventud / Ciclo vital |
| Asistencia escolar por edad | Juventud |
| Nivel educativo | Género / Juventud |
| Lengua materna | Identidad cultural |
| Años en territorio | Territorialidad |
| Ocupación principal/secundaria | Género / Economía propia |
| Distribución de áreas por comunidad | Territorialidad |

---

## 🛠️ Tecnologías Utilizadas

| Herramienta | Uso |
|-------------|-----|
| **Excel VBA** | Formulario de captura, validaciones, lógica de negocio |
| **Power Query** | Transformación de datos de selección múltiple |
| **Power Pivot / DAX** | Medidas calculadas para KPIs del dashboard |
| **Tablas Dinámicas** | Agregaciones y análisis por categoría |
| **Segmentadores** | Filtrado interactivo del dashboard |

---

## 🗂️ Estructura del Proyecto

```
📁 Sistema-CensoPoblacional-ComunidadArhuaca
│
├── 📊 Censo_Demo.xlsx          # Archivo Excel con datos ficticios de demostración
├── 📁 VBA/                     # Módulos de código VBA exportados
│   ├── ModuloBtnGuardar.bas
│   ├── ModuloBtnBuscar.bas
│   ├── ModuloBtnEditar.bas
│   ├── ModuloBtnEliminar.bas
│   ├── ModuloBtnLimpiar.bas
│   ├── ModuloValidaciones.bas
│   ├── ModuloActualizar.bas
│   └── ModuloLlenarComboBox.bas
├── 📁 screenshots/             # Capturas del sistema
│   ├── formulario_registro.png
│   ├── dashboard_general.png
│   └── dashboard_predial.png
└── 📄 README.md
```

---

## 📸 Capturas del Sistema

### Formulario de Registro
> *Captura del formulario VBA con las 6 pestañas de información*
> <img width="743" height="678" alt="image" src="https://github.com/user-attachments/assets/39667f7d-b8f0-44b1-b309-f0ad53ad866c" />
> <img width="743" height="680" alt="image" src="https://github.com/user-attachments/assets/427c91e2-d5c4-4014-a346-402ea2de136f" />
> <img width="741" height="674" alt="image" src="https://github.com/user-attachments/assets/eb51b0d6-8602-44e8-b2d7-6668590a8404" />
> <img width="739" height="673" alt="image" src="https://github.com/user-attachments/assets/90507c2f-c96d-44b3-b927-1597bb21e7b2" />
> <img width="744" height="678" alt="image" src="https://github.com/user-attachments/assets/551cfe19-cb89-4540-b514-375b3a62a30e" />
> <img width="741" height="678" alt="image" src="https://github.com/user-attachments/assets/05955b71-db39-4b3f-93cf-ccad17f81b49" />

### Dashboard Analítico
> *Captura del dashboard con segmentadores activos y gráficas*
<img width="1342" height="437" alt="image" src="https://github.com/user-attachments/assets/993a0f36-5526-460b-a1f9-02583a4a1580" />
<img width="1333" height="461" alt="image" src="https://github.com/user-attachments/assets/89a5f37d-2efb-4d28-bac9-3630c4b7041c" />
<img width="1338" height="292" alt="image" src="https://github.com/user-attachments/assets/0dca54e9-3601-4086-8148-4a7885b949a8" />


--

## 🚀 Cómo usar el archivo demo

1. Descargar `Censo_Demo.xlsx`
2. Habilitar macros al abrir el archivo
3. Usar el botón **"Abrir Formulario"** para acceder al sistema de registro
4. Navegar al **Dashboard** para explorar los indicadores interactivos
5. Probar los segmentadores para filtrar por comunidad, departamento, sexo o grupo de edad

---

## 📌 Nota sobre los datos

Este repositorio contiene **únicamente datos ficticios** creados con fines de demostración. Los datos reales de las comunidades son confidenciales y no forman parte de este repositorio, en cumplimiento de los principios de soberanía de datos de los pueblos indígenas.

---

