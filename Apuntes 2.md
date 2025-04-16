# Apuntes Dinamica de Sistemas 2 Corte 
### Rincon Benavides Juan Esteban 
## Correccion primer parcial---19/03/2025
## Punto 1
Para el primer punto del parcial nos presenta la siguiente ecuación la cual deberemos solucionar según las condiciones iniciales determinadas en este mismo 

$$2\ddot{x} + 2\dot{x} + x = 1$$

$$X(0) = 0, \quad \dot{X}(0) = 2$$

Una vez con esto pasaremos a la solución del primer punto del parcial teniendo en cuenta los temas vistos en el corte quedando de la siguiente forma

$$-s^2 X(s) + sX(0) - \dot{X}(0) + [sX(s) - X(0)] + X(s) = \frac{1}{2s}$$

$$-s^2 X(s) - 2 + sX(s) + X(s) = \frac{1}{2s}$$

$$X(s)(s^2 + s + \frac{1}{2}) = \frac{1}{2s} + 2$$

$$X(s) = \frac{4s + 1}{(s^2 + s + \frac{1}{2})2s}$$

$$\frac{4s + 1}{(s^2 + s + \frac{1}{2})2s} = \frac{A}{2s} + \frac{B s + C}{s^2 + s + \frac{1}{2}}$$

$$4s + 1 = A(s^2 + s + \frac{1}{2}) + (Bs + C)(2s)$$

$$4s + 1 = A s^2 + A s + \frac{A}{2} + 2 B s^2 + 2 C s$$

$$4s + 1 = (A + 2B)s^2 + (A + 2C)s + \frac{A}{2}$$

Una vez con esto podemos hallar las ecuaciones correspondientes con esto podremos encontrar los valores de A B Y C teniendo las siguientes ecuaciones

$$\frac{A}{2} = 1$$

$$A + 2C = 4$$

$$A + 2B = 0$$

Una vez con este sistema de ecuaciones pasaremos a resolver las incógnitas teniendo como resultado lo siguiente para A:

$$A = 2$$

Sustituyendo A en la tercera ecuacion tendremos que el resultado de B es:

$$A + 2B = 0$$

$$B = -1$$

Una vez con lo siguiente podremos reemplazar en la segunda ecuación A también para así poder hallar el resultado de C

$$A + 2C = 4$$

$$2 + 2C = 4$$

$$C = \frac{4 - 2}{2}$$

$$C = 1$$

Una vez teniendo esto podremos reemplazar los valores de A B y C en la ecuación de fracciones parciales esto para dar fin al ejercicio y poder hallar la transformada inversa del mismo

$$\frac{2}{2s} + \frac{-s + 1}{s^2 + s + \frac{1}{2}}$$

$$\mathcal{L}^{-1} \left( \frac{-s + 1}{s^2 + s + \frac{1}{2}} \right)$$

$$s^2 + s + \frac{1}{2} = \left(s + \frac{1}{2}\right)^2 + \frac{3}{4}$$

$$x(t) = 2 + e^{-\frac{1}{2}t} \left( \cos\left( \frac{\sqrt{3}}{2}t \right) - \sqrt{3} \sin\left( \frac{\sqrt{3}}{2}t \right) \right)$$

## Punto 2
Para el segundo punto del ejercicio del parcial deberemos hallar $f(s)$ la ecuación correspondiente es

$$F(s) = \frac{6s}{\left(s - \frac{5}{2}\right)\left(s^2 - 4s + 8\right)}$$

Una vez tengamos la ecuacion pasaremos a resolver el ejercicio este lo resolveremos por fracciones parcciales teniendo lo siguiente

$$\frac{6s}{\left(s - \frac{5}{2}\right)\left(s^2 - 4s + 8\right)} = \frac{A}{s - \frac{5}{2}} + \frac{Bs + C}{s^2 - 4s + 8}$$

$$6s = A(s^2 - 4s + 8) + (Bs + C)\left(s - \frac{5}{2}\right)$$

$$6s = As^2 - 4As + 8A + Bs^2 - \frac{5}{2}Bs + Cs - \frac{5}{2}C$$

$$6s = s^2(A + B) + s(-4A + C - \frac{5}{2}B) + (8A - \frac{5}{2}C)$$

Al haber hecho el despeje por medio de fracciones parciales podemos asignar el siguiente sistema de ecuaciones esto con el fin de hallar las incógnitas de A B y C

$$A + B = 0$$

$$-4A + C - \frac{5}{2}B = 6$$

$$8A - \frac{5}{2}C = 0$$

Empesaremos hallando C y B en terminos de A

$$8A - \frac{5}{2}C = 0$$

$$C = \frac{2(8A)}{5}$$

$$C = \frac{16A}{5}$$

y para B 

$$A + B = 0$$

$$B = -A$$

una vez teniendo C y B en terminos de A remplazaremos en la segunda ecuacion para hallar A

$$-4A + C - \frac{5}{2}B = 6$$

$$\frac{-4A + 16A'}{5} - \frac{5(-A)}{2} = 6$$

$$\frac{-4A + 16A}{5} + \frac{5A}{2} = 6
\quad \text{(Multiplicamos por 10)}$$

$$-40A + 32A + 25A = 60$$

$$17A = 60$$

$$A = \frac{60}{17}$$

Teniendo A ya podremos hallar B y C teniendo que para B es 

$$B = -A$$

$$B = -\frac{60}{17}$$

y para C tenemos que 

$$C = \frac{16A}{5}$$

$$C = \frac{16}{5} \cdot \frac{60}{17}$$

$$C = \frac{192}{17}$$

Una vez hayas las incógnitas podremos reemplazarlas en las fracciones parciales teniendo como resultado lo siguiente este resultado es al que le ha realizaremos la transformada inversa de Laplace

$$\frac{\frac{60}{17}}{5 - \frac{5}{2}} + \frac{-\frac{60}{17}s + \frac{192}{17}}{s^2 - 4s + 8}$$

Teniendo como resultado en la transformada lo sigiente 

$$f(s) = \frac{24}{17} \delta(t) + \frac{1}{17} \left[ -60 e^{2t} \cos(2t) + 72 e^{2t} \sin(2t) \right]$$

# Sistemas Mecanicos 
### 26/03/2025
## Principio general de modelamiento

[![image.png](https://i.postimg.cc/52XKQWgv/image.png)](https://postimg.cc/87Vmx3qP)

Para el modelamiento de sistemas mecánicos veremos que está representado por varios, como mecánico eléctrico hidráulico térmico y combinaciones de estos mismos cómo matemáticamente están representados estos sistemas para darnos una idea de su funcionamiento
Estos sistemas tienen una cierta cantidad de elementos característicos los cuales se representan cada uno con su ecuación y un funcionamiento específico Como lo son los siguientes para un sistema mecánico más amortiguador

## Resorte
Como bien su nombre indica este es un elemento resortado la cual se considera para beneficio de los cálculos resortes lineales la cual la fuerza externa aplicada y el desplazamiento están relacionados por una constante de proporcionalidad dicha constante dependerá siempre del ejercicio, su representación gráfica y ecuación es la siguiente

[![image.png](https://i.postimg.cc/P51ZR6r9/image.png)](https://postimg.cc/PCrPLQDQ)

## Amortiguador 
Este es un elemento mecanico el cual nos ayuda en los sistemas a dicipar energia por medio de calor su funcionamiento es lineal segun la velocidad de desplazamiento que genere puede ser usadado tambien oara representar la friccion entre una masa y una superficie, al analizarlo de una forma limeal nos ayuda a entender mejor su funcicionamiento y a representarlo mejor matematicamente, su representacion grafica y modelamiento es el siguiente

[![Screenshot-2025-04-09-17-02-51-473-com-microsoft-teams-edit.jpg](https://i.postimg.cc/T1MwLmYL/Screenshot-2025-04-09-17-02-51-473-com-microsoft-teams-edit.jpg)](https://postimg.cc/9RbVsD9C)

## Tipos de friccion
Existen tres tipos de friccion en estos sistemas los cuales serian la friccion estatica, friccion por deslizamiento y friccion por rozamiento cabe a clarar que estos tres tipos de friccion se dan cuando ninguna de las superficies estan lunricadas 

[![IMG-20250409-172155.jpg](https://i.postimg.cc/k5GyMV4P/IMG-20250409-172155.jpg)](https://postimg.cc/8F8vtzMZ)

En el caso del rozamiento por rodamiento veremos que la furza las cuales tendremos en nuestro sistema son torques y pares por ser circular el elementos una de las circunstancias que tendremos es que tendra un par de fricción muy pequeño a si como se ve en la imaguen

[![Screenshot-2025-04-09-17-25-24-871-com-microsoft-teams-edit.jpg](https://i.postimg.cc/VNJjQ3GY/Screenshot-2025-04-09-17-25-24-871-com-microsoft-teams-edit.jpg)](https://postimg.cc/mcGc76Wq)

## Sistema masa-resorte-amortiguador 
Este es uno de los sistemas mas censillos que se pueden dar, variara su dificultad segun la cantidad de elementos a analizar,para el análisis y solución de estos sistemas debemos tener en cuenta el fenómeno físico que modela el sistema en general nos basamos en 3 leyes

[![image.png](https://i.postimg.cc/hjX8h3zc/image.png)](https://postimg.cc/62N4mcfm)

Estas nos ayudarán a analizar y resolver el sistema estos sistemas masa resorte amortiguador pueden verse de la siguiente manera

[![image.png](https://i.postimg.cc/CKLspKwZ/image.png)](https://postimg.cc/YvZW1MGk)

Teniendo una vez el sistema podremos dar solución a este ejemplo sabiendo que para el análisis del mismo deberemos solucionar el diagrama de cuerpo libre correspondiente teniendo en cuenta para qué direcciones van las fuerzas y asumiendo el signo para cada una de ellas, teniendo como solución el siguiente diagrama de bloques

[![image.png](https://i.postimg.cc/bNc0Ngzf/image.png)](https://postimg.cc/Th05trLt) 

Una vez hecho el diagrama de bloques sólo nos queda plantear las ecuaciones del sistema para ello utilizaremos la ley de sumatorias de kirchhoff teniendo en cuenta que todas las fuerzas tienen que ser iguales a la masa por aceleración

$$u - F_R - F_F = m \cdot a$$

$$F_R = k_2 \cdot y(t)$$

$$u(t) - k_2 \cdot y(t) - F_F = m \cdot a$$

$$F_F = k_1 \cdot \frac{dy(t)}{dt}$$

$$u(t) - k_2 \cdot y(t) - k_1 \cdot \frac{dy(t)}{dt} = m \cdot a$$

$$a = \frac{d^2 y(t)}{dt^2}$$

$$u(t) - k_2 \cdot y(t) - k_1 \cdot \frac{dy(t)}{dt} = m \cdot \frac{d^2 y(t)}{dt^2}$$

Un ejemplo más complicado podría ser el que analizaremos a continuación este ejemplo simula una rueda que está enganchada a una masa junto con un amortiguador y un resorte como una especie de automóvil para ello el diagrama general que nos dan es el siguiente.

[![image.png](https://i.postimg.cc/W4cgs6gf/image.png)](https://postimg.cc/qNQzLKm8)

Para el análisis del ejercicio veremos que es un ejercicio el cual las fuerzas aplicadas están en el eje y por lo cual tendremos que analizar la fuerza  de peso ya que influye en el sistema, a continuación el diagrama de cuerpo libre queda de la siguiente forma.

[![image.png](https://i.postimg.cc/QxnqZTfR/image.png)](https://postimg.cc/9rZ9Gr5p)

una vez con esto el procedimiento es muy similar a la anterior pues debemos garantizar que la sumatoria de fuerzas sea igual a masa por aceleración teniendo el siguiente resultado

$$\sum F = m a$$

$$U - k_2 - k_1 + W + mg = m a$$

$$U(t) - k_2 y(t) - k_1 \frac{dy(t)}{dt} + mg = m \frac{d^2 y(t)}{dt^2}$$

Habiendo analizado 2 sistemas podremos dar paso a uno de los sistemas más complejos ya que en este caso dependeremos de 2 masas y multitud de elementos el diagrama correspondiente para este tipo de ejercicios es el siguiente

[![image.png](https://i.postimg.cc/sXQJXD1T/image.png)](https://postimg.cc/34hGfhXG)

Para el análisis de este sistema sigue los mismos pasos que los anteriores pues necesitaremos analizar el diagrama de cuerpo libre para así ver dónde están actuando las fuerzas correspondientes de cada elemento esto será individual para cada una de las masas teniendo 2 diagramas de cuerpo libre
### Para la masa 1
[![image.png](https://i.postimg.cc/vTW8Gfyb/image.png)](https://postimg.cc/Lg8FTqhb)

Una vez en el diagrama de cuerpo libre correspondiente de igual manera analizaremos que la sumatoria de fuerzas sean igual a la masa por la aceleración de esa masa 1, en estos sistemas cuyas masas están entrelazadas por un resorte o un amortiguador se debe tener en cuenta que la distancia de elongación del resorte depende del movimiento de ambas masas asimismo la velocidad del émbolo del amortiguador depende del movimiento de ambas más para facilitar y analizar los cálculos teniendo como resultado lo siguiente

$$u - F_{R1} - F_{R2} - F_F = m_1 \cdot a_{m1}$$

$$u(t) - k_1 \cdot x_1(t) - k_2 \cdot (x_1(t) - x_2(t)) - b \cdot \frac{d(x_1(t) - x_2(t))}{dt} = m_1 \cdot \frac{d^2 x_1(t)}{dt^2}$$

## Para la masa 2
[![image.png](https://i.postimg.cc/Kv67qyqT/image.png)](https://postimg.cc/hf07vNq4)

De igual manera que para la masa número uno tendremos que analizar y dar sentido al diagrama de cuerpo libre teniendo en cuenta las mismas recomendaciones dichas para el sistema de la masa número uno, sabiendo que la distancia de obligación de cada uno de los resortes o émbolos de amortiguador van a depender de ambas masas teniendo como consecuente lo siguiente.

$$F_{R2} + F_F - F_{R3} = m_2 \cdot a_{m2}$$

$$k_2 \cdot (x_1(t) - x_2(t)) + b \cdot \frac{d(x_1(t) - x_2(t))}{dt} - k_3 \cdot x_2(t) = m_2 \cdot \frac{d^2 x_2(t)}{dt^2}$$

# Sistemas rotacionales 
### 2/04/2025
Los sistemas rotacionales son un tipo de sistema dinámico el cual el movimiento se describe en términos de rotación alrededor de un eje honesto con diferencia a los sistemas traslacionales los cuales siempre se mueven en línea recta sea en el eje x o en el eje y, hoy los sistemas rotacionales implican variables angulares y torques estos sistemas son fundamentales en el estudio de dinámica de cuerpos rígidos de igual forma que en los sistemas traslacionales se aplican leyes comparables a la del movimiento lineal las cuales son

[![image.png](https://i.postimg.cc/wTJ8Kpzz/image.png)](https://postimg.cc/8j1nWxsX)

Una representación gráfica de estos sistemas sería la siguiente, igual que en los sistemas traslacionales los pasos de solución de estos ejercicios serán muy parecidos teniendo en cuenta que sí o sí necesitaremos analizar y hacer un diagrama de cuerpo libre hola teniendo que la solución para este ejercicio es la siguiente.

[![image.png](https://i.postimg.cc/P5h7BvKb/image.png)](https://postimg.cc/xcxgmCwq)

[![image.png](https://i.postimg.cc/xjzF834y/image.png)](https://postimg.cc/Wts7fgjh)

$$T - F_R - F_F = J \cdot \alpha \quad \rightarrow \quad \alpha \text{ aceleración angular}$$

$$T(t) - F_F = J \cdot \alpha \quad \rightarrow \quad \alpha \text{ aceleración angular}$$

$$T(t) - k \cdot \theta(t) - b \cdot \frac{d\theta(t)}{dt} = J \cdot \frac{d^2 \theta(t)}{dt^2}$$

## Trabajo, Energía y Potencia 
El trabajo en este caso es una medida de la energía transferida a un objeto cuando una fuerza se aplica a lo largo de un desplazamiento esta fuerza es constante, en otras es una medida de la realización del esfuerzo a continuación veremos la fórmula general para hallarla, la energía puede dividirse en 2, energía potencial, energía cinética.

[![image.png](https://i.postimg.cc/FK7ncYv0/image.png)](https://postimg.cc/gwbDbkn0)
### Energía Potencial 
Esta energía consiste más que todo en que en sistemas mecánicos la energía potencial cambia de acuerdo a su posición esto con respecto a una referencia está además de eso en los sistemas mecánicos veremos que los resortes y las masas son los encargados de almacenar energía potencial esta es equivalente al trabajo realizado por la fuerza externa para poder hallar matemáticamente se utiliza una integral definida teniendo así lo siguiente

[![image.png](https://i.postimg.cc/FKMGLGDQ/image.png)](https://postimg.cc/hJ09FLkC)

### Energía Cinética 
Para este caso la energía cinética es debido a la velocidad que genera cada sistema dinámico solamente los elementos de inercia pueden almacenar energía cinética un ejemplo de ellos puede ser el cambio en la energía cinética es el trabajo realizado sobre una masa por la aplicación de una fuerza que acelera o desacelera 

[![image.png](https://i.postimg.cc/bvymPL3y/image.png)](https://postimg.cc/RWY7Q7ky)

## Potencia 
Podemos definir la potencia en un sistema mecánico como la velocidad a la cual se realiza cierto trabajo o transferencia de energía esto puede estar asociado al movimiento lineal o rotacional en el caso de sistemas lineales tenemos que

$$P = \frac{dW}{dt} = \vec{F} \cdot \vec{v}$$

donde:
- \( W \) es el trabajo,  
- \( \vec{F} \) es la fuerza aplicada,  
- \( \vec{v} \) es la velocidad del objeto.




