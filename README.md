En esta práctica, programaremos un robot en real cuyo comportamiento será girarse al encontrarse con un obstáculo de color rojo y cuando no tenga uno delante, se moverá hacia delante con una velocidad lineal.

Para ello, primero aplicaremos un filtro para el color rojo de la imagen que nos proporciona el sensor, en este caso la cámara.
El comportamiento será tal que si el área filtrada de la imagen es cero, le ordenamos velocidad lineal hacia adelante y de giro cero al robot y si dicho área es distinto de cero, le ordenamos girar de forma estática durante un tiempo determinado almacenado en una variable y luego otra vez velocidad lineal hacia adelante.

Es básicamente un algoritmo de autómatas finitos, donde si estoy en un estado y se deja de cumplir una condición en este caso si hay área o no, transito a otro que seguir adelante o volver girar.
