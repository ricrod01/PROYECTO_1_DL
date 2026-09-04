REPRODUCCIÓN:

  1. Se ha usado Python 3.13.7. con las siguientes librerías:
     - matplotlib: 3.10.6
     - pandas: 2.3.3
     - scikit-learn: 1.7.2
     - joblib: 1.5.3
     - numpy: 2.3.3
     - tensorflow: 2.21.0
     - statistics: 3.13.7
  3. La semilla usada ha sido seed=0
  4. El conjunto de datos utilizados contaba con 100,000 datos, de los cuales 89,936 eran transacciones normales, 3,994 eran de anomalías debido al orden no congruente, 3,611 eran de anomalías debido a transacciones cortas (muchas transacciones en poco tiempo) y 2,459 eran anomalías debido a compras en establecimientos no comunes para el cliente. Este conjunto no se incluye en el repositorio debido a su peso, pero puede ser generado usando el archivo generador_datos.ipynb.

VERSIONES

  1. Los modelos se encuentran en los archivos .pkl, .joblib y .keras. Además, la lógica del modelo C (mejor modelo) se encuentra en el archivo modelo_c.py.
  2. Las versiones de los modelos consiste principalmente en la actualización del umbral, con el fin de reducir los costos.

USO DE IA EN EL PROYECTO: 

  El uso de IA en el presente proyecto ha quedado restringido principalmente al mejoramiento del código implementado.
  También se ha usado para el arreglo de errores de sintaxis y mantenimiento de una estructura coherente de los códigos.

DECISIONES TÉCNICAS IMPORTANTES:
  1. La generación de datos por medio de código propio en lugar de buscar bases de datos en internet. Esto se ha hecho así, dado que se pensó en
     la dificultad de encontrar una base de datos que se acoplara con las necesidades del proyecto -como la cantidad de datos y la calidad de los mismos-
     sumado al hecho de que se tratase de datos relativos al sector bancario, que dificultaba la búsqueda.
  2. Elección de LSTM para el modelo B. Se consideró en primera instancia el uso de una GRU para este fin, ya que es un modelo relativamente más simple
      que el de LSTM. La decisión del uso de una LSTM se ha basado debido a su mejor capacidad predictiva.
  3. Estructura del modelo C. La elección de esta combinación de modelos se fundamenta en que cada submodelo esté especializado en un tipo de anomalía;
     de esta manera, cada submodelo aprende a reconocer los patrones de cada anomalía.

CANDIDATO AL PROYECTO FINAL:

Se conservará el modelo C, el cual está compuesto de tras submodelos: CNN-1D, LSTM y Random Forest. Esto se ha hecho con el fin de que cada submodelo estará especializado en resolver un tipo de anomalía. Uno de los limitantes de este modelo es que el costo de entrenamiento es el segundo mayor de los tres modelos optimizados respecto al umbral. 
