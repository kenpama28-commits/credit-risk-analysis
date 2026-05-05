\# 📊 Análisis de Riesgo Crediticio y Predicción de Morosidad


\## 🎯 Objetivo del proyecto

Análisis end-to-end de una cartera de 150.000 clientes bancarios para identificar 

patrones de morosidad, construir KPIs financieros ejecutivos y predecir el riesgo 

crediticio individual mediante modelos de machine learning.


\*\*Resultado clave:\*\* El modelo Gradient Boosting alcanzó un AUC-ROC de 0.8480,

identificando que los clientes de riesgo Alto tienen 20x más probabilidad de 

entrar en mora que los de riesgo Bajo.


\---


\## 🛠️ Stack tecnológico

| Herramienta | Uso en el proyecto |

|-------------|-------------------|

| Python · Pandas · NumPy         | Limpieza, transformación y análisis de datos |

| SQLite · SQLAlchemy             | Almacenamiento y consultas SQL de KPIs |

| Matplotlib · Seaborn            | Visualizaciones del análisis exploratorio |

| Scikit-learn · Imbalanced-learn | Modelos predictivos y balanceo SMOTE |

| Power BI · DAX                  | Dashboard ejecutivo interactivo |


\---

\## 📁 Estructura del proyecto



credit-risk-analysis/

├── data/

│   ├── raw/                  # Dataset original de Kaggle

│   └── processed/            # Datos limpios y KPIs exportados

│       └── kpis/             # Tablas de KPIs individuales

├── notebooks/

│   ├── 01\_data\_collection    # Descarga y primera exploración

│   ├── 02\_data\_cleaning      # Limpieza, nulos, outliers, SQL

│   ├── 03\_eda                # Análisis exploratorio y visualizaciones

│   ├── 04\_kpis               # Construcción de KPIs financieros

│   └── 05\_model              # Modelos predictivos y evaluación

├── reports/                  # Gráficos exportados y dashboard .pbix

├── sql/                      # Queries SQL documentadas

└── README.md


\---


\## 📈 Hallazgos principales



\- \*\*Tasa de morosidad global:\*\* 6.7% — por encima del benchmark del 5%

\- \*\*Segmento crítico:\*\* Riesgo Alto (7.5% de la cartera) concentra el 44% de toda la mora

\- \*\*Predictor más fuerte:\*\* Historial de atrasos pasados (`total\_atrasos`)

\- \*\*Señal temprana:\*\* Uso de crédito rotativo > 75% anticipa estrés financiero

\- \*\*Perfil de mayor riesgo:\*\* Clientes jóvenes (18–30 años) con múltiples atrasos



\---



\## 🤖 Resultados del modelo



| Modelo                  | AUC-ROC | Precision | Recall |              

| Regresión Logística     | 0.8080  | 0.1888    | 0.7521 |

| Random Forest           | 0.8227  | 0.2455    | 0.5332 |

| Gradient Boosting     ★| 0.8480   | 0.2068    | 0.7521 |



★ Modelo seleccionado para producción



\---



\## 📊 Dashboard Power BI



\[🔗 Ver dashboard interactivo](https://app.powerbi.com/links/UGVbHd0Nxf?ctid=577fc1d8-0922-458e-87bf-ec4f455eb600\&pbi\_source=linkShare)



\---



\## 🚀 Cómo reproducir el proyecto



```bash

\# 1. Clona el repositorio

git clone https://github.com/kenpama28-commits/credit-risk-analysis.git

cd credit-risk-analysis



\# 2. Instala dependencias

pip install -r requirements.txt



\# 3. Configura tu API key de Kaggle en \~/.kaggle/kaggle.json



\# 4. Ejecuta los notebooks en orden (01 → 05)

```



\---



\## 📬 Contacto



\*\*Kevin Palacio Martinez\*\*  \[kenpama28@gmail.com]



