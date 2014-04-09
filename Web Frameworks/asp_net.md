##ASP.NET

ASP.NET MVC 4 es un marco de trabajo para crear aplicaciones web
escalables basadas en estándares, utilizando patrones de diseño bien establecidos
y el poder de ASP.NET y .NET Framework.

Sitio Oficial: http://www.asp.net/get-started

Wikipedia: http://en.wikipedia.org/wiki/ASP.NET

Existen muchas implementaciones dentro de ASP.NET que permiten la creación de
diferentes tipos de aplicaciones.
**Todas las soluciones descritas a continuación corren bajo el mismo framework
aunque sirven para propósitos distintos:**

####Websites

>Para creación de websites existen dos enfoques principales: WebForms y MVC.

#####Webforms
Webforms nace como un intento de parte de Microsoft de traer al público que trabajaba con
Visual Basic 6 desarrollando windows forms en un ambiente RAD. Los formularios son
desarrollados usando archivos .ASPX que permiten declarar en un mismo archivo código HTML
y de C#/VB.NET/Cualquier otro lenguaje del CLR.

Perdió popularidad ante frameworks más robustos que implementaban patrones MVC y MVVM
como Ruby on Rails.

En años recientes el stack de ASP.NET ha cambiado substancialmente, trayendo hacia
webforms muchas prácticas y funcionalidades de MVC.

* [Getting started with ASP.NET 4.5 Web Forms - ASP.NET](http://www.asp.net/web-forms/tutorials/aspnet-45/getting-started-with-aspnet-45-web-forms/introduction-and-overview)
* [Introduction to ASP.NET WebForms - Pluralsight](http://pluralsight.com/training/courses/TableOfContents?courseName=aspdotnet-webforms4-intro) :moneybag:

#####MVC

Fue el primer proyecto del stack de Microsoft en ser liberado bajo una licencia Open Source.

Es la implementación de Microsoft del patron
[Model-View-Controller](http://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93controller) para
ASP.NET.

**El modelo** representa el estado de un aspecto particular de la aplicación.
**El controlador** maneja las interacciones y actualiza el modelo para reflejar cambios en la aplicación.
**Los views** son responsables de presentar la información al usuario final a partir de un model.


* [ASP.NET MVC Overview - ASP.NET](http://www.asp.net/mvc/tutorials/older-versions/overview/asp-net-mvc-overview)
* [Getting started with ASP.NET MVC 5](http://www.asp.net/mvc/tutorials/mvc-5/introduction/getting-started)
* [Understanding Controllers (C#) - ASP.NET](http://www.asp.net/mvc/tutorials/controllers-and-routing/aspnet-mvc-controllers-overview-cs)
* [Introduction to the Razor Syntax - Scott Gu](http://weblogs.asp.net/scottgu/archive/2010/07/02/introducing-razor.aspx)
* [Building Applications with ASP.NET MVC - Pluralsight](http://pluralsight.com/training/Courses/TableOfContents/mvc4-building) :free:
* [Professional ASP.NET MVC 5 - Amazon](http://amzn.com/1118794753) :moneybag: Escrito por el equipo que hizo ASP.NET MVC
* [In Depth: The ASP.NET MVC Pipeline - Steve Sanderson](http://blog.stevensanderson.com/2007/11/20/aspnet-mvc-pipeline-lifecycle/) :rocket: (Rocket Science)

####APIs
Debido al auge de aplicaciones web abiertas, que extienden su funcionalidad exponiendo
métodos públicos a través de la web para que los developers construyan sobre ellas,
Microsoft publicó en el 2012 una forma más fácil de crear servicios tipo [REST]](http://en.wikipedia.org/wiki/Representational_state_transfer)

Anteriormente Microsoft había expuesto endpoints mediante el protocolo [SOAP](http://en.wikipedia.org/wiki/SOAP) que nunca se popularizo,
y luego mediante [WCF (Windows Communication Foundation)](http://en.wikipedia.org/wiki/Windows_Communication_Foundation) que resultó
ser un framework muy robusto pero difícil de implementar/configurar.

El Web API facilita la serialización de objectos a JSON y XML y su publicación a endpoints de HTTP
con mínima intervención por parte del programador.

* [Getting started with the Web API - ASP.NET](http://www.asp.net/web-api/overview/getting-started-with-aspnet-web-api/tutorial-your-first-web-api)
* [WCF or ASP.NET Web API? - The Code Project Article](http://www.codeproject.com/Articles/341414/WCF-or-ASP-NET-Web-APIs-My-two-cents-on-the-subjec)
* [Introduction to the ASP.NET Web API - Pluralsight](http://www.pluralsight.com/training/Courses/TableOfContents/aspnetwebapi) :moneybag:

#####SignalR
Es la implementación de [Web Sockets](http://en.wikipedia.org/wiki/WebSocket) para el .NET Framework

* [Introduction to SignalR - ASP.NET](http://www.asp.net/signalr/overview/signalr-20/getting-started-with-signalr-20/introduction-to-signalr)

####OWIN/KATANA

OWIN son las siglas del `Open Web Interface for .NET`. Una especificación que crea una
abstracción entre servidores web y aplicaciones web. Es efectivamente un desacoplamiento
del servidor web y la aplicación.

Esto permite la creación de plugins o `middleware` y la posibilidad de aplicaciones web
que son auto-albergadas sin la necesidad de un servidor como IIS. Este approach que se hizo
popular con frameworks como NodeJS facilita incluso la implementación de aplicaciones web
en ambientes que no dependan de windows.


* [Getting started with OWIN and Katana - ASP.NET](http://www.asp.net/aspnet/overview/owin-and-katana/getting-started-with-owin-and-katana)
