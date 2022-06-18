### 2) Dibujar un diagrama de flujo de datos que permita cargar y determinar e imprimir la posición del
último elemento negativo dentro de un vector X con datos numéricos enteros ingresados por el
usuario, con entre 8 y 40 elementos.

```mermaid
flowchart TD
	1(veces = 'Cuantos elementos desea ingresar?') --> 2{veces < 8? o veces > 40?}
    2 --> |Si| 1
    2 --> |No| 3{veces > 0?}
    3 --> |Si| 4(numero = 'Ingrese un número')
    4 --> 5(añadir 'numero' a la lista)
    5 --> 6{Si numero es negativo}
    6 --> |Si| 7(posicion_negativo = Obtener posicion)
    6 --> |No| 8
    7 --> 8(veces -= 1)
    8 --> 3
    3 --> |No| 9(print: 'posicion_negativo')
```
