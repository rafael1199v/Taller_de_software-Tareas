# Resumen Lectura _Software Engineering at Google_
### Nombre: Rafael Andres Vargas Mamani

## Capitulo 1. _Qué es Ingeniería de software?_
Existen muchas diferencias entre la programación y la Ingeniería de Software. Algunas de las diferencias mas importantes son:
* Tiempo
* Escalabilidad
* Trade-offs (Compensaciones a cambio del sacrificio de otra)
* Personas

Un ingeniero de software tiene que ver mas allá del futuro cercano. Tiene que preocuparse por las acciones de mantener un proyecto a lo largo del tiempo, reduciendo los costos a largo plazo y estar mas pendiente al cambio eventual de las cosas.

La ingeniería de software involucra a una gran cantidad de personas en un proyecto donde se necesita un buen trabajo en equipo, mientras la programación es acto de creación individual.

### Tiempo y cambio
Cuando uno no tiene mucha experiencia, el lapso de vida es medido en horas o días. Los programas no tiene una refactorización ni un mantenimiento a largo plazo.


![Img tiempo y costo](https://www.oreilly.com/api/v2/epubs/9781492082781/files/assets/seag_0101.png)


### La ley de Hyrum
Esta ley basicamente indica que:
> Con una gran cantidad de usuarios, no importa lo que prometas en el contrato: Todos los comportamientos observables en tu sistema serán dependidos de otra persona.

![Img Comic](https://imgs.xkcd.com/comics/workflow_2x.png)


### Es necesario el cambio?
Para la mayoría de los proyectos a largo plazo, tienen que estar abiertos al cambio. Incluso si estuvieras haciendo una aplicación con una tecnología que provee un soporte a largo plazo, tienes que tener en cuenta los avances en el hardware, en la seguridad y en las nuevas innovaciones de la humanidad. Nunca puedes quedarte sin adaptarte al cambio.

### Políticas
* **No escalables**  
    _La cantidad de trabajo debería crecer a la par de la organización?_  
    Estas políticas son identificadas cuando la organización escala de 10 a 100 veces su tamaño.
    - La enfoque de una deprecación sufre cuando el proyecto tiene una gran cantidad de usuarios donde cualquier cambio que parezca insignificante sea un dolor de cabeza para muchos usuarios.
    - El uso de las ramas de desarrollo es otra política que tiene problemas de escalado.
      En grandes organizaciones, cuando se completa una rama de desarrollo se tiene que probar y unir con las demás. Aumentando un esfuerzo de trabajo al sincronizar y probar todas las ramas unidas. 
 
* **Escalables**
    - __Beyonce Rule__ 
      _"If you like it you should have [test, lint, e2e, ticket] on it!"_  
      Esta política aplicado a las pruebas en el sistema de continua integración hace que se modifique o se añada mas convenciones y procesos. La Regla de Beyonce es rentable y de adoptar fácilmente. 

### Shifting Left
Este termino indica que considerando la linea de tiempo del flujo de trabajo de los desarrolladores, cuando mas a la izquierda se detecte un problema, entonces se es fácil y barato de arreglar.

![Img Shifting Left](https://www.oreilly.com/api/v2/epubs/9781492082781/files/assets/seag_0102.png)

### Compensaciones y costos
El costo no solo se refiere a los dolares o cualquier otra moneda. Los costos abarcan:
- Costos financieros (dinero)
- Costos de recursos (Uso de CPU)
- Costos transacionales (¿Que cuesta tomar esa acción?)
- Costos de oportunidad (¿Que es lo que cuesta no tomar esa acción?)
- Costos sociales (¿Que impacto tendrá esta elección en nuestra sociedad en general?)

Muchas de estas decisiones no se pueden medir y solo se pueden basar en la experiencia. Sin embargo, incluso cuando existen muchas formas de tener métricas para tomar las mejores decisiones, los datos están en constante cambio y pueden hacer que tomemos malas decisiones a lo largo de nuestra vida.

> **Tip:** Recuerda que es mejor admitir tus equivocaciones. Los lideres que admiten sus errores son mas respetados.

### Ingeniería de software vs Programación
Al final de toda esta reflexión, ¿La ingeniería de software es mejor que la programación?.
La respuesta es **No**. En realidad estos dos enfoques tienen diferentes dominios de las cuales algunas herramientas pueden ayudar al otro, pero no significa que uno sea mejor que otro.
La programación es el arte de producir código, mientras que la ingeniería de software es un conjunto de políticas, prácticas y herramientas necesarias para que el código sea útil durante el tiempo que sea necesario.   
