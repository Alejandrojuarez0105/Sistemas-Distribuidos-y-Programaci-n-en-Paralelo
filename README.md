# Sistemas Distribuidos y Programación en Paralelo
# Clase 1 - .NET

## Porcentajes:
* Parcial = 25%
* Entregas de portafolios y ejercicios = 20%
* Interés = 5%
* Final = 50%


## Primera clase:

.NET
Es una plataforma de desarrollo de propósito general para la construcción de diferentes tipos de aplicaciones.

.NET es una Plataforma NO un lenguaje de programación

### Estructura .NET
* CIL (Common Intermediate Language) -> Es el lenguaje de programación que permite la interoperabilidad entre todos los lenguajes soportados en la plataforma .NET. El compilador .NET de cualquier lenguaje debe cumplir todas las normas dictadas por el CLS (Common Language Specification) para que el código CIL generado sea compatible 100% con el resto de lenguajes .NET. Esto nos permite que los ensamblados generados en un lenguaje puedan ser reutilizados por otros, ya que todos se traducen al mismo lenguaje CIL y se interpretan por la máquina virtual de .NET de la misma manera.

* CLR (Common Language Runtime) -> Es lo que se llama un entorno de ejecución para cualquier código de la plataforma .NET compilado. Se encarga de la compilación Just-In-Time (JIT) del CIL al código máquina nativo mediante un compilador en tiempo de ejecución.
  
* Cuando ejecuto un .NET necesito tener un CLS
  
* El CLR es como el director de orquesta
  
* El garbage collector es gestionado por el CLR

### Metadatos
Es el conjunto de información almacenada en los ensamblados que informa sobre todas las características de las clases incluidas en el código generado.
Cuando el compilador .NET genera el código CIL, además de incluir en él las instrucciones correspondientes a las sentencias fuente escritas por el programador, incluye un conjunto de *METADATOS* que describen todas las clases o tipos incluidos en la biblioteca y cada uno de los miembros de cada tipo.

### Reflection
Facultad de .NET mediante la cual en tiempo de ejecución se puede cargar una biblioteca completamente desconocida y:
* Determinar qué clases pueden proporcionar
* Conocer cuáles son la totalidad de miembros de cada clase (públicos o privados).
* Instanciar objetos de esas clases
* Invocar a sus métodos
* Tomar o alterar el valor de sus propiedades

Reflection, como no podía ser de otra manera, está implementada en un conjunto de clases que forma parte de la biblioteca de clases de .NET. Y se apoya en los metadatos que el compilador almacena en los ficheros EXE y DLL.

### Código gestionado
Se denomina código gestionado a todo el código que se ha generado mediante compiladores .NET y que, por lo tanto, va a ser ejecutado bajo el control del Common Language Runtime (CLR)

### Visual Studio
Entorno integrado de desarrollo (IDE) para programar, depurar, probar e implementar soluciones en cualquier plataforma .NET.

### C#
Lenguaje de programación elegante, tipado y orientado a objetos que permite a los desarrolladores crear una gran variedad de aplicaciones seguras y sólidas que se ejecutan en el ecosistema de .NET

### .NET Framework vs .NET
| Característica               | .NET Framework                                    | .NET (Core/5+)                                   |
|------------------------------|---------------------------------------------------|--------------------------------------------------|
| **Plataforma**                | Exclusiva para Windows                            | Multiplataforma (Windows, macOS, Linux)          |
| **Madurez**                   | Lanzado en 2002, es una plataforma madura y estable| Lanzado en 2016 como .NET Core, evolucionó a .NET 5 en 2020 y versiones posteriores |
| **Compatibilidad**            | Compatible con aplicaciones existentes que se ejecutan en Windows | No completamente compatible con todas las bibliotecas y aplicaciones de .NET Framework, pero muchas se pueden migrar |
| **Desarrollo**                | Ideal para aplicaciones de escritorio (Windows Forms, WPF) y aplicaciones web (ASP.NET) que se ejecutan en servidores Windows | Ideal para aplicaciones modernas, incluyendo aplicaciones web (ASP.NET Core), microservicios, aplicaciones de consola y más |
| **Rendimiento**               | -                                                 | Mejor rendimiento y menor consumo de recursos en comparación con .NET Framework |
| **Actualizaciones**           | Recibe actualizaciones de mantenimiento, pero no se espera que reciba nuevas características importantes | Recibe actualizaciones frecuentes con nuevas características y mejoras |

### WCF
Windows Communication Foundation en .NET es la tecnología que nos permite desarrollar servicios SOA (Service Oriented Applications)

### .NET Remoting
También parte del framework de .NET, .NET Remoting es una interfaz para comunicación de procesos remotos. Esta API nos permite desarrollar aplicaciones remotas fácilmente. Los componentes que forman parte de la aplicación bien pueden estar todos en las mismas máquinas o distribuidos por el mundo. Conceptualmente .NET Remoting se parece a Java RMI.

### DevOps
La palabra surge a partir de la fusión de dos términos en inglés development (desarrollo) y operations (operaciones). Está práctica tiene como objetivo unificar el ciclo de vida del software, defendiendo enérgicamente la automatización y el monitoreo en todos los pasos de ese ciclo y asumiéndolo como un proceso cíclico en continua retroalimentación.

#### Para pensar:
* ¿Qué es el software libre?
* ¿Qué es un método privado?
* Ser consciente de nuestra ignorancia, es decir, saber escuchar ideas y ser sinceros si no sabemos algo.
* NO SE PUEDE meter el método que prueba dentro de una misma clase, son diferentes capas.
* No es lo mismo programar orientado a objetos a que algo sea haga como código spaghetti. 
* No confundir visual studio code con visual studio
* Preguntar siempre, mucho, mucho, mucho
* Un código se puede decompilar
