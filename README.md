# Santander - Clasificación de preguntas

Santander nos propone un desafío basado en NLP, donde lo que se busca es entender las preguntas que hacen los clientes con el fin de ser más asertivos en las respuestas, esto es fundamental para brindar una mejor experiencia al usuario.

Esta competencia tiene como objetivo desarrollar un algoritmo de clasificación que, utilizando técnicas de NLP (Natural Language Processing), sea capaz de entender la intención de un cliente (target) al momento de realizar una pregunta (predictor) en alguno de los canales del Banco.

### Datos

- training.csv: reúne la información del caso, el mismo tiene dos columnas
    - Pregunta: pregunta realizada por el cliente. (String)
    - Intención: intención de la pregunta realizada, contiene 350 intenciones aproximadamente. (String)

- test.csv: solo contiene la pregunta realizada por el cliente.

**Score de predicciones:** los resultados serán medidos utilizando la métrica Balance Accuracy.

### Solución

Utilicé los pesos del modelo [BETO](https://github.com/dccuchile/beto) (Bidirectional Encoder Representations from Transformers entrenado con textos en español) y luego entrené una última capa con los datos de entrenamiento.

![img](https://www.vproexpert.com/wp-content/uploads/2019/12/google-bert-745x342-1.png)


La librería con la que realicé el pre-procesado y la creación del modelo fué [transformers](https://github.com/huggingface/transformers)

El score alcanzado fue de: #####



### Fuentes
- [huggingface - transformers](https://huggingface.co/)
- [BERT Research Series](https://www.youtube.com/watch?v=FKlPCK1uFrc&list=PLam9sigHPGwOBuH4_4fr-XvDbe5uneaf6)
- [NLP Specialization](https://www.coursera.org/learn/attention-models-in-nlp)
- [TensorFlow documentation](https://www.tensorflow.org/api_docs/python/tf/all_symbols)
- [Preprocessing for BERT](https://www.youtube.com/watch?v=Osj0Z6rwJB4)
- [Sentiment analysis with BERT](https://www.youtube.com/watch?v=8N-nM3QW7O0&t=2699s)
- [Illustrated BERT](https://jalammar.github.io/illustrated-bert/)
- [Primer puesto](https://github.com/frandorr/santander-question-classifier) , [segundo puesto](https://github.com/jeffersonlicet/santander-questions-classification) 

