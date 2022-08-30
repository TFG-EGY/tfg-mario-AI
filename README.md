# Implementaciones de bots de Super Mario Bros
## Configuración del entorno
Para este proyecto se debe usar una versión de Python inferior a la v: 8.  
Además, se debe tener instalado el toolkit de **Jupyter notebook**, ya que es donde va a tener lugar el desarrollo del código.

Se ha de instalar la librería **PyTorch** según las especificaciones hardware de nuestro equipo. [Enlace](https://pytorch.org/) a la guía de instalación oficial.  
Para la instalación del resto de dependencias necesarias:  
`pip install -r requirements`

Una vez esto podemos decir que se tenemos configuradas las dependecias necesarias para poder ejecutar o entrenar las implementaciones de este repositorio.

## Organización del código
Las carpetas principales son: DDQN, DQN y PPO. Los subdirectorios de cada una de ellas son los siguientes:  
* DQN: aquí se sitúa la primera versión de la implementación de DQN
    * /models: en este directorio deberán situarse los modelos entrenados resultantes  

* DDQN  
    * /models
        * ddqn: aquí se encuentra la implementación del algoritmo DDQN y los archivos .csv de datos para extraer métricas. En este directorio deberán situarse también los archivos del modelo entrenado.  
        * dqn: aquí se encuentra la versión DQN que usa el mismo código que DDQN, también se encuentran los archivos .csv de datos para extraer métricas. En este directorio deberán situarse también los archivos del modelo entrenado.  

* PPO: aquí se encuentra el notebook de la implementación con el algoritmo PPO. También se encuentran los archivos .csv de datos para extraer métricas.
    * /train: aquí deberá situarse el modelo entrenado obtenido. En caso de realizar el entrenamiento el modelo resultante se creará en este diretorio.

* En el directorio raíz se encuentra el notebook *tests.ipynb*, donde se ha realizado la implementación del código necesario para realizar la comparativa entre los resultados de los algoritmos.

## Modelos entrenados
Los archivos de los modelos entrenados, en caso de desear visualizar el comportamiento de los bots, por cuestiones de almacenamiento se encuentran alojados en el siguiente enlace: [Modelos entrenados](https://hdvirtual.us.es/discovirt/index.php/s/wq2jkdG73WDmF4t)  
Para facilitar el entendimiento de dichos archivos, se ha organizado de la misma manera que en el repositorio de GitHub, de manera que solamente se deben arrastrar a la misma carpeta en la que se encuentran alojados.

## Ejecución de los bots entrenados
Para la ejecución de los bots entrenados, en primer lugar deberán situarse los archivos en las carpetas indicadas y luego, dependiendo de cada algoritmo, se deberán seguir las instrucciones descritas en cada notebook de cada implementación.