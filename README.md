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
|   VTH(V)  |          |   RTH(Ω)  |             |
|:---------:|----------|:---------:|-------------|
| Calculado | 5.0556 V | Calculado | 298.855 ohm |
| Medido    | 5.06 V   | Medido    | 299 ohm     |
| Error %   | 0,8%     |   Error % | 0,48%       |


***Tabla 2. Comprobación del Teorema de Thévenin***
| Parámetro Eléctrico | Circuito Original |           |         | Circuito   Equivalente Th |        |         |
|:-------------------:|:-----------------:|:---------:|:-------:|:-------------------------:|:------:|:-------:|
|                     | calculado         | medido    | Error % | calculado                 | medido | Error % |
| Voltaje (V)         | 3.89 V            |  3.8926 V | 0,06%   | 3.88 V                    | 3.89V  | 0,25%   |
| Corriente (mA)      | 3.89 mA           | 3.8926 mA | 0,06%   | 3.88 mA                   | 3.89mA | 0,25%   |

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
