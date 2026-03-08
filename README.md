## Propósito

El objetivo del presente análisis de  **"Churn de Clientes"** es exponer información valiosa derivada de la extracción, procesamiento y análisis exploratorio inicial con el propósito de que, en una segunda fase, se apliquen modelos predictivos y se desarrollen estrategias para reducir la evasión.

## Estructura

challenge2-data-science-LATAM/
│

├── graficas_informe/   # Directorio que almacena las imágenes de gráficas mostradas en el informe

├──pasos_p_estandarizacion.md    # Documenta en resumen los cambios hechos a las columnas

├── TelecomX_Data_prepared.csv    # Datos transformados con los nuevos formatos y columnas
├── TelecomX_Data.json      # Dataset en formato JSON

├── TelecomX_diccionario.md    # Diccionario de los datos originales

├── TelecomX_LATAM.ipynb    # Notebook principal con el analisis completo
└── README.md               # Documentacion del proyecto

## Insights

```markdown
***Los clientes perdidos superan una cuarta parte de todos los analizados*.**
![image.png](./graficas_informe/.png)

Factores que parecen mostrar relación las tasas de churn de clientes:

1. **Tipo de contrato por periodo**: 
    1. Contratos por mes tienden a presentar más cancelación.
    2. Los clientes con mayor tasa de churn suelen tener menos de 10 meses contratados en total.
2. **Tipo de servicio de internet**: Fibra óptica representa mayor tasa de churn frente a DSL.
3. **Edad del cliente**: Aprox. la mitad de clientes de 65 o más años cancelaron su contrato.
4. **Método de pago**: El pago electrónico es el que mayor tasa de churn presenta frente a los otros métodos.
5. **Dependientes del cliente:** Si el cliente tiene, hay más probabilidad de retención en TelecomX.
6. **Cuentas**:
    1. Los clientes que gastan más de 60 dólares al mes suelen tener una alta tasa de Churn.
    2. El 50% de clientes que cancelaron contrato lo hicieron cuando gastaron un máximo de ~134 dólares. 
```

## Instrucciones para ejecutar el notebook

1. Descargar el repositorio actual
2. Asegurarse de tener los prerrequisitos instalados en la computadora propia o entorno virtual con el que se ejecutará el notebook.
    1. Pyhton
    2. pandas
    3. numpy
    4. request
    5. matplotib
    6. plotly
3. Abrir el proyecto en VScode o Jupyter
4. Ir a TelecomX_LATAM.ipynb  y ejecutar todas las celdas secuencialmente.