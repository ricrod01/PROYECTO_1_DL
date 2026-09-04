CANDIDATOS AL PROYECTO FINAL:
  Se conservará el modelo C, el cual está compuesto de tras submodelos: CNN-1D, LSTM y Random Forest. Esto se ha hecho con el fin de que cada submodelo estará especializado en resolver un tipo de anomalía. Uno de los limitantes de este modelo es que el costo de entrenamiento es el segundo mayor de los tres modelos optimizados respecto al umbral. 

USO DE IA EN EL PROYECTO: 
  El uso de IA en el presente proyecto ha quedado restringido principalmente al mejoramiento del código implementado.
  También se ha usado para el arreglo de errores de sintaxis y mantenimiento de una estructura coherente de los códigos.

DECISIONES TÉCNICAS IMPORTANTES:
  1. La generación de datos por medio de código propio en lugar de buscar bases de datos en internet. Esto se ha hecho así, dado que se pensó en
     la dificultad de encontrar una base de datos que se acoplara con las necesidades del proyecto -como la cantidad de datos y la calidad de los mismos-
     sumado al hecho de que se tratase de datos relativos al sector bancario, que dificultaba la búsqueda.
  2. Elección de LSTM para el modelo B. Se consideró en primera instancia el uso de una GRU para este fin, ya que es un modelo relativamente más simple
      que el de LSTM. La decisión del uso de una LSTM se ha basado principalmente en el hecho de que se tenía cierta experiencia previa en su uso por medio
     de tareas, ejercicios y proyectos anteriores, por lo que ya se tenía parte de una plantilla para su elaboración.
  3. Estructura del modelo C. La elección de esta combinación de modelos se fundamenta en que cada submodelo esté especializado en un tipo de anomalía;
     de esta manera, cada submodelo aprende a reconocer los patrones de cada anomalía.

