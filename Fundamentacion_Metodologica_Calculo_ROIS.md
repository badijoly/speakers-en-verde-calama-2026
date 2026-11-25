# Marco Metodológico y Fundamentación Teórica del Indicador ROIS
## Retorno sobre la Inversión Social (SROI) • Programa Speakers En Verde Calama 2026
**Instrumento:** Corfo Viraliza Formación • Código 25VIRTL-307467  
**Entidad Ejecutora:** Verdical SpA  
**Territorio de Aplicación:** Comuna de Calama, Provincia de El Loa, Región de Antofagasta  
**Fecha de Emisión:** Noviembre 2026  

---

## 1. Fundamentación y Origen de la Estrategia de Cálculo

### 1.1. Antecedentes y Limitación de las Evaluaciones Tradicionales
En los programas públicos de formación, emprendimiento e innovación ambiental (como los fondos *Viraliza Formación* de Corfo), la rendición tradicional suele restringirse a métricas de cobertura administrativa: número de personas inscritas, porcentaje de asistencia bruta y encuestas finales de satisfacción (NPS).

Si bien estas métricas son necesarias, **no cuantifican el valor social, pedagógico ni territorial que el programa deja instalado en la comunidad**. Evaluar una inversión pública de \$35.000.000 CLP únicamente por la cantidad de firmas en una lista desconoce:
1. El contexto de vulnerabilidad socioeducativa de los colegios beneficiarios.
2. La severidad del entorno bioclimático donde se implementan las soluciones (aridez extrema y radiación en el Desierto de Atacama).
3. La ganancia psicométrica real de competencias (efectividad del aprendizaje).
4. El efecto multiplicador que los proyectos de los estudiantes tienen en sus hogares y liceos.
5. Los costos evitados en mitigación ambiental derivados de los proyectos escolares.

### 1.2. Marcos de Referencia Internacional y Nacional
Para resolver esta brecha, Verdical SpA diseñó un modelo econométrico adaptado de **Retorno sobre la Inversión Social (ROIS)** fundamentado en tres pilares metodológicos consolidados:

1. **Guía Internacional SROI (*A Guide to Social Return on Investment*, Social Value International / Cabinet Office UK):**  
   Establece el principio de monetización de externalidades positivas y cambios socioeconómicos intangibles, comparando el valor presente de los beneficios sociales netos frente a la inversión inicial ($SROI = \frac{\text{Beneficio Social Monetizado}}{\text{Inversión Total}}$).
2. **Sistema Nacional de Inversiones (Ministerio de Desarrollo Social y Familia - MDSF, Chile):**  
   Adopta los principios de precios sombra, evaluación social de capital humano y factores de corrección territorial para zonas extremas o aisladas del país.
3. **Métrica Psicométrica de Richard Hake (1998, *American Journal of Physics*):**  
   Aplica la fórmula de ganancia pedagógica normalizada ($g$) para medir objetivamente la fracción de la brecha de conocimiento que un programa logra cerrar entre la evaluación diagnóstica (*ex-ante*) y la evaluación de egreso (*ex-post*).

---

## 2. Formulación Algorítmica General

El índice **ROIS** se calcula mediante la siguiente función de valor social:

$$\text{ROIS} = \frac{[ ( ID \times FP_{\text{vuln}} + IR_{\text{efectivo}} ) \times F_{\text{bioclima}} \times (1 + g_{\text{Hake}}) \times V_{\text{base}} + CAE ]}{CTI}$$

Donde:
* **$ID$**: Impacto Directo (Beneficiarios plenos ponderados por asistencia real).
* **$FP_{\text{vuln}}$**: Factor de Vulnerabilidad Socioeducativa y Territorial.
* **$IR_{\text{efectivo}}$**: Impacto Replicado en Hogares y Comunidad Escolar (Efecto Cascada).
* **$F_{\text{bioclima}}$**: Factor de Ajuste Bioclimático por Zona Hiperárida y Desértica.
* **$g_{\text{Hake}}$**: Ganancia Normalizada de Aprendizaje Psicométrico (Hake).
* **$V_{\text{base}}$**: Valor Social de Referencia por Unidad Formativa Estandarizada (\$777.415 CLP).
* **$CAE$**: Costos Ahorrados por Mitigación Ambiental y Alertas Tempranas.
* **$CTI$**: Costo Total de Inversión Ejecutada.

---

## 3. Desglose Conceptual y Justificación de Cada Factor

```
                                      FÓRMULA ALGORÍTMICA ROIS
┌──────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                                  │
│   ROIS = [ ( ID × FP_vuln + IR_efectivo ) × F_bioclima × (1 + g_Hake) × V_base + CAE ] / CTI    │
│                                                                                                  │
└───────────────┬──────────────────────┬─────────────┬──────────────┬───────────────┬──────────────┘
                │                      │             │              │               │
         ┌──────┴──────┐        ┌──────┴──────┐ ┌────┴─────┐ ┌──────┴──────┐ ┌─────┴──────┐
         │ ID × FP_vuln│        │IR_efectivo  │ │F_bioclima│ │  g_Hake     │ │   CAE      │
         │  17.58 × 1.25│       │   15.00 pers│ │   1.15   │ │   +25.5%    │ │ $12.5M CLP │
         │   = 21.98   │        │  (Hogares)  │ │ (Aridez) │ │(Aprendizaje)│ │(Mitigación)│
         └─────────────┘        └─────────────┘ └──────────┘ └─────────────┘ └────────────┘
```

---

### Variable 1: Impacto Directo Ponderado ($ID = 17,58$ alumnos plenos)
* **¿Qué representa?**  
  El número equivalente de estudiantes que completaron íntegramente la experiencia formativa, corregido por su asistencia efectiva verificada en actas físicas.
* **Base de Cálculo:**  
  $$\text{N° Inscritos en Nómina Regular} \times \text{Tasa de Asistencia Promedio en Terreno}$$
  $$25 \text{ estudiantes} \times 70,33\% = 17,5825 \approx \mathbf{17,58\text{ alumnos equivalentes}}$$
* **Justificación Metodológica:**  
  Evita asumir que los 25 inscritos recibieron el 100% del programa. Premia la permanencia real en aula y mentorías (163 asistencias efectivas sobre 234 convocatorias programadas).

---

### Variable 2: Factor de Vulnerabilidad Socioeducativa ($FP_{\text{vuln}} = 1,25$)
* **¿Qué representa?**  
  Un ponderador de equidad territorial y educativa que reconoce el valor social superior de formar estudiantes en contextos de alta vulnerabilidad.
* **Base de Cálculo:**  
  Ponderador de **$1,25$ (+25% de sobrevaloración)** fundamentado en los índices oficiales IVE-SINAE (Índice de Vulnerabilidad Escolar de JUNAEB) de los establecimientos participantes en Calama:
  - *Liceo Bicentenario Politécnico Cesáreo Aguirre Goyenechea (TP)*: IVE > 85%.
  - *Liceo Minero América*: IVE > 80%.
  - *Liceo Francisco de Aguirre (B-8)*: IVE > 82%.
* **Justificación Metodológica:**  
  Bajo las directrices de inversión social del Estado chileno, intervenir pedagógicamente en establecimientos técnico-profesionales municipales y vulnerables de provincia tiene un retorno social de movilidad superior al de colegios particulares de la capital.
  $$\text{Impacto Directo Ponderado} = ID \times FP_{\text{vuln}} = 17,5825 \times 1,25 = \mathbf{21,98\text{ unidades}}$$

---

### Variable 3: Impacto Replicado en Hogares y Comunidad Escolar ($IR_{\text{efectivo}} = 15,00$ beneficiarios)
* **¿Qué representa?**  
  El efecto cascada o multiplicador secundario generado por la transferencia de las soluciones ambientales formuladas por los equipos hacia sus familias y pares de colegio.
* **Base de Cálculo:**  
  5 proyectos escolares finalizados y defendidos en el Demoday $\times$ 3 beneficiarios directos del núcleo familiar/escolar vinculados a la adopción del proyecto = **$15,00$ personas**.
* **Justificación Metodológica:**  
  Las metodologías SROI exigen computar los beneficiarios indirectos validados cuando existe evidencia de transferencia tecnológica o cambios conductuales en los hogares (gestión de residuos, compostaje o uso racional de recursos hídricos impulsados por los estudiantes).
  $$\text{Núcleo Social Base} = (ID \times FP_{\text{vuln}}) + IR_{\text{efectivo}} = 21,98 + 15,00 = \mathbf{36,98\text{ unidades de impacto}}$$

---

### Variable 4: Factor Bioclimático de Aridez ($F_{\text{bioclima}} = 1,15$)
* **¿Qué representa?**  
  Ajuste territorial que premia el desarrollo y la implementación de soluciones ambientales adaptadas a las restricciones bioclimáticas extremas de la Provincia de El Loa.
* **Base de Cálculo (Desglose Aditivo de 3 Componentes de +5%):**
  - **Base Neutral:** $1,00$ (condición estándar de zona templada/central).
  - **Componente A — Estrés Hídrico Severo y Radiación UV (+0,05):** Calama enfrenta decretos de escasez hídrica continua y los niveles de radiación solar más altos del mundo. Formar capital humano capaz de mitigar estos factores añade un valor ecosistémico diferencial.
  - **Componente B — Pertinencia de Adaptación al Desierto (+0,05):** Reconoce que los prototipos no son genéricos, sino adaptados a suelos salinos, polvo en suspensión de faenas mineras y alta oscilación térmica.
  - **Componente C — Factor Zona Extrema / Aislamiento (+0,05):** Reconocimiento de costos logísticos y menor oferta de programas de economía circular en la macrozona norte respecto a la zona central (análogo al factor de localización de MIDEPLAN/MDSF).
  $$F_{\text{bioclima}} = 1,00 + 0,05 + 0,05 + 0,05 = \mathbf{1,15\text{ (+15% de ajuste territorial)}}$$
* **Efecto en la Fórmula:**
  $$\text{Impacto Ajustado por Bioclima} = 36,98 \times 1,15 = \mathbf{42,52\text{ unidades}}$$

---

### Variable 5: Ganancia Psicométrica de Aprendizaje ($g_{\text{Hake}} = 0,255$ / $+25,5\%$)
* **¿Qué representa?**  
  La fracción de la brecha máxima posible de aprendizaje que los estudiantes efectivamente lograron cerrar durante el programa.
* **Formulación de Richard Hake (1998):**
  $$g = \frac{\% \text{Post} - \% \text{Pre}}{100\% - \% \text{Pre}}$$
* **Datos Empíricos del Programa:**
  - Diagnóstico Inicial (*Ex-Ante*): $20,7\%$ de dominio autónomo en competencias de sostenibilidad, oratoria y pitch.
  - Egreso del Programa (*Ex-Post*): $57,7\%$ de dominio autónomo.
  - Ganancia neta absoluta: $+37,0$ puntos porcentuales.
  $$g = \frac{57,7\% - 20,7\%}{100\% - 20,7\%} = \frac{37,0\%}{79,3\%} = \mathbf{0,255\text{ (+25,5% de ganancia normalizada)}}$$
* **Justificación Metodológica:**  
  La ganancia de Hake es el estándar dorado en educación técnica y científica para evitar el sesgo de la nota de entrada. Indica que el programa cerró más de un cuarto de todo lo que los alumnos desconocían inicialmente.
* **Multiplicador Pedagógico:**
  $$(1 + g_{\text{Hake}}) = 1 + 0,255 = \mathbf{1,255}$$
  $$\text{Valor Social Pedagógico} = 42,52 \times 1,255 = \mathbf{53,37\text{ unidades de impacto total}}$$

---

### Variable 6: Valor Social Unitario y Retorno Formativo (\$41.493.639 CLP)
* **Monetización:**
  Las $53,37$ unidades de impacto se valorizan con base en el costo social de formación técnica especializada por participante certificado en la Región de Antofagasta ($V_{\text{base}} = \$777.415$ CLP):
  $$53,37 \text{ unidades} \times \$777.415\text{ CLP} = \mathbf{\$41.493.639\text{ CLP}}$$

---

### Variable 7: Costos Ahorrados por Mitigación Ambiental ($CAE = \$12.500.000$ CLP)
* **¿Qué representa?**  
  Costos que las instituciones públicas, liceos y municipalidades evitan desembolsar gracias a las soluciones tempranas, sensibilización y planes de reciclaje/eficiencia diseñados en el programa.
* **Base de Cálculo:**  
  5 proyectos escolares avaluados en un beneficio social conservador de $\$2.500.000$ CLP anuales cada uno por concepto de:
  - Disminución de residuos enviados a vertedero comunal.
  - Ahorro en consumo hídrico de áreas verdes escolares.
  - Mitigación de riesgos de microbasurales perimetrales.
  $$5 \text{ proyectos} \times \$2.500.000\text{ CLP} = \mathbf{\$12.500.000\text{ CLP}}$$

---

### Variable 8: Costo Total de Inversión Ejecutada ($CTI = \$35.000.000$ CLP)
* Presupuesto íntegramente ejecutado y rendido, compuesto por:
  - **Subsidio Comité Corfo Antofagasta (Fondo Viraliza Formación):** \$24.500.000 CLP (70%).
  - **Aporte y Cofinanciamiento Institucional:** \$10.500.000 CLP (30%).
  $$\text{Inversión Total (CTI)} = \mathbf{\$35.000.000\text{ CLP}}$$

---

## 4. Síntesis Numérica Paso a Paso del ROIS Auditado

| Paso | Operación Matemática | Resultado Parcial | Significado |
| :---: | :--- | :---: | :--- |
| **1** | $ID = 25 \times 70,33\%$ | **17,58** | Alumnos plenos equivalentes por asistencia |
| **2** | $ID \times FP_{\text{vuln}} = 17,58 \times 1,25$ | **21,98** | Ajuste por alta vulnerabilidad escolar |
| **3** | $(ID \times FP_{\text{vuln}}) + IR_{\text{efectivo}} = 21,98 + 15,00$ | **36,98** | Núcleo de beneficiarios directos + hogares |
| **4** | Núcleo $\times F_{\text{bioclima}} = 36,98 \times 1,15$ | **42,52** | Ajuste por condiciones de aridez en Calama |
| **5** | Bioclima $\times (1 + g_{\text{Hake}}) = 42,52 \times 1,255$ | **53,37** | Ponderación por ganancia pedagógica efectiva |
| **6** | Monetización Formativa ($53,37 \times \$777.415$) | **\$41.493.639 CLP** | Valor de capital humano instalado |
| **7** | Retorno Social Total ($\$41.493.639 + \$12.500.000 CAE$) | **\$53.993.639 CLP** | Valor social consolidado generado |
| **8** | **Ratio Final ROIS** ($\$53.993.639 / \$35.000.000 CTI$) | **1,54x** | **Por cada \$1 invertido se retornan \$1,54 al territorio** |

---

## 5. Análisis de Viabilidad y Estándares de Aprobación

```
 Umbral Crítico de Viabilidad (1.00x)                    Resultado Auditado (1.54x)
───────────────┬────────────────────────────────────────────────────▲────────
               │                                                    │
               │            Zona de Retorno Social Positivo         │
  Destrucción  │                                                    │
   de Valor    │  +$0,54 de beneficio neto por cada $1 invertido   │
```

1. **Superación del Umbral de Viabilidad:**  
   En evaluación social de proyectos, un índice superior a **$1,00x$** certifica que la iniciativa no destruye valor público ni constituye un gasto a fondo perdido, sino una inversión con retorno socioeconómico neto positivo.
2. **Retorno Específico sobre el Subsidio Estatal Corfo:**  
   Si se compara el retorno social (\$53.993.639 CLP) frente al subsidio público adjudicado por Corfo (\$24.500.000 CLP), el ratio asciende a **$2,20x$** en el primer año y a **$3,18x$** proyectado a 5 años por la vigencia de las capacidades instaladas.
3. **Respaldo ante Auditorías Técnicas:**  
   Cada variable cuenta con respaldo empírico auditable:
   - Asistencias respaldadas en 37 actas físicas firmadas en Calama.
   - Ganancia de Hake respaldada en 51 evaluaciones psicométricas (31 pre y 20 post).
   - Vulnerabilidad escolar respaldada en registros públicos SINAE-JUNAEB.

---

*Documento técnico preparado por Verdical SpA como anexo metodológico del cierre del proyecto Viraliza Formación Corfo 25VIRTL-307467.*
