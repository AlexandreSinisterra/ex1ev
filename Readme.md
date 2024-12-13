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