# Proyecto Final – Analítica Avanzada de Datos

Proyecto final de la unidad de aprendizaje **Analítica Avanzada** (Sexto Semestre, Ciencia de Datos).

Análisis y modelado predictivo sobre datos hospitalarios de pacientes con diabetes: limpieza de datos, ingeniería de variables y construcción de un pipeline de machine learning.

## Contenido

| Archivo | Descripción |
|---|---|
| `ProyectoFinal_Hospital_Completo (1).ipynb` | Notebook con el análisis completo (código, resultados e interpretaciones). |
| `ProyectoFinalAnalítica.pdf` | Reporte final del proyecto. |
| `description.pdf` | Enunciado / descripción del proyecto. |
| `diabetic_data.csv` | Conjunto de datos de encuentros hospitalarios de pacientes diabéticos. |

## Resumen del trabajo

1. **Exploración de datos** del dataset hospitalario.
2. **Tratamiento de valores nulos** sin eliminar filas ni columnas:
   - Categoría explícita `"Missing"` para variables categóricas con muchos nulos (p. ej. `weight`, `diag_1/2/3`).
   - Imputación por moda dentro de grupos similares (`age`, `gender`) para resultados de laboratorio (`max_glu_serum`, `A1Cresult`).
3. **Ingeniería de variables:**
   - Agrupación de códigos CIE-9 (`diag_1`, `diag_2`, `diag_3`) en macro-categorías clínicas.
   - Variables de polifarmacia: `n_medicamentos_activos`, `treatment_complexity`, `polypharmacy_index`, `insulin_change`.
4. **Pipeline de modelado** con codificación de variables (One-Hot y Target Encoding).

## Cómo ejecutarlo

1. Clona el repositorio:
   ```bash
   git clone https://github.com/sofiarodriguezzz/Proyecto-Analitica-Avanzada-de-Datos.git
   cd Proyecto-Analitica-Avanzada-de-Datos
   ```
2. Instala las dependencias habituales (`pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`, `jupyter`).
3. Abre el notebook con Jupyter y ejecútalo en orden, manteniendo `diabetic_data.csv` en la misma carpeta.

## Autora

Sofía – Estudiante de Ciencia de Datos
