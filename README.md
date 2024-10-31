# Examen Parcial - NLP
Este repositorio contiene un conjunto de implementaciones de algoritmos y modelos de procesamiento del lenguaje natural (NLP) y sus respectivos análisis. El proyecto abarca desde modelos de n-gramas con suavizado hasta técnicas avanzadas como Word2Vec y GloVe, aplicadas a un corpus de ejemplo en español.

## Contenido
1. Descripción
2. Modelos Implementados
3. Análisis y Resultados
4. Referencias


## Descripción
Este proyecto explora diversos modelos de NLP, desde técnicas estadísticas hasta modelos de representación de palabras mediante embeddings. Cada modelo ha sido implementado desde cero en Python, permitiendo un análisis detallado de su comportamiento en un corpus de texto en español. Los temas cubiertos incluyen:

- Modelos de n-gramas y suavizado (Laplace, Add-k, Good-Turing)
- Técnicas de agrupamiento (Brown Clustering)
- Reducción de dimensionalidad (LSA)
- Modelos de word embeddings (Word2Vec y GloVe)

## Modelos Implementados
1. Modelos de N-gramas
Suavizado de Laplace y Add-k: Se implementaron modelos bigrama con suavizado Laplace y Add-k, ajustando la probabilidad para manejar palabras no vistas.
Suavizado Good-Turing: Implementación de Good-Turing para ajustar la probabilidad de palabras poco frecuentes o no vistas. Se incluye una estimación para N5 en caso de que ciertos valores de frecuencia estén ausentes.
2. Clustering de Brown
Se implementó el algoritmo de Brown Clustering para agrupar palabras en función de su contexto en el corpus. Este método permite descubrir relaciones entre palabras según sus patrones de coocurrencia.

3. Análisis Semántico Latente (LSA)
Se construyó una matriz de términos-documentos utilizando TF-IDF y se aplicó SVD para reducir la dimensionalidad, obteniendo una representación en un espacio semántico reducido.

4. Word Embeddings
Word2Vec (CBOW y Skip-Gram): Implementación de Word2Vec utilizando las arquitecturas CBOW y Skip-Gram con muestreo negativo.
GloVe: Implementación de GloVe con una matriz de coocurrencia, optimizando la función de costo para aprender representaciones de palabras.

## Análisis y Resultados
Cada modelo se evaluó y analizó de acuerdo con su capacidad para capturar relaciones entre palabras y mejorar la representatividad semántica. Los resultados muestran cómo las técnicas de suavizado y las arquitecturas avanzadas como Word2Vec y GloVe logran diferentes niveles de precisión en la estimación de la probabilidad de palabras o en la creación de embeddings efectivos.
Los resultados más significativos de los modelos y técnicas están documentados en el notebook Examen_Parcial_NLP.ipynb.

Referencias
Jurafsky, D., & Martin, J. H. (2009). Speech and Language Processing. Pearson.
Mikolov, T., et al. (2013). Efficient Estimation of Word Representations in Vector Space. arXiv preprint arXiv:1301.3781.
Pennington, J., Socher, R., & Manning, C. D. (2014). GloVe: Global Vectors for Word Representation. EMNLP.
Suavizado Add-one: https://github.com/kapumota/Actividades-CC0C2/blob/main/Cuadernos-CC0C2/Clase2/Modelos-lenguaje1.ipynb
Suavizado Add-k: https://github.com/kapumota/Actividades-CC0C2/blob/main/Cuadernos-CC0C2/Clase2/Modelos-lenguaje2.ipynb
Suavizado Backoff:  https://github.com/kapumota/Actividades-CC0C2/blob/main/Cuadernos-CC0C2/Clase2/Counts-backoff-suavizado.ipynb
Suaviado Stupid Backoff: https://github.com/kapumota/Actividades-CC0C2/blob/main/Cuadernos-CC0C2/Clase2/Topicos-avanzados.ipynb
Glove y word2vec: https://github.com/kapumota/Actividades-CC0C2/blob/main/Cuadernos-CC0C2/Clase4/Embeddings.ipynb
Repositorio de mi resolucion de la PC1: https://github.com/Kinartb/CC0C2/blob/main/PC1/pc1_nlp.py
