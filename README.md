# 🌿 Dashboard NPS & Evaluación de Satisfacción — Speakers En Verde Calama 2026

[![Corfo Viraliza](https://img.shields.io/badge/Corfo-Viraliza%2025VIRTL--307467-0099FF?style=for-the-badge)](https://www.corfo.cl/)
[![NPS Score](https://img.shields.io/badge/NPS%20Score-%2B84.6%20pts%20(Excelencia)-10B981?style=for-the-badge)](#)
[![Satisfacción](https://img.shields.io/badge/Meta%202%20Satisfacci%C3%B3n-88.4%25-blue?style=for-the-badge)](#)
[![GitHub Pages](https://img.shields.io/badge/Deploy-GitHub%20Pages%20Ready-181717?style=for-the-badge&logo=github)](#despliegue-rápido-en-github-pages)

Repositorio oficial del **Dashboard Interactivo y Análisis Estadístico de Satisfacción** del programa **Speakers En Verde**, desarrollado en la comuna de **Calama** (Provincia de El Loa, Región de Antofagasta) bajo el instrumento **Viraliza Formación Código 25VIRTL-307467** del **Comité Corfo Antofagasta**.

---

## 📊 Métricas Clave y Cumplimiento de Metas

| Métrica / Indicador | Resultado Obtenido | Meta / Estándar Corfo | Evaluación |
| :--- | :---: | :---: | :---: |
| **NPS Score (Net Promoter Score)** | **+84.62 pts** | $\ge +50.0\text{ pts}$ | **Nivel de Excelencia Mundial (World Class)** |
| **Nota Promedio Recomendación (0-10)** | **9.35 / 10** | $\ge 8.00$ | **Sobresaliente** |
| **Meta 1 (Disposición a Recomendar)** | **88.46%** (23/26) | $\ge 70.0\%$ | **Superada con éxito** |
| **Meta 2 (Satisfacción Global Notas 4 ó 5)** | **88.42%** (275/311) | $\ge 75.0\%$ | **Superada con éxito** |
| **Muestra Total Analizada** | **26 participantes** | 5 Liceos de Calama | 22 Estudiantes, 4 Docentes Líderes |

---

## 🚀 Despliegue Rápido en GitHub Pages

Este proyecto está diseñado para funcionar como una aplicación web autónoma (Single Page Application) sin necesidad de entornos Node.js ni procesos de compilación (build steps).

### Paso 1: Inicializar el repositorio Git local
```bash
cd dashboard_github
git init
git add .
git commit -m "feat: Dashboard interactivo Speakers En Verde Calama 2026"
```

### Paso 2: Vincular con tu repositorio en GitHub y subir los cambios
```bash
git remote add origin https://github.com/TU-USUARIO/speakers-en-verde-calama-2026.git
git branch -M main
git push -u origin main
```

### Paso 3: Activar GitHub Pages en 1 clic
1. En GitHub, ingresa a tu repositorio y ve a **Settings** (Configuración) > **Pages** (en el menú lateral izquierdo).
2. En **Build and deployment** > **Branch**: selecciona `main` y la carpeta `/(root)`.
3. Haz clic en **Save** (Guardar).
4. En 30 segundos tu dashboard estará público en:  
   `https://TU-USUARIO.github.io/speakers-en-verde-calama-2026/`

---

## 📁 Estructura del Proyecto

```plaintext
dashboard_github/
├── index.html         # Aplicación interactiva (Tailwind CSS, Chart.js, Lucide Icons)
├── data.json          # Dataset completo estructurado (encuestas, dimensiones, KPIs)
├── README.md          # Documentación del proyecto y guía de uso
└── .gitignore         # Configuración de exclusión para Git
```

---

## 📈 Componentes del Dashboard

1. **KPI Cards Hero**: Tarjetas dinámicas que recalculan en tiempo real según los filtros activos.
2. **Filtros Interactivos**: Filtrado por establecimiento educacional (5 colegios) y rol (Estudiante / Docente Líder).
3. **Gráficos Estadísticos con Chart.js**:
   - Donut Chart con la distribución de Promotores, Pasivos y Detractores.
   - Gráfico de barras comparativo de NPS y Satisfacción por Establecimiento.
   - Ranking horizontal de las 12 dimensiones formativas y logísticas evaluadas.
4. **Matriz Detallada de Dimensiones**: Medias (1-5), recuento de notas 1 al 5, % satisfacción y NPS por ítem.
5. **Explorador Cualitativo con Buscador en Vivo**: Testimonios textuales de los participantes clasificados en:
   - ⭐ *Hitos de Mayor Valor*
   - 🔧 *Aspectos a Mejorar*
   - 💬 *Comentarios Adicionales*
6. **Base de Datos Completa**: Tabla con las 26 encuestas transcritas y badges de categorización NPS.

---

## 🏫 Establecimientos Participantes

- **Colegio Chuquicamata** (6 encuestas | NPS +100.0 pts)
- **Liceo Bicentenario Politécnico Cesáreo Aguirre Goyenechea** (6 encuestas | NPS +100.0 pts)
- **Liceo Minero América** (5 encuestas | NPS +100.0 pts)
- **Colegio Ecológico Montessori** (5 encuestas | NPS +40.0 pts)
- **Liceo Francisco de Aguirre (B-8)** (4 encuestas | NPS +75.0 pts)

---

## 📄 Archivos Complementarios del Proyecto

En el directorio del proyecto también se encuentran disponibles:
- **`Informe_Ejecutivo_NPS_Speakers_En_Verde_Calama_2026.pdf`**: Informe ejecutivo imprimible en formato A4 listo para presentación ante el comité.
- **`Speakers_En_Verde_Calama_2026_Evaluacion_NPS.xlsx`**: Libro de cálculo Excel con 4 pestañas formateadas profesionalmente.
- **`Respuestas_Speakers_En_Verde_Calama_2026.csv`**: Archivo plano para interoperabilidad con R, Python o PowerBI.

---

*Proyecto financiado y apoyado por el Comité Corfo Antofagasta a través del instrumento Viraliza Formación Código 25VIRTL-307467.*
