# Apuntes Dinamica de Sistemas 2 Corte 
### Rincon Benavides Juan Esteban 
## Correccion primer parcial
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
Este es uno de los sistemas mas censillos que se pueden dar variara su dificultad segun la cantidad de elementos a analizar









