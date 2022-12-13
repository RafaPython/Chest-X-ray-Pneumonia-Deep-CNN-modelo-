# Modelo para la detecciónd e neumonía mediante imagenes de rayos x utilizando un CNN profundo

Integrantes:

* Julio Emmanuel Meza Rangel
+ Carlos Rendón Hernández
* Rafael Alejandro García Ramírez



El presente trabajo es un modelo de red neuronal convolucional profundo que mediante los datos públicos obtenidos de Mendeley Data [3] que consisten en radiagrafías tomadas a infantes de entre 1 y 5 años de edad quienes acudieron al centro médico para mujeres y niños de Guangzhou en China, como parte de una revisión médica habitual.

Las imágenes se dividen en tres datasets, uno de entrenamiento, uno de prueba y uno de validación; cada uno con las imágenes clasificadas como 'Normal' para los pacientes sanos y 'Pneumonia' para los pacientes positivos a neumonía. Esta clasificación fue realizada por dos expertos del hospital de Guangzhou.

Dentro de este proyecto se realiza una red convolucional profunda para la clasificación. Se utilizó para la construcción la paquetería de tensorflow y keras con kernels cuyos parámetro se ajustan con el entrenamiento del modelo. Esto nos permite un mejor entrenamiento al no tener que realizar una capa por cada elemento de la imagen (dígase lineas verticales, horizontales o formas en específico), esto es de gran ayuda pues dentro de las imágenes no se puede percibir una forma en concreto a identificar dentro de aquellas positivas.

El proceso de diagnóstico de la neumonía consiste en realizar una radiografía del tórax donde un experto analiza si existe inflamación en los pulmones, posteriormente se realiza un análisis de sangre para determinar si el sistema inmunitario se encuetra luchando contra una infección. Este método muy habitualmente permite un diagnóstico relativamente más rápido que otros métodos, siento que es casi inmediato de no ser por la necesidad de que un especialista determine las condiciones; es por ello del posible interés de acotar este paso para su rápido diagnóstico.

El dataset utilizado para este proyecto se puede encontrar tanto en la pagina de Mendeley Data en el artículo Labeled Optical Coherence Tomography (OCT) and Chest X-Ray Images for Classification o también dentro de la plataforma Kaggle dentro de la publicación Chest X-Ray Images (Pneumonia)
