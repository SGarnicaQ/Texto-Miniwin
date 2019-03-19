#Que es?

Es un pequeño fragmento de codigo el cual mejora un aspecto muy pobre de miniwin el cual es *el texto*, a partir del uso del llamado de una funcion se podra escribir texto en miniwin pero esta vez con un estilo diferente, pudiendo modificar el tamaño espaciado entre otros...

#Como usarlo

La funcion `d_text(int x, int y, const std::string& s, int xt, int yt, int esp, double deg, bool xMedio)` permite imprimir el texto a partir de los siguientes argumentos.

- `int x`: 
	posicion en x del texto.
- `int t`: 
	posicion en y del texto.
- `const std::string& s`: 
	string del texto a imprimir.
- `int xt`: 
	tamaño en x o width del texto.
- `int yt`: 
	tamaño en y o height del texto.
- `int esp`: 
	espaciado entre letra y letra (numero de pixeles que separan las letras).
- `double deg`: 
	degradado del tamaño de forma vertical de las letras. 
	el valor debe ser entre 0 y 1, donde 1 es la letra sin degradado y mientras mas se acerque al cero el degradado sera mayor.
- `bool xMedio`: 
	si es 0 la posicion x y del texto sera la esquina superior izquierda.si es 1 la posicion x y del texto sera el punto medio.

> Los caracteres que son permitidos para el d_text por el momento son las letras de la A a la Z y el espacio, aquellos caracteres como: la ñ y los numeros de 0 al 9, (',', '.', ':', ...) aun no son permitidos, tampoco los que son con tilde.

#Ejemplo

`d_text(vancho()/2,valto()/2,"hola mundo", 10, 10, 4, 1, 0)`