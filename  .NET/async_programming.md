##Programación Asíncrona en el .NET Framework

Asynchronous programming es la habilidad que tiene un programa para no bloquear
el thread actual en el cual se está ejecutando la operación. Es un paradigma
muy común en frameworks como javascript, donde esto se logra usando callbacks.

En .NET esto se logra de esta forma:
* Se marca un método como `async` para que el compilador sepa que el método puede retornar sin haber terminado
* Se cambiar el return type del método para que retorne `Task<T>` siendo T lo que se quiere retornar
* Se ejecuta el método que se desea realizar asíncrono con el keyword `await`, lo que permite que en ese momento
el método "suelte el thread" hasta que la operación termine, y lo retome cuando esta haya concluído

El beneficio de usar métodos asíncronos es mejores tiempos de respuesta para
operaciones que requieren mucho tiempo (acceso a bases de datos, operaciones I/O,
  llamadas a servicios externos por HTTP, etc.) y un mejor [throughput](http://en.wikipedia.org/wiki/Throughput)
  o cantidad concurrente de requests de una aplicación.

####Algunos recursos

* [How to Build ASP.NET Web Applications Using Async - Channel 9](http://channel9.msdn.com/Events/TechEd/NorthAmerica/2013/DEV-B337#fbid=) :free:
* [The future of C# and VB.NET - Channel 9](http://channel9.msdn.com/events/PDC/PDC10/FT09/) Esta es con Anders Hejlsberg, el creador de C# :exclamation:
* [Asynchronous Programming with Async and Await - MSDN](http://msdn.microsoft.com/en-us/library/hh191443.aspx)
* [Asynchronous C#, by Jon Skeet - Pluralsight](http://pluralsight.com/training/Courses/TableOfContents/skeet-async) :moneybag:
