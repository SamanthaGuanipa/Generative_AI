# Generación de mi propio texto de Shakespeare

Se tiene una frase dada y se deberá predecir la siguiente palabra, la Red Neuronal Recurrente (RNN) tomará la primera palabra de la frase, esta será pasada por una red neuronal y predecirá la siguiente palabra. Sin embargo, para poder predecir la tercera palabra, toma la activación del estado oculto y la segunda palabra como entrada. El mismo proceso continúa y se capta la relación secuencial porque se utiliza el estado oculto de la palabra anterior para predecir la siguiente, lo que significa que de alguna manera se está utilizando una versión codificada de la frase anterior para predecir la palabra siguiente.

Existen estructuras más eficaces, como las unidades recurrentes controladas (GRU) y las de memoria a largo plazo (LSTM). El problema práctico de por qué se utilizan las GRU y las LSTM en lugar de las RNN es el siguiente: en las RNN, se utiliza la información de cada palabra anterior para predecir correctamente la palabra siguiente, pero a veces una parte de una frase es suficiente para predecir la palabra siguiente en las LSTM y las GRU.

Se utilizará esta idea para diseñar una red de forma que el modelo decida qué palabras seleccionar y escriba como Shakespeare.
