##Pruebas Unitarias (Unit Testing)

En programación, una prueba unitaria es una forma de probar el correcto
funcionamiento de un módulo de código.

El pensamiento detrás de las pruebas unitarias es, que si se prueba como
debería funcionar cada módulo/segmento/función de forma atómica y aislada,
entonces el sistema como un conjunto debería funcionar correctamente.

[Fuente: Wikipedia](http://es.wikipedia.org/wiki/Prueba_unitaria)

###Test-Driven-Development (TDD)
TDD es un tema complejo y difícil de aproximar a primera vista. El primer enlace
en la lista es un demo en vivo de Brad Wilson y Rob Connery y es excelente para
entender como la metodología funciona.

TDD funciona bajo un ciclo de trabajo llamado "Red-Green-Refactor": Se escribe una prueba para que falle,
luego se escribe el código para hacer que la prueba pase, y finalmente se hace refactor del código y se
usa la prueba para verificar que todo esté bien.

Más información en estos dos blog posts:
- http://www.jamesshore.com/Blog/Red-Green-Refactor.html
- http://stackoverflow.com/questions/5750366/red-green-refactor-why-refactor

Algunos recursos formales:
* [Brad Wilson: Play by Play TDD](http://pluralsight.com/training/courses/TableOfContents?courseName=play-by-play-wilson-tdd) (Pluralsight) :star: :moneybag:
* [Test-Driven Development, Kent Beck](http://amzn.com/0321146530) (Amazon):moneybag:
* [Ian Cooper: TDD, where did it all go wrong](http://vimeo.com/68375232)?


###Behaviour-Drive-Development (BDD)
BDD es un proceso de desarrollo de software basado en Test-Drive-Development que combina
aspectos de TDD, Domain-Driven Design y Diseño orientado a objetos para proveer a
desarrolladores de software y analistas de negocios con herramientas compartidas
para definir el comportamiento de sistemas.

La metodología es una aproximación que busca unificar el lenguaje descriptivo
de los requerimientos de una aplicaicón con la definición técnica de pruebas unitarias
que prueban el código.

[Fuente: Wikipedia](http://en.wikipedia.org/wiki/Behavior-driven_development)

####Cucumber
[Cucumber](http://cukes.info/)  Es una herramienta que facilita
la escritura de pruebas unitarias en texto puro que es legible para cualquier persona
sin conocimiento técnico. Utiliza un [Lenguaje de Dominio](http://martinfowler.com/books/dsl.html)
llamado [Gherkin](https://github.com/cucumber/cucumber/wiki/Gherkin) que traduce
requerimientos de negocios a unit tests usando expresiones regulares.

Existen implementaciones de Cucumber para más de 40 lenguajes. Aquí algunos:
* Java https://github.com/cucumber/cucumber-jvm
* Javascript https://github.com/cucumber/cucumber-js
* .NET http://specflow.org
* Ruby http://cukes.info/
* Python http://pythonhosted.org/lettuce/
