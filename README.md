## UNIVERSIDAD DE LAS FUERZAS ARMADAS ESPE
![](https://github.com/erickfi/Practica-5/blob/master/Img/Escudo.jpg)
### Práctica de laboratorio N° 6
## Teorema de la Máxima Transferencia de Potencia
**Autores:** Figueroa Erick, León Jipshon,Viracucha William.
### 1. PLANTEAMIENTO DEL PROBLEMA
Al momento de diseñar un circuito eléctrico, por lo general, se busca que el circuito cumpla su trabajo, es decir, que los elementos electrónicos del mismo realicen el trabajo, pero no se toma en cuenta la eficacia para realizar este trabajo, recordando que la potencia representa la tasa de la energía que se convierte en trabajo, existen circuitos que buscan precisamente este objetivo, entregar la máxima potencia de tal forma que el trabajo se realice de ser posible sin pérdida de energía.

Por otro lado, para conocer la potencia que entrega un circuito es necesario analizar todos los componentes del mismo, aunque este proceso se puede simplificar si usamos el [Teorema de Thévenin](https://github.com/erickfi/Practica-5), de esta forma simplificamos el circuito y obtenemos un circuito simplificado para carga variable, su aplicación en la ingeniería es fundamental, ya que es importante en los procesos de automatización donde se busca que las máquinas funcionen a su máxima capacidad, es decir, que tengan una máxima potencia.


### 2. OBJETIVOS
#### Objetivo General
- Comprobar experimentalmente el Teorema de la Máxima Transferencia
#### Objetivos Específicos
- Calcular y comparar los valores de un circuito de Thévenin de forma analítica y experimental.
- Aplicar las *Leyes de Kirchhoff* y el *Teorema de superposición* para analizar y reducir un circuito a un circuito de Thévenin.
### 3. MARCO TEÓRICO
El **Teorema de la Máxima Transferencia de Potencia** estable:
> "La máxima potencia se transfiere a la carga cuando la resistencia de la carga es igual a la resistencia de Thévenin vista desde la carga (RL=RTh).

Es por esto que la forma más fácil de analizar la potencia suministrada a una carga es simplificando un circuito de dos terminales a un circuito de Thévenin.

![](https://github.com/erickfi/Practica-5/blob/master/Img/Cambio%20circuito.PNG)

Si graficamos la potencia suministrada en función de la variación de la carga obtenemos un gráfica similara a una camapana de Gauss.

![](https://github.com/erickfi/Laboratorio-6/blob/master/Img/Grafica.PNG)

En la cuál podemos observar que el punto más alto de transferencia es alcanzado cuando RL=RTh, si esto ocurre la potencia máxima se puede calcular como:

![](https://github.com/erickfi/Laboratorio-6/blob/master/Img/Con%20RTH.PNG)

Sin embargo, en los circuitos que se realizan en la vida real es poco probable que esto sucede, por lo general la resistencia que presenta la carga (RL) es diferente a la resistencia de la fuente (RTh), es por ello que para calcular la potencia se utiliza:

![](https://github.com/erickfi/Laboratorio-6/blob/master/Img/Con%20RL.PNG)

Ya que RL y RTh no son iguales no se puede alcanzar una _transferencia máxima de potencial ideal,_ pero este valor se puede aproximar variando la resistencia de la carga hasta que sea similar a la resistencia de la fuente pero sin que el funcionamiento del resto de elementos del circuito se vea afectado.


### 4. DIAGRAMAS
**Diagrama del circuito**

![](https://github.com/erickfi/Laboratorio-6/blob/master/Img/Diagrama.PNG)

**Medición de valores**

![](https://github.com/erickfi/Laboratorio-6/blob/master/Img/Thinker%206.1.PNG)
![](https://github.com/erickfi/Laboratorio-6/blob/master/Img/Thinker%206.2.PNG)
![](https://github.com/erickfi/Laboratorio-6/blob/master/Img/Thinker%206.3.PNG)

### 5. LISTA DE COMPONENTES

![](https://github.com/erickfi/Laboratorio-6/blob/master/Img/Materiales.PNG)

### 6. TABLA DE RESULTADOS

***Tabla 1. Valores del Circuito equivalente de Thévenin***

|   RL (Ω)  | Corriente  |   Voltaje  | Potencia calculada | Potencia calculada |
|:---------:|:----------:|:----------:|:------------------:|:------------------:|
|           |  Medida    |   medido   | Experimentalmente  | teóricamente       |
|           |   (mA)     |    (V)     |       (mW)         |        (mW)        |
|   220     |   10.6     |   2.32     | 24.592             | 24.548             | 
|   470     |   8.98     |   4.22     | 37.895             | 37.918             |
|   680     |   7.98     |   5.43     | 43.311             | 43.288             |
|   820     |   7.43     |   6.09     | 45.248             | 45.216             |
|   1000    |   6.82     |   6.82     | 46.512             | 46.487             |
|   1500    |   5.56     |   8.33     | 46.314             | 46.296             |
|   1800    |   5        |   9        | 45                 | 45                 |
|   2200    |   4.41     |   9.71     | 42.821             | 42.82              |
|   3900    |   2.94     |   11.5     | 33.81              | 33.737             |
|   4700    |   2.54     |   11.9     | 30.226             | 30.379             |



### 7. Explicación de Código Fuente

- 1. Arme el circuito tal como se encuentra en el diagrama.
- 2. Mida el voltaje y corriente de la resistencia 5.
- 3. Luego desconecte la resistencia 5 y mida el voltaje del circuito abierto 
- 4. Apague las fuentes y mida la resistencia en el circuito abierto
- 5. Arme el circuito equivalente de Thévenin agregándole la resistencia 5 en serie y configure la fuente y el potenciómetro con los valores del voltaje y resistencia medidos cuando el circuito estaba abierto, al final mida el voltaje e intensidad de corriente de la resistencia de 1kOhm la figura 

### 8. CONCLUSIONES



### 9. RECOMENDACIONES


### 10. CRONOGRAMA

![](https://github.com/erickfi/Laboratorio-6/blob/master/Img/Cronograma%206.PNG)

### 11. REFERENCIAS
- M. A. Sadiku.Fundamentos de circuitos eléctricos. Mc Graw Hill, third edition, 2006
### 12. ANEXOS
- [Cálculos análiticos](https://github.com/erickfi/Practica-5/blob/master/Anexos/C%C3%A1lculos%20Anal%C3%ADticos.pdf)
- [Cómo funciona el circuito](https://www.youtube.com/watch?v=TRDsxjXFfmg&feature=youtu.be)
- [Cómo se implementó el circuito](https://www.youtube.com/watch?v=GO8c0AroBgk&feature=youtu.be)
