**English**:
This code performs several operations for manipulating, analyzing, and visualizing customer churn data, including steps for data transformation, dataframe unification, handling missing values, univariate and bivariate analysis, as well as statistical tests like the Chi-Square test. Here's a summary of what each part does:

1. **Data Loading**:

   - Loads three CSV datasets: `churn_contracts.csv`, `churn_customers.csv`, and `churn_services.csv`.

2. **Data Transformation**:

   - Converts the `TotalCharges` column from string to float, handles missing values, and renames columns in `df_customers`.
   - Permanently renames the `SeniorCitizen` column to `Above65yo` and changes column names in `df_customers`.

3. **DataFrame Unification**:

   - Merges customer, service, and contract dataframes to create a single `df_churn` dataframe.

4. **Missing Value Detection and Handling**:

   - Detects missing values and uses different approaches to handle them, including removing rows and columns and imputing values with 0 or the mean.

5. **Univariate Analysis**:

   - Performs counting and visualization of the distribution of the `Churn` variable (customers who have left or stayed) and other variables like `Contract` (contract type) and `Tenure` (contract duration).

6. **Bivariate Analysis**:

   - Explores the correlation between the `Churn` and `Contract` variables and tests the hypothesis that customers with monthly contracts are more likely to churn using the Pearson Chi-Square test.

7. **Hypothesis Testing - Chi-Square**:

   - Performs the Chi-Square test to verify the correlation between qualitative variables, like `Churn` and `Contract`, and between `Churn` and a transformed variable, such as `TempoMenor6Meses`.

8. **Correlation Between Numerical Variables**:
   - Calculates the correlation between numerical variables like `Tenure` and `TotalCharges` to explore the relationship between contract duration and payment amount.

This code is a complete example of how to explore and analyze a customer churn dataset using pandas, matplotlib, and scipy for visualization and statistical tests.

1. Clone Repo

2. Install Dependencies

```bash
pip install -r requirements.txt
```

3. Run Jupyter notebook

---

**Spanish**:
Este código realiza varias operaciones de manipulación, análisis y visualización de datos sobre churn de clientes, incluyendo las etapas de transformación de datos, unificación de dataframes, tratamiento de valores ausentes, análisis univariado y bivariado, además de pruebas estadísticas como el test de Chi-Cuadrado. Aquí está un resumen de lo que hace cada parte:

1. **Carga de datos**:

   - Carga tres datasets CSV: `churn_contracts.csv`, `churn_customers.csv` y `churn_services.csv`.

2. **Transformación de datos**:

   - Convierte la columna `TotalCharges` de cadena a flotante, maneja los valores ausentes y renombra columnas en `df_customers`.
   - Renombra permanentemente la columna `SeniorCitizen` a `Above65yo` y cambia los nombres de las columnas en `df_customers`.

3. **Unificación de DataFrames**:

   - Realiza merges entre los dataframes de clientes, servicios y contratos para crear un único dataframe `df_churn`.

4. **Detección y tratamiento de valores ausentes**:

   - Detecta valores ausentes y utiliza diferentes enfoques para manejarlos, incluyendo la eliminación de filas y columnas, así como la imputación de valores con 0 o la media.

5. **Análisis univariado**:

   - Realiza el conteo y la visualización de la distribución de la variable `Churn` (clientes que dejaron o no el servicio) y otras variables como `Contract` (tipo de contrato) y `Tenure` (tiempo de contrato).

6. **Análisis bivariado**:

   - Explora la correlación entre las variables `Churn` y `Contract` y prueba la hipótesis de que los clientes con contrato mensual tienen mayor propensidad al churn usando el test de Chi-Cuadrado de Pearson.

7. **Prueba de Hipótesis - Chi-Cuadrado**:

   - Realiza el test de Chi-Cuadrado para verificar la correlación entre variables cualitativas, como `Churn` y `Contract`, y entre `Churn` y una variable transformada, como `TempoMenor6Meses`.

8. **Correlación entre variables numéricas**:
   - Calcula la correlación entre variables numéricas como `Tenure` y `TotalCharges` para explorar la relación entre el tiempo de contrato y el valor pagado.

Este código es un ejemplo completo de cómo explorar y analizar un conjunto de datos de churn de clientes utilizando pandas, matplotlib y scipy para visualización y pruebas estadísticas.

---

**Português**:
Este código realiza várias operações de manipulação, análise e visualização de dados sobre churn de clientes, incluindo as etapas de transformação de dados, unificação de dataframes, tratamento de valores ausentes, análise univariada e bivariada, além de testes estatísticos como o teste Qui-Quadrado. Aqui está um resumo do que cada parte faz:

1. **Carregamento de dados**:

   - Carrega três datasets CSV: `churn_contracts.csv`, `churn_customers.csv`, e `churn_services.csv`.

2. **Transformação de dados**:

   - Converte a coluna `TotalCharges` de string para float, lida com valores ausentes e renomeia colunas em `df_customers`.
   - Renomeia permanentemente a coluna `SeniorCitizen` para `Above65yo` e altera os nomes das colunas no `df_customers`.

3. **Unificação de DataFrames**:

   - Faz merges entre os dataframes de clientes, serviços e contratos para criar um único dataframe `df_churn`.

4. **Detecção e tratamento de valores ausentes**:

   - Detecta valores ausentes e usa diferentes abordagens para lidar com eles, incluindo a remoção de linhas e colunas, bem como a imputação de valores com 0 ou a média.

5. **Análise univariada**:

   - Realiza contagem e visualização da distribuição da variável `Churn` (clientes que abandonaram ou não o serviço) e outras variáveis como `Contract` (tipo de contrato) e `Tenure` (tempo de contrato).

6. **Análise bivariada**:

   - Explora a correlação entre as variáveis `Churn` e `Contract` e testa a hipótese de que clientes com contrato mensal têm maior propensão ao churn usando o teste Qui-Quadrado de Pearson.

7. **Teste de Hipótese - Qui-Quadrado**:

   - Realiza o teste de Qui-Quadrado para verificar a correlação entre variáveis qualitativas, como `Churn` e `Contract`, e entre `Churn` e uma variável transformada, como `TempoMenor6Meses`.

8. **Correlação entre variáveis numéricas**:
   - Calcula a correlação entre variáveis numéricas como `Tenure` e `TotalCharges` para explorar a relação entre o tempo de contrato e o valor pago.

Esse código é um exemplo completo de como explorar e analisar um conjunto de dados de churn de clientes utilizando pandas, matplotlib e scipy para visualização e testes estatísticos.
