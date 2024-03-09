El código consta de dos secciones distintas.

La primera parte se centra en el análisis de señales EEG (Electroencefalografía) para eliminar segmentos similares entre diferentes electrodos. 
Comienza definiendo una función llamada eliminar_segmentos que realiza este proceso. Primero, identifica las marcas de tiempo idénticas entre los electrodos 
y obtiene los segmentos correspondientes a esas marcas. Luego, calcula la correlación de Pearson entre los segmentos de cada par de electrodos. Si la correlación 
es mayor o igual a 0.7, se conserva el segmento con mayor amplitud y se elimina el otro. Este proceso se realiza iterativamente para 
diferentes combinaciones de electrodos, optimizando así la eliminación de segmentos redundantes.

La segunda parte del código trabaja con matrices de datos y tiene como objetivo filtrar elementos no deseados de submatrices 3x3. Se definen las matrices originales 
y se extraen todas las posibles submatrices 3x3. Luego, se filtran los elementos no deseados de estas submatrices y se imprimen los resultados. Este proceso se repite 
para todas las submatrices.

En ambas secciones del código, se utiliza una estructura clara y ordenada, con comentarios explicativos y nombres de variables descriptivos para facilitar la comprensión 
y el mantenimiento del código.
