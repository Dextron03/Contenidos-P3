# Tu Guía Completa para Programación 3 (P3)

¡Hola! Bienvenido a tu ruta de aprendizaje para Programación 3. Este documento está diseñado para ser tu compañero de estudio. Hemos traducido todos esos términos técnicos a un lenguaje sencillo, con ejemplos de la vida real, y los hemos combinado con los objetivos exactos de tu curso.

Ponte cómodo, prepárate un café, y vamos a recorrer paso a paso todo lo que vas a aprender en esta increíble aventura creando aplicaciones modernas con **.NET**.

---

## Módulos 1 y 2: Fundamentos MVC, Entity Framework y Operaciones CRUD

**¿Qué te espera en este módulo? (Lo académico)**
En estos primeros pasos aprenderás a crear y gestionar modelos de datos en ASP.NET Core MVC, además de implementar las operaciones básicas que toda aplicación necesita: CRUD (Crear, Leer, Actualizar, Borrar). Todo esto utilizando Entity Framework Core. También conocerás cómo aplicar migraciones, trabajar con consultas LINQ y conectar la base de datos con tu página web.
*   *Subtemas:* Creación de modelos en MVC, Introducción a EF Core (Code First), Operaciones CRUD, uso básico de LINQ y un laboratorio práctico.

**Explicación:**
Para entender el patrón **MVC (Modelo-Vista-Controlador)**, imagina un restaurante de lujo. Tú eres el cliente que hace un pedido. El **Controlador** es el camarero experimentado: toma tu orden, va a la cocina, solicita lo necesario y te lleva el plato terminado. El **Modelo** representa la cocina y los ingredientes: es el núcleo donde están las reglas de cómo preparar la comida (la lógica de tu aplicación y la estructura de los datos). Finalmente, la **Vista** es la presentación espectacular de tu plato en la mesa: la página web (el código HTML y CSS) que ves en la pantalla de tu navegador. Separar estas tres partes asegura que, si el chef decide cambiar la receta, el camarero no necesite aprender un trabajo nuevo, manteniendo el restaurante (tu código) en perfecto orden.

Por otro lado, conectar tu aplicación a una base de datos históricamente requería hablar en un lenguaje tosco llamado SQL. **Entity Framework (un ORM)** es tu traductor automático. En lugar de escribir sentencias complejas de base de datos, tú trabajas cómodamente con objetos en C# (como crear una clase "Cliente"). Entity Framework toma ese objeto, lo traduce a SQL por detrás, y lo guarda en la base de datos de manera invisible. Es como tener un secretario que se encarga de todo el papeleo engorroso por ti.

**Recursos (Videos):**
*   [MVC - The Model View Controller Design Pattern Explained](https://www.youtube.com/watch?v=Tp3G7VKSbu0)
*   [Controllers and Views in .NET 9: A Quick Start Guide for Beginners](https://www.youtube.com/watch?v=wFEuR2Wu9f4)
*   [Step-by-Step Tutorial: ASP.NET Core MVC + EF Core in .NET 9](https://www.youtube.com/watch?v=U1Pi3AMEflA)
*   [C# Essentials: Linq for Lists](https://www.youtube.com/watch?v=yClSNQdVD7g)

**Artículos y Foros Recomendados:**
*   [Overview of ASP.NET Core MVC (Microsoft)](https://learn.microsoft.com/en-us/aspnet/core/mvc/overview?view=aspnetcore-8.0)
*   [Handle requests with controllers in ASP.NET Core MVC](https://learn.microsoft.com/en-us/aspnet/core/mvc/controllers/actions?view=aspnetcore-8.0)
*   [Tutorial: Code First Approach in ASP.NET Core MVC with EF (Medium)](https://medium.com/c-sharp-programming/tutorial-code-first-approach-in-asp-net-core-mvc-with-ef-5baf5af696e9)

**Proyectos de Ejemplo:**
*   `Proyectos Ejemplo/Primer Proyecto/NewSuperMarket2025.rar`
*   `Proyectos Ejemplo/Segundo Proyecto/ItlaInvestmentApp.zip`
*   `Proyectos Ejemplo/Tercer Proyecto/ItlaInvestmentApp.rar`

---

## Módulo 3: Arquitectura Cebolla (Onion Architecture) e Inyección de Dependencias

**¿Qué te espera en este módulo? (Lo académico)**
Se introducirá la Arquitectura Onion como una forma moderna de estructurar aplicaciones para lograr independencia entre capas y un mejor mantenimiento. Separaremos la lógica de negocio (Dominio) de la persistencia (Infraestructura), aplicando principios de diseño como SOLID y Clean Architecture.
*   *Subtemas:* Principios de arquitectura en capas, Dominio y Entidades, Persistencia y Repository Pattern, Inyección de Dependencias y comparación con Clean Architecture.

**Explicación:**
A medida que desarrollas software, el código crece y puede convertirse rápidamente en un monstruo inmanejable donde tocar una línea rompe diez más. Aquí es donde entra la **Arquitectura Cebolla**. Imagina tu proyecto, literalmente, como una cebolla con varias capas protectoras concéntricas. En el centro exacto, resguardado de todo el mundo exterior, viven las reglas más importantes de tu negocio (tu *Dominio*). Las capas exteriores son detalles que pueden cambiar con el tiempo, como la base de datos o si usas una página web o una app móvil (tu *Infraestructura* y *Presentación*). La regla de oro aquí es que las capas externas pueden conocer el centro, pero el centro jamás debe depender de las capas externas. Así, si mañana cambias de base de datos, tu núcleo permanece intacto.

Acompañando a esta arquitectura, está el concepto vital de la **Inyección de Dependencias**. Piensa en ello como un quirófano. Un cirujano (tu código) no debe preocuparse por fabricar su propio bisturí o desinfectar sus guantes. Simplemente pide "necesito un bisturí", y una enfermera (el inyector de dependencias) le proporciona inmediatamente una herramienta limpia y lista para usar. Esto hace que tus componentes de software sean ligeros, especializados y muchísimo más fáciles de probar.

**Recursos (Videos):**
*   [Hexagonal, Onion & Clean Architecture](https://www.youtube.com/watch?v=JubdZIdLQ4M)
*   [¿Qué es la ARQUITECTURA CEBOLLA? | Onion Architecture](https://www.youtube.com/watch?v=NzeqehKvM10)
*   [Dependency Injection for Absolute Beginners with C#](https://www.youtube.com/watch?v=tTJetZj3vg0)

**Artículos y Foros Recomendados:**
*   [The S.O.L.I.D Principles in Pictures (Medium)](https://medium.com/backticks-tildes/the-s-o-l-i-d-principles-in-pictures-b34ce2f1e898)
*   [The Clean Architecture (Uncle Bob)](https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html)
*   [Understanding Onion Architecture (CodeGuru)](https://www.codeguru.com/csharp/understanding-onion-architecture/)
*   [Onion Architecture (Dev.to)](https://dev.to/barrymcauley/onion-architecture-3fgl)
*   [Dependency injection in ASP.NET Core (Microsoft)](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/dependency-injection?view=aspnetcore-8.0)

**Proyectos de Ejemplo:**
*   `Proyectos Ejemplo/Cuarto Proyecto/ItlaInvestmentApp.rar`
*   `Proyectos Ejemplo/Quinto Proyecto/ItlaInvestmentAppWithAutomapper.rar`

---

## Módulo 6: Autenticación y Autorización con ASP.NET Identity

**¿Qué te espera en este módulo? (Lo académico)**
Aprenderás a implementar ASP.NET Core Identity, el sistema de seguridad más usado en aplicaciones web .NET. Verás cómo gestionar usuarios, roles, contraseñas, y cómo extender esto con la confirmación de correos y recuperación de contraseñas. *(Nota: También se repasan temas extras como subida de archivos, uso de AutoMapper, envío de correos y manejo de sesiones).*

**Explicación:**
Toda aplicación seria necesita un sólido sistema de control de acceso. Crear uno desde cero es peligroso y propenso a errores (¿cómo guardarías las contraseñas sin que sean robadas?). **ASP.NET Core Identity** es como contratar a una agencia de seguridad de élite para el edificio de tu aplicación.

Esta "agencia" se encarga del trabajo pesado y delicado: no solo registra usuarios y verifica que sus credenciales sean correctas al iniciar sesión (*Autenticación*), sino que también implementa complejos algoritmos de encriptación (hashing) para que, incluso si alguien roba tu base de datos, las contraseñas sigan siendo indescifrables. Además, maneja la *Autorización*, verificando su lista de invitados para saber si la persona que entra es un "Usuario Normal" que solo puede leer, o un "Administrador" que tiene las llaves de todo el sistema. También automatizan flujos molestos como enviar los correos electrónicos de "Haz clic aquí para confirmar tu cuenta" o el siempre necesario "Olvidé mi contraseña".

**Recursos (Videos):**
*   [Authentication made easy with ASP.NET Core Identity](https://www.youtube.com/watch?v=S0RSsHKiD6Y)
*   [Complete ASP NET Core Identity Tutorial](https://www.youtube.com/watch?v=ACsFF1mkEsQ)
*   [Mapping C# data with AutoMapper - Complete tutorial](https://www.youtube.com/watch?v=Ijw0Q5EOqmE)
*   [Envía Email como un PRO con C# y MailKit](https://www.youtube.com/watch?v=Ye-zSiZGLog)

**Artículos y Foros Recomendados:**
*   [Upload Files In ASP.NET MVC 5 (C# Corner)](https://www.c-sharpcorner.com/article/upload-files-in-asp-net-mvc-5/)
*   [What are Web Sessions ? — ELI5 (Medium)](https://medium.com/@naveenxdex/what-are-web-sessions-eli5-86bced56982b)
*   [How To Use Sessions In ASP.NET Core (C# Corner)](https://www.c-sharpcorner.com/article/how-to-use-session-in-asp-net-core/)
*   [Sending Emails in .Net 5 With MailKit](https://improveandrepeat.com/2021/09/sending-emails-in-net-5-with-mailkit/)
*   [Getting Started with AutoMapper in ASP.NET Core (Code-Maze)](https://code-maze.com/automapper-net-core/)
*   [ASP.NET Core Identity Tutorial (TekTutorialsHub)](https://www.tektutorialshub.com/asp-net-core/asp-net-core-identity-tutorial/)

**Proyectos de Ejemplo:**
*   `Proyectos Ejemplo/Sexto Proyecto/ItlaInvestmentAppWithIdentity (1).rar`

---

## Módulos 7 y 8: Creación y Seguridad de APIs RESTful (JWT)

**¿Qué te espera en estos módulos? (Lo académico)**
Se introducen las APIs como componente esencial moderno para conectar clientes externos. Verás cómo exponer endpoints, usar Swagger, y algo fundamental: la seguridad en APIs. Implementarás JWT (JSON Web Tokens) y Bearer Authentication para proteger la información de accesos no autorizados.

**Explicación:**
A medida que la tecnología avanza, tu sistema no solo será consumido desde un navegador web de escritorio, sino también por aplicaciones móviles, relojes inteligentes y hasta refrigeradores con pantallas. Estos dispositivos no saben qué hacer con el HTML lleno de botones y colores de tu página web; solo necesitan *datos*. Una **API (Application Programming Interface)** es la ventanilla de atención que devuelve solo la información pura (generalmente en un formato de texto ligero llamado JSON), actuando como el cerebro central que alimenta a todos estos dispositivos.

Sin embargo, como esta ventanilla da a la calle y cualquiera puede hacerle solicitudes, la seguridad cambia radicalmente. En lugar de usar las clásicas 'Cookies' que funcionan solo en navegadores, las APIs modernas utilizan **JSON Web Tokens (JWT)**. Piensa en el JWT como una pulsera VIP de un festival de música. Al llegar al festival (el inicio de sesión), presentas tu identificación (usuario y contraseña). Si todo es correcto, te ponen esta pulsera criptográfica. A partir de ese momento, para entrar a cualquier zona restringida, ya no presentas tu identificación, simplemente muestras tu pulsera (el Token) con cada solicitud que hagas, demostrando instantáneamente quién eres y qué privilegios posees.

**Recursos (Videos):**
*   [What is an API (in 5 minutes)](https://www.youtube.com/watch?v=ByGJQzlzxQg)
*   [Build REST APIs in .NET 9](https://www.youtube.com/watch?v=38GNKtclDdE)
*   [Top 12 Tips For API Security](https://www.youtube.com/watch?v=6WZ6S-qmtqY)
*   [Secure Your ASP NET Core API with JWT](https://www.youtube.com/watch?v=tBESNoQjlVQ)

**Artículos y Foros Recomendados:**
*   [ASP.NET Core 5 — JWT Authentication Tutorial with Example API (Medium)](https://medium.com/c-sharp-programming/asp-net-core-5-jwt-authentication-tutorial-with-example-api-aa59e80d02da)
*   [Asp Net Core 5 Rest API Authentication with JWT Step by Step (Dev.to)](https://dev.to/moe23/asp-net-core-5-rest-api-authentication-with-jwt-step-by-step-140d)
*   [Refresh JWT with Refresh Tokens in Asp Net Core 5 Rest API Step by Step (Dev.to)](https://dev.to/moe23/refresh-jwt-with-refresh-tokens-in-asp-net-core-5-rest-api-step-by-step-3en5)

**Proyectos de Ejemplo:**
*   `Proyectos Ejemplo/Septimo Proyecto/ItlaInvestmentAppWithApi.rar`
*   `Proyectos Ejemplo/Octavo Proyecto/ItlaInvestmentAppWithApiSecurity.rar`

---

## Módulo 9: Patrón CQRS, MediatR y Azure Functions

**¿Qué te espera en este módulo? (Lo académico)**
Trabajaremos con el patrón CQRS (Command and Query Responsibility Segregation), el uso del patrón Mediator y la implementación de código en la nube (Azure Functions). Esto sirve para arquitecturas modernas, mejorando la mantenibilidad y preparándonos para sistemas que manejan muchos eventos o necesitan escalar.

**Explicación:**
En este módulo, el nivel arquitectónico se vuelve fascinante. Comenzaremos con **CQRS**. Las aplicaciones tradicionales usan la misma "tubería" en el código tanto para guardar datos como para buscarlos. Pero en el mundo real, una página suele leerse miles de veces por cada vez que se modifica algo. CQRS separa radicalmente esto en dos tuberías distintas: una optimizada exclusivamente para hacer *Preguntas* (Queries, consultas rápidas) y otra para ejecutar *Órdenes* (Commands, modificaciones complejas). Esta separación permite que el sistema respire y sea muchísimo más veloz bajo presión.

Para acompañar esto, utilizamos el patrón **Mediator**. Imagina el caos de un aeropuerto donde los pilotos de los aviones tuvieran que hablarse entre todos simultáneamente para no chocar. El código acoplado es igual de caótico. El Mediator actúa como la torre de control: ningún piloto (clase de tu código) se habla directamente con otro. Todos envían un mensaje a la torre, y es la torre la encargada de rutear la información al componente adecuado. Esto resulta en un código bellamente desacoplado.

Por último, echaremos un vistazo a **Azure Functions**, que introduce el concepto de "Serverless" (sin servidor). En lugar de alquilar una máquina completa las 24 horas del día solo para ejecutar una pequeña tarea de limpieza cada madrugada, programas una Función de Azure. Es un trozo de código flotando en la nube que despierta, ejecuta su tarea y vuelve a dormir, cobrándote fracciones de centavo solo por el milisegundo exacto en que operó.

**Recursos (Videos):**
*   [Mastering CQRS in Just 5 Minutes](https://www.youtube.com/watch?v=SvjdJoNPcHs)
*   [Patrón CQRS explicado FÁCIL en 10 minutos](https://www.youtube.com/watch?v=DJCWpUVf5E0)
*   [Intro to MediatR](https://www.youtube.com/watch?v=yozD5Tnd8nw)

**Artículos y Foros Recomendados:**
*   [Clean code architecture and CQRS pattern based web api (Dev.to)](https://dev.to/silentrobi/clean-code-architecture-and-cqrs-pattern-based-web-api-using-netcore-4a2e)
*   [CQRS (Martin Fowler)](https://martinfowler.com/bliki/CQRS.html)
*   [Mediator (Refactoring Guru)](https://refactoring.guru/es/design-patterns/mediator)
*   [What are Azure Functions (C# Corner)](https://www.c-sharpcorner.com/article/what-is-azure-functions/)

**Proyectos de Ejemplo:**
*   `Proyectos Ejemplo/Noveno Proyecto/ItlaInvestmentAppWithCqrsMediatorAndAzureFunctions.rar`

---

## Módulo 10: Documentación Swagger y Unit Testing (xUnit)

**¿Qué te espera en este módulo? (Lo académico)**
Abordaremos herramientas fundamentales: cómo documentar tu API usando Swagger/OpenAPI y cómo implementar pruebas unitarias automatizadas usando la librería xUnit en .NET. Prepárate porque aquí cae el Segundo Parcial.

**Explicación:**
Cuando creas una API, esta se convierte en el producto que otras personas (u otros equipos de desarrollo) van a consumir. Si les entregas una API sin manual, es como vender un mueble desarmado sin las instrucciones. **Swagger** soluciona esto generando de manera automática un manual interactivo. Analiza tu código y crea una página web pulida donde cualquier desarrollador puede ver exactamente qué hace tu API e incluso probarla en vivo haciendo clics, sin necesidad de escribir ni una sola línea de código para testearla.

Por otro lado, a medida que tu software se hace complejo, hacer pruebas manuales (ejecutar la app, hacer clic aquí, llenar un formulario allá) se vuelve una tarea titánica y propensa a descuidos. **xUnit (Pruebas Unitarias)** es la práctica de escribir código cuyo único propósito en la vida es probar tu código de producción. Construyes pequeños inspectores de calidad automatizados. Así, si dentro de seis meses cambias una función matemática crítica y accidentalmente la rompes, tu batería de pruebas unitarias saltará en rojo en cuestión de milisegundos, avisándote del error antes de que el código defectuoso llegue a las manos del usuario final.

**Recursos (Videos):**
*   [How to Improve Swagger API Documentation](https://www.youtube.com/watch?v=H-hlgAi3B-M)
*   [What Is Unit Testing?](https://www.youtube.com/watch?v=x95ez7_V7rA)

**Artículos y Foros Recomendados:**
*   [What is SwaggerUI (C# Corner)](https://www.c-sharpcorner.com/blogs/net-core-api-with-swagger-documentation)
*   [ASP.NET Core web API documentation with Swagger / OpenAPI (Microsoft)](https://learn.microsoft.com/en-us/aspnet/core/tutorials/web-api-help-pages-using-swagger?view=aspnetcore-6.0)
*   [Introducción a xUnit (Dev.to)](https://dev.to/maadcode/introduccion-a-xunit-una-poderosa-herramienta-para-unit-testing-en-net-34b0)
*   [The Ultimate Guide to Unit Testing in .NET (C#) Using xUnit and Moq (Dev.to)](https://dev.to/zrebhi/the-ultimate-guide-to-unit-testing-in-net-c-using-xunit-and-moq-without-the-boring-examples-28ad)

**Proyectos de Ejemplo:**
*   `Proyectos Ejemplo/Decimo Proyecto/ItlaInvestmentAppWithApiDocumentationAndTests.rar`

---

## Módulo 11: Manejo Global de Errores

**¿Qué te espera en este módulo? (Lo académico)**
Nos enfocaremos en cómo capturar las excepciones (errores) en toda la aplicación de forma centralizada utilizando Middleware personalizado e IExceptionHandler, asegurando aplicaciones más seguras y fáciles de mantener.

**Explicación:**
En el desarrollo de software, los errores (Excepciones) van a ocurrir, es inevitable. La base de datos se caerá un segundo, el usuario enviará un formato incorrecto o un archivo no se encontrará. Si no atrapas estos errores correctamente, la aplicación colapsará violentamente, mostrándole al usuario final una pantalla terrorífica llena de texto críptico y líneas de código exponiendo la fragilidad de tu sistema.

El **Manejo Global de Excepciones** (Global Exception Handling) es como instalar una gigantesca red de seguridad de circo debajo de todo el trapecio que es tu código. Si en cualquier rincón oscuro de tu aplicación algo falla y un proceso "cae", en lugar de estrellarse contra el suelo, es atrapado suavemente por esta red central. Allí, tu red inspecciona qué fue lo que falló, lo anota discretamente para que tú lo revises luego, y le devuelve al usuario un mensaje elegante, profesional y tranquilo, como: "Lo sentimos, estamos experimentando un inconveniente técnico momentáneo, por favor intenta en unos minutos", salvaguardando la experiencia de usuario y la seguridad de tu servidor.

**Recursos (Videos):**
*   [Global Error Handling in .NET Just Got WAY Better](https://www.youtube.com/watch?v=rXdsm9R5TR0)
*   [Coding Shorts: ASP.NET Core Middleware Explained](https://www.youtube.com/watch?v=TqCshF0o0nE)

**Artículos y Foros Recomendados:**
*   [ASP.NET Core Middleware (Microsoft)](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/middleware/?view=aspnetcore-6.0)
*   [Middleware in ASP.NET 6 - Intro and Basics (Exception Not Found)](https://exceptionnotfound.net/middleware-in-asp-dotnet-6-intro-and-basics/)
*   [Global Error Handling in ASP.NET Core 8 (Milan Jovanovic)](https://www.milanjovanovic.tech/blog/global-error-handling-in-aspnetcore-8)

**Proyectos de Ejemplo:**
*   `Proyectos Ejemplo/Decimo Primer Proyecto/ItlaInvestmentAppWithGlobalExceptionHandler.rar`

---

## Módulo 12: Comportamientos y Validaciones (Behavior Pipelines)

**¿Qué te espera en este módulo? (Lo académico)**
Aprenderás a usar Behavior Pipelines en MediatR y validaciones con FluentValidation. Esto permite estructurar la lógica limpiamente y garantizar que los datos cumplan reglas estrictas antes de ser procesados por la aplicación.

**Explicación:**
El código central que maneja las reglas vitales de tu negocio no debería tener que lidiar con minucias administrativas. Es como tener al director general de un banco revisando personalmente si el formulario de un cliente tiene un correo electrónico válido o si un número telefónico está en blanco. Para eso existen los filtros.

Los **Behavior Pipelines** de MediatR, combinados con **FluentValidation**, actúan como una serie de estrictos puestos de control y aduanas antes de que los datos puedan si quiera rozar el núcleo de tu aplicación. El pipeline intercepta la solicitud del usuario en pleno vuelo. Si la aduana detecta que los datos no tienen sentido (por ejemplo, una fecha de nacimiento en el futuro o un pago negativo), bloquea el paso inmediatamente, aborta la operación y le devuelve un mensaje claro al usuario pidiendo la corrección. Al utilizar esta técnica, el director general (tu lógica de negocio central) asume con total confianza que cualquier documento que llega a su escritorio ya ha sido rigurosamente verificado y es 100% puro y procesable.

**Recursos (Videos):**
*   [Make Your Business Rules Cleaner With Fluent Validation](https://www.youtube.com/watch?v=AYrmu9_RFnM)
*   [MediatR Pipeline Behavior in .NET - For Beginners](https://www.youtube.com/watch?v=km4W27ggQzY)

**Artículos y Foros Recomendados:**
*   [Validation with MediatR Pipeline and FluentValidation (Code With Mukesh)](https://codewithmukesh.com/blog/validation-with-mediatr-pipeline-behavior-and-fluentvalidation/)
*   [Validate with Fluent Validations in .NET (C#) (Medium)](https://medium.com/codenx/code-with-fluent-validations-in-net-c-da2fb517566d)

**Proyectos de Ejemplo:**
*   `Proyectos Ejemplo/Decimo Segundo/ItlaInvestmentAppWithBehaviorValidation.rar`

---

## Módulo 13: Observabilidad y Logs con Serilog

**¿Qué te espera en este módulo? (Lo académico)**
Exploraremos Serilog, una de las mejores librerías para gestión de logs en .NET. El objetivo es registrar información estructurada que facilite el monitoreo, la depuración y trazabilidad de errores en entornos reales.

**Explicación:**
Cuando estás desarrollando en tu máquina personal, si algo se rompe, tú estás ahí mismo mirando la pantalla, puedes pausar el código y ver exactamente qué falló. Pero cuando tu aplicación está instalada en un servidor a miles de kilómetros de distancia, dándole servicio a miles de usuarios, te vuelves ciego y sordo a lo que sucede en sus entrañas.

Aquí es vital implementar un sistema de **Logging** (Registros o Bitácoras) potente, y **Serilog** es la herramienta ideal para ello. Serilog es la equivalente a instalar una sofisticada "caja negra" de avión en tu software. Va documentando silenciosamente todo evento crucial: quién inició sesión, cuánto tiempo tardó una base de datos en responder y, críticamente, registra el rastro forense completo cuando ocurre un error. Pero la verdadera magia de Serilog es que no escupe texto plano y desordenado; genera "Logs Estructurados". Esto significa que la información guarda un formato inteligente, permitiéndote luego entrar a un panel de control y buscar con bisturí: *"Por favor búscame todos los registros de la última hora donde la variable 'UsuarioId' fue igual a 554 y el estado del pago haya dado error"*. Esto reduce el tiempo para cazar un bug de días a meros minutos.

**Recursos (Videos):**
*   [How to Add Professional Logging in .NET with Serilog](https://www.youtube.com/watch?v=ZI1Ufk-foKo)

**Artículos y Foros Recomendados:**
*   [Serilog y ASP.NET Core: Más Allá de los Logs Básicos - Parte 9 (Dev.to)](https://dev.to/isaacojeda/parte-9-aspnet-core-logging-con-serilog-48o4)
*   [5 Serilog Best Practices For Better Structured Logging (Milan Jovanovic)](https://www.milanjovanovic.tech/blog/5-serilog-best-practices-for-better-structured-logging)
*   [Getting Started (GitHub Serilog Wiki)](https://github.com/serilog/serilog/wiki/Getting-Started)

**Proyectos de Ejemplo:**
*   `Proyectos Ejemplo/Decimo Tercero/ItlaInvestmentAppWithLogs.zip`

---

## Módulo 14: Despliegue en la Nube con Microsoft Azure

**¿Qué te espera en este módulo? (Lo académico)**
Abordarás el proceso de llevar tu aplicación a Microsoft Azure, entendiendo despliegues manuales y automatizados. Aprenderás a integrar todo esto con buenas prácticas de control de versiones y trabajo colaborativo (Git y Gitflow).

**Explicación:**
Después de semanas de duro trabajo programando, tienes una aplicación espectacular que... solo existe en tu disco duro. El Despliegue (Deployment) es el gran salto donde sacas tu proyecto de tu entorno de desarrollo y lo subes a un entorno de producción en internet para que el mundo entero pueda usarlo. Utilizaremos **Microsoft Azure**, uno de los servicios en la nube más poderosos del planeta, para hospedar tu base de datos y tus servidores web.

Pero subir archivos manualmente es una práctica del pasado, propensa a que alguien se equivoque copiando un archivo. Aquí descubriremos el increíble mundo de la automatización a través de **CI/CD** (Integración Continua y Despliegue Continuo). Configurarás un flujo de trabajo moderno (usando Git, GitHub Workflows) en el que la magia ocurre sola: cada vez que tú y tu equipo terminen de trabajar y suban una nueva versión del código fuente al repositorio, una flota de robots invisibles (servidores en la nube) tomarán el código, ejecutarán tus pruebas unitarias de calidad, empaquetarán la aplicación y la instalarán de manera segura y automática en los servidores de Azure, ¡todo esto mientras tú te sirves una taza de café!

**Recursos (Videos):**
*   [Manual Deployment to Azure from Visual Studio](https://www.youtube.com/watch?v=sWn44dvRIb0)
*   [CI/CD for .NET Apps on Azure Using GitHub Workflows](https://www.youtube.com/watch?v=2ieL-3eV1lU)
*   [Git Tutorial for Beginners: Learn Git in 1 Hour](https://www.youtube.com/watch?v=8JJ101D3knE)

**Artículos y Foros Recomendados:**
*   [How to actually deploy or host your ASP.NET Core Web API to Azure (Medium)](https://medium.com/@vikasosmium/how-to-actually-deploy-or-host-your-asp-net-core-web-api-to-azure-288418077d1a)
*   [Modelos basados en DTU y vCore para bases de datos SQL de Azure (LinkedIn Pulse)](https://www.linkedin.com/pulse/modelos-basados-en-dtu-y-vcore-para-bases-de-datos-soleto-olguin/)
*   [Flujo de trabajo de Gitflow (Atlassian)](https://www.atlassian.com/es/git/tutorials/comparing-workflows/gitflow-workflow)

---

## Módulo 15: Migraciones, Modernización y Proyecto Final

**¿Qué te espera en este módulo? (Lo académico)**
Aprenderás a mantener al día tus aplicaciones. Abordaremos la migración de librerías viejas a nuevas (como pasar de AutoMapper a Mapster o de MediatR a Mediator), la actualización al framework .NET 10 y mejoras en JWT. 
**Finalmente:** Desarrollarás un gran proyecto final aplicando todos los conocimientos adquiridos en los módulos previos.

**Explicación:**
El mundo del desarrollo de software avanza a un ritmo vertiginoso. Lo que hace unos años era el estándar de oro para el rendimiento, hoy puede considerarse lento o estar obsoleto. Un ingeniero senior no solo sabe crear software desde cero, sino que posee la habilidad crítica de mantener el código vivo y actualizarlo. Aprenderás a modernizar tu aplicación con cirugía de precisión, intercambiando librerías antiguas por alternativas modernas y ultra-rápidas, y realizando el salto al ecosistema más reciente de **.NET 10**, todo esto sin romper la aplicación que está funcionando.

Finalmente, el **Proyecto Final**. Este es el punto culminante de tu viaje donde todas las piezas del rompecabezas colisionan. Integrarás las bases de datos de Entity Framework, con la arquitectura cebolla, el esquema veloz de CQRS, el control de acceso de Identity, protegido todo por JWT, verificado por pruebas unitarias automatizadas y desplegado fluidamente a la nube en Microsoft Azure. Este proyecto dejará de ser una práctica para convertirse en una aplicación de nivel empresarial que formará una parte brillante y sólida de tu portafolio profesional.

**Recursos (Videos):**
*   [.NET 10 | Everything you NEED to KNOW!](https://www.youtube.com/watch?v=AbD4XST2Pcw)
*   [Migrating from AutoMapper to Mapster in .NET](https://www.youtube.com/watch?v=eeX-HbR4ZBo)
*   [.NET 9 to .NET 10 Migration + xUnit v3](https://www.youtube.com/watch?v=Cenq5929s54)

**Artículos y Foros Recomendados:**
*   [MAPSTER High-performance mapper for .NET (Medium)](https://medium.com/codenx/mapster-high-performance-mapper-for-net-767a3f361043)
*   [.NET 10: What You Need to Know (ABP.io)](https://abp.io/community/articles/.net-10-what-you-need-to-know-lts-release-coming-november-2025-xennnnky#gsc.tab=0)
*   [What’s new in .NET 10 (Microsoft)](https://learn.microsoft.com/en-us/dotnet/core/whats-new/dotnet-10/overview)

**Proyectos de Ejemplo:**
*   `Proyectos Ejemplo/Decimo Cuarto/ItlaInvestmentAppMigrationNet10.rar`

---

## Evaluaciones y Proyectos Finales

A lo largo del curso y al final del mismo, tendrás que enfrentarte a requerimientos del mundo real para poner a prueba tus conocimientos. Aquí están los mandatos oficiales para los diferentes proyectos (revisa tu asignación particular):

**Mandatos:**
*   `Mandatos/ArtemisBanking/Mini proyecto final_ Artemis banking (1).pdf`
*   `Mandatos/evote/Mini proyecto_ eVote360.pdf`
*   `Mandatos/Horizon FutureVest/Mini proyecto_ Horizon FutureVest.pdf`
*   `Mandatos/LinkUp/Mini proyecto_ LinkUp.pdf`
*   `Mandatos/Predictor/Predictor de tendencia de Activos.pdf`
*   `Mandatos/RealEstateApp/Proyecto final - RealEstateApp (1).pdf`

---

¡Disfruta mucho de este camino de aprendizaje! Estás a punto de dominar muchas herramientas que se utilizan hoy en día en empresas de tecnología a nivel mundial. ¡Manos a la obra!
