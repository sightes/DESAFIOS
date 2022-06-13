# DESAFIOS
Resolucion del desafio propuesto para spot2 detallado en https://github.com/sightes/DESAFIOS/blob/main/Data%20Challenge%202.0.pdf

Para visualizar y ejecutar el desafio https://colab.research.google.com/github/sightes/DESAFIOS/blob/main/Spot2.ipynb

LOS MAPAS INTERACTIVOS SOLO SON VISIBLES DESDE COLAB, NO SON VISIBLES DESDE GITHUB


# IMPORTANTE !

Las 2 primeras celdas, descargan directamente los datos desde https://www.inegi.org.mx/app/descarga/?ti=6 y consideran los topicos :

      - Comercio por menor 
      - Servicios de alojamiento temporal y de preparación de alimentos y bebidas
      
      
# Entorno de desarrollo

Se selecciono Google Colab , debido a que utiliza el proceso en la nube, requerimientos de desempeno, sin embargo , esto 
puede extenderse a alguna infrestructura mas sofisticada siempre cuando lo amerite

# Modo de ejecucion 

Ejecutar las celdas respectivas paso a paso 

# Como Funciona?

  - El algoritmo descarga los comercios registrados en formato CSV , luego se descomprimen y secuencialmente se exploca carpeta por carpeta, extrayendo y limpiando la data
   
  - Se trabaja sobre los nombres del comercio, buscando las palabras "pizza" o "pizzer"
  
  - luego se recorre la tabla solicitada por el cliente, la cual se contrasta con las pizzerias registradas los ultimos 3 anios, con esto se proyecta en un mapa ,
  para luego calcular las distancias en kilometros respecto a cada objetivo ( se valido contra google maps el funcionamiento de esta metrica)
  
  - Finalmente se genera un grafico de barras a fin de saber la distribucion en terminos de trabajadores de la competencia .

# Problemas conocidos 

a veces se confunde con la palabra pizzarro , pizzarrenio etc etc , en futuras versiones podria ser arreglado dicho bug

# to do 

-Generacion de reporte 
-Mejoras de rendimiento
-Arreglo de bugs 
-Optimizacion y seleccion de lugares en cercanias 


# Ejemplos 

Ejemplo muestra del mapa completo del pais con todas las pizzeria

  ![alt text](https://github.com/sightes/DESAFIOS/blob/main/mapa%20general.PNG?raw=true)
  
  
Es posible filtrar aquella competencia que se encuentra cerca de los objetivos 

  ![alt text](https://github.com/sightes/DESAFIOS/blob/main/personal%20cercanias.PNG?raw=true)
  
  
 O la cercania de uno solo 

  ![alt text](https://github.com/sightes/DESAFIOS/blob/main/personal%20suc.PNG?raw=true)

   
  
