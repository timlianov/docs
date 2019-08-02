# Python and Java web-stacks comparison

|                               | Java/Spring                                                   | Python/aiohttp                                | Python/Django                              | Python/Flask                               |
|-------------------------------|---------------------------------------------------------------|-----------------------------------------------|--------------------------------------------|--------------------------------------------|
| Links                         | [github](https://github.com/spring-projects/spring-framework) | [github](https://github.com/aio-libs/aiohttp) | [github](https://github.com/django/django) | [github](https://github.com/pallets/flask) |
| Proposed architecture pattern | monolith                                                      | microservices (k8s-driven)                    | monolotith                                 | monolith, microservices (k8s-driven)       |
| AJAX                          | Yes                                                           | Yes                                           | Yes                                        | Yes                                        |
| MVC framework                 | Yes                                                           | No                                            | Yes                                        | No                                         |
| i18n & l10n                   | Yes                                                           | No                                            | Yes                                        | Yes                                        |
| ORM                           | Yes                                                           | SQL-Alchemy                                   | Yes                                        | SQL-Alchemy                                |
| DB migrations                 | Flyway,  luquibase                                            | alembic                                       | Yes                                        | Flask-Migrate, alembic                     |
| Security                      | Yes                                                           | aiohttp-security (3rd-party lib)              | Yes                                        | Yes                                        |


## Java / Spring Framework
A key element of Spring is infrastructural support at     the application level: Spring focuses on the "plumbing" of enterpri    se applications so that teams can focus on application-level busine    ss logic, without unnecessary ties to specific deployment environme    nts.

### Key features
- Lightweight: Spring Framework is lightweight with respect to size and transparency.
- Inversion Of Control (IOC): In Spring Framework, loose coupling is achieved using Inversion of Control. The objects give their own dependencies instead of creating or looking for dependent objects.
- Aspect Oriented Programming (AOP): By separating application business logic from system services, Spring Framework supports Aspect Oriented Programming and enables cohesive development.
- Container: Spring Framework creates and manages the life cycle and configuration of application objects.
- MVC Framework: Spring Framework is a MVC web application framework. This framework is configurable via interfaces and accommodates multiple view technologies.
- Transaction Management: For transaction management, Spring framework provides a generic abstraction layer. It is not tied to J2EE environments and it can be used in container-less environments.
- JDBC Exception Handling: The JDBC abstraction layer of the Spring Framework offers an exception hierarchy, which simplifies the error handling strategy.

## Python / aiohttp

It is an Async http client/server framework. It su    pports both client and server Web-Sockets out-of-the-box and avoids     Callback. It provides Web-server with middlewares and pluggable ro    uting.

### Key features
 - Supports both client and server side of HTTP protocol.
 - Supports both client and server Web-Sockets out-of-the-box and avoids Callback Hell.
 - Provides Web-server with middlewares and pluggable routing.

## Python / Django
Django is a high-level Python Web framework that e    ncourages rapid development and clean, pragmatic design.

### Key features
- a lightweight and standalone web server for development and testing
- a form serialization and validation system that can translate between HTML forms and values suitable for storage in the database
- a template system that utilizes the concept of inheritance borrowed from object-oriented programming
- a caching framework that can use any of several cache methods
- support for middleware classes that can intervene at various stages of request processing and carry out custom functions
- an internal dispatcher system that allows components of an application to communicate events to each other via pre-defined signals
- an internationalization system, including translations of Django's own components into a variety of languages
- a serialization system that can produce and read XML and/or JSON representations of Django model instances
- a system for extending the capabilities of the template engine
- an interface to Python's built-in unit test framework
- Django REST framework is a powerful and flexible toolkit for building Web APIs.

## Python / Flask

Flask is a micro web framework written in Python. It is classified as a microframework because it does not require particular tools or libraries. It has no database abstraction layer, form validation, or any other components where pre-existing third-party libraries provide common functions. However, Flask supports extensions that can add application features as if they were implemented in Flask itself. 

### Key features
- Contains development server and debugger
- Integrated support for unit testing
- RESTful request dispatching
- Uses Jinja2 templating
- Support for secure cookies (client side sessions)
- 100% WSGI 1.0 compliant
- Unicode-based
- Extensive documentation
- Google App Engine compatibility
- Extensions available to enhance features desired



