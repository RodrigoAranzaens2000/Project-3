# Proyecto de Análisis de Datos de Instacart

## Descripción del Proyecto

En este proyecto, trabajarás con datos de Instacart.

Instacart es una plataforma de entregas de comestibles donde los clientes pueden registrar un pedido y recibirlo en su domicilio, similar a Uber Eats y DoorDash. Este conjunto de datos fue lanzado públicamente por Instacart en 2017 para una competición en Kaggle. Los datos reales pueden descargarse directamente desde la página de la competición en Kaggle.

El conjunto de datos proporcionado ha sido modificado respecto al original. Se ha reducido el tamaño del conjunto para agilizar los cálculos y se han introducido valores ausentes y duplicados. Se ha tenido cuidado de conservar las distribuciones de los datos originales al realizar estos cambios.

Tu misión es limpiar los datos y preparar un informe que brinde información sobre los hábitos de compra de los clientes de Instacart. Después de responder a cada pregunta, escribe una breve explicación de tus resultados en una celda markdown de tu Jupyter notebook.

Este proyecto requerirá que hagas gráficos que comuniquen tus resultados. Asegúrate de que cualquier gráfico que crees tenga un título, ejes etiquetados y una leyenda si es necesario; e incluye `plt.show()` al final de cada celda con un gráfico.

## Diccionario de Datos

Hay cinco tablas en el conjunto de datos, y tendrás que usarlas todas para hacer el preprocesamiento de datos y el análisis exploratorio de datos. A continuación se muestra un diccionario de datos que enumera las columnas de cada tabla y describe los datos que contienen.

### instacart_orders.csv

Cada fila corresponde a un pedido en la aplicación Instacart.
- **order_id**: Número de ID que identifica de manera única cada pedido.
- **user_id**: Número de ID que identifica de manera única la cuenta de cada cliente.
- **order_number**: El número de veces que este cliente ha hecho un pedido.
- **order_dow**: Día de la semana en que se hizo un pedido (0 si es domingo).
- **order_hour_of_day**: Hora del día en que se hizo el pedido.
- **days_since_prior_order**: Número de días transcurridos desde que este cliente hizo su pedido anterior.

### products.csv

Cada fila corresponde a un producto único que pueden comprar los clientes.
- **product_id**: Número ID que identifica de manera única cada producto.
- **product_name**: Nombre del producto.
- **aisle_id**: Número ID que identifica de manera única cada categoría de pasillo de víveres.
- **department_id**: Número ID que identifica de manera única cada departamento de víveres.

### order_products.csv

Cada fila corresponde a un artículo pedido en un pedido.
- **order_id**: Número de ID que identifica de manera única cada pedido.
- **product_id**: Número ID que identifica de manera única cada producto.
- **add_to_cart_order**: El orden secuencial en el que se añadió cada artículo en el carrito.
- **reordered**: 0 si el cliente nunca ha pedido este producto antes, 1 si lo ha pedido.

### aisles.csv

- **aisle_id**: Número ID que identifica de manera única cada categoría de pasillo de víveres.
- **aisle**: Nombre del pasillo.

### departments.csv

- **department_id**: Número ID que identifica de manera única cada departamento de víveres.
- **department**: Nombre del departamento.

## Estructura del Proyecto

El proyecto está estructurado de la siguiente manera:

- **data/**: Contiene los datos crudos proporcionados.
- **notebooks/**: Jupyter notebooks para el análisis y visualización de datos.
- **scripts/**: Scripts de Python para el procesamiento y análisis de datos.
- **reports/**: Documentación e informes sobre hallazgos y recomendaciones.

## Cómo Empezar

Para empezar con el proyecto, sigue estos pasos:

1. Clona el repositorio:
    ```bash
    git clone https://github.com/RodrigoAranzaens2000/Project-3.git
    ```

2. Navega al directorio del proyecto:
    ```bash
    cd Project-3
    ```

3. Configura un entorno virtual e instala las dependencias necesarias:
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # En Windows usa `venv\Scripts\activate`
    pip install -r requirements.txt
    ```

4. Explora los datos y los notebooks de análisis en el directorio `notebooks/`.

## Contribuir

Aceptamos contribuciones para mejorar el proyecto. Para contribuir, por favor sigue estos pasos:

1. Haz un fork del repositorio.
2. Crea una nueva rama:
    ```bash
    git checkout -b feature/tu-nueva-funcionalidad
    ```
3. Realiza tus cambios y haz commit:
    ```bash
    git commit -m 'Añadir nueva funcionalidad'
    ```
4. Sube los cambios a la rama:
    ```bash
    git push origin feature/tu-nueva-funcionalidad
    ```
5. Abre un pull request.


## Contacto

Para cualquier pregunta o consulta, por favor contáctanos en [aranzaensrodrigo@gmail.com](mailto:aranzaensrodrigo@gmail.com).

---

¡Gracias por contribuir al Proyecto de Análisis de Datos de Instacart!
