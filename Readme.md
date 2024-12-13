# Examen 1ª Evaluación

---
>3er intento(la 3era va la vencida)

Explica a continación cada apartado del examen

Con cada apartado realiza un commit diferente

---

## diagrama de flujo

![/home/dam/COD/diagrama.jpg](https://cdn.discordapp.com/attachments/926647859259011124/1317046413917683723/rn_image_picker_lib_temp_49f385e4-9431-457f-8173-934a6997d07f.jpg?ex=675d428e&is=675bf10e&hm=973daf7d24d8bd08cf0320055899ddb608d13dd91b77b67fd5e0ae1c28e25325&)

- mediante `2` bucles recorremos el array, las longitudes de os bucles son las del array `8` valores, de `0` al `7`
- en el tablero las casillas vacias valen `0`, las blancas `1` y las negras `2`
- compara cada casilla con el valor `1` y `2`, para saber si hay una ficha
- si hay una ficha muestra por pantalla donde con `tablero[i][j]` y suma `1` al `contador de las fichas`
- cuando termina el bucle resta el contador de las blancas al de las negras, por lo tanto si habia `mas blancas` el valor será `negativo`
- no puse caso de empate, para eso tendriamos que poner anteriormente un `if` con `contador_negra==0`

---

## tablero

int[][] matriz = {

{1, 0, 1, 0, 1, 0, 1, 0},

{0, 1, 0, 1, 0, 1, 0, 1},

{1, 0, 1, 0, 1, 0, 1, 0},

{0, 0, 0, 0, 0, 0, 0, 0},

{0, 0, 0, 0, 0, 0, 0, 0},

{0, 2, 0, 2, 0, 2, 0, 2},

{2, 0, 2, 0, 2, 0, 2, 0},

{0, 2, 0, 2, 0, 2, 0, 2},

};

---
## 3 funciones

1. En el bucle podriamos hacer una funcion llamada recorrerTableroNegras, donde devolveríamos el contador de las negras
2. En el mismo bucle haríamos una funcion igual pero con las blancas
3. por ultimo podriamos hacer una nueva funcion llamada ganador que sea la resta de turnos y la impresion por pantalla del ganador. seria un void

---
## Javadoc

/**
1.
* contaría la cantidad de fichas negras
* @param negras seria el contador de las fichas negras
* @param tablero es nuestro tablero para que lo vaya recorriendo
* @return devuelve la cantidad de fichas negras
  */

    public static int recorrerTableroNegras(int negras, int[][] tablero){}
  /**
2.
* es lo mismo que el de arriba pero con fichas blancas
* @param negras seria el contador de las fichas blancas
* @param tablero es nuestro tablero para que lo vaya recorriendo
* @return devuelve la cantidad de fichas blancas
  */

    public static int recorrerTableroBlancas(int blancas, int[][] tablero){}
/**
3.
* le damos estos 2 valores para que los compare y segun cual de ellos es mayor nos diga el ganador
* @param negras la cantidad de fichas negras
* @param blancas la cantidad de fichas blancas
  */

  public static void ganador(int negras, int blancas){}

>tuve que cambiar el programa a algo parecido ya que el mio tendría que **devolver varios valores o no se veian bien como se podrían meter 3 funciones**, así que lo que cambiaría de mi programa es **que haga 2 veces el bucle**, uno con las fichas negras y otro con las blancas con su respectivo contador, asi ya hice `2` funciones, la ultima sería la que nos dice quien gana con los parametros de los `2 `contadores comparándolos y viendo cual es el mayor. Si queremos que la ultima funcion nos devuelva un `valor` lo que tendriamos que hacer es al principio de todo crear una `variable` nueva llamada `ganador` y que entre tambien aqui como `parámetro` y sea lo que nos devuelva, segun el valor devuelto, `1` para las blancas y `2` para las negras, a partir de eso en el main con un `if else` pondremos el ganador.