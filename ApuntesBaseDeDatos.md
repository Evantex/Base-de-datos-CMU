# Apuntes base de datos 


## Modelado MER (modelo Entidad Relación) y MR (Modelo Relacional)

-   Cuando se representa una relación con una tabla de valores los distintos elementos estarán representados de la siguiente manera:
    -   La tabla representa al 'Tipo de Entidad': es como la plantilla o la Clase si hablaramos en términos de paradigma orientado a objetos.
    -   Cada fila de la tabla se denomina tupla y corresponde a una 'Entidad' real
    -   Cada columna representa un atributo de la Entidad y el tipo de dato de ese atributo está representado por un dominio de posibles valores para lo cual se especifica un tipo de dato o formato. **Un dominio cuenta con**:
        -   Un nombre
        -   Un tipo de dato
        -   Un formato
        -   Ejemplo: EdadesEmpleado (número entero comprendido entre 16 y 80)




-   El grado de una relación es el número de atributos de la misma.


### ¿Cúanto plantear un 'Tipo de Entidad' y cúando plantear un atributo de una entidad ya existente?
Según Chat GPT, podemos tener en cuenta ciertos criterios a la hora de evaluar la existencia o no de un tipo de entidad:

| Caso | Conviene usar atributo cuando... | Conviene usar entidad cuando... |
|--------|----------------------------------|---------------------------------|
|Identidad| El valor no necesita tener un identificador propio.| El concepto tiene una identidad independiente (por ejemplo, una comuna puede existir sin evento)
|Reutilización / relación|Solo lo usás dentro de una entidad (por ejemplo, “color” de un auto).|Puede estar relacionado con múltiples entidades o aparecer en varios contextos (por ejemplo, varios eventos pueden ocurrir en la misma comuna).
|Atributos propios|No tiene atributos adicionales.|Tiene uno o más atributos propios (por ejemplo, la comuna tiene nombre, código postal, etc.).
|Cardinalidad|Siempre es 1:1 y sin estructura interna.|Hay relaciones 1:N o N:N
|Volumen de datos|El valor se repite poco y no amerita una tabla propia.|Puede repetirse muchas veces y conviene normalizarlo.

---





