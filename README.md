# migrations-wildfly-java

[https://docs.wildfly.org/](https://docs.wildfly.org/)

## WildFly 13 ?

[https://docs.wildfly.org/13/Getting_Started_Guide.html](https://docs.wildfly.org/13/Getting_Started_Guide.html)

Mai 2018. 

Releasé avant la LTS Java 11. A priori compatible Java 8, 9, 10.

Java EE 7.

## Wildfly 15 ?

[https://www.wildfly.org/news/2018/12/13/WildFly15-Final-Released/](https://www.wildfly.org/news/2018/12/13/WildFly15-Final-Released/)

[https://docs.wildfly.org/15/Getting_Started_Guide.html](https://docs.wildfly.org/15/Getting_Started_Guide.html)

Décembre 2018.

Première version compatible Java 11. Compatible Java 8, 9, 10, 11.

Java EE 8.

## "Equivalences" avec JBoss EAP et JEE

[http://www.mastertheboss.com/jboss-server/jboss-eap/what-is-the-difference-between-jboss-eap-wildfly-and-jboss-as](http://www.mastertheboss.com/jboss-server/jboss-eap/what-is-the-difference-between-jboss-eap-wildfly-and-jboss-as)

[https://access.redhat.com/articles/113373](https://access.redhat.com/articles/113373)

| Java EE       | JBoss EAP    | WildFly       |
| ------------- | -------------| ------------- |
| 7             | 7.0 et 7.1   | 8 à 13        |
| 8             | 7.2 et 7.3   | 14 à 21       |

## Red Hat Application Migration Toolkit

[https://access.redhat.com/documentation/en-us/red_hat_application_migration_toolkit/4.2/](https://access.redhat.com/documentation/en-us/red_hat_application_migration_toolkit/4.2/)

Migration paths:
[https://access.redhat.com/documentation/en-us/red_hat_application_migration_toolkit/4.2/html/getting_started_guide/supported_configurations](https://access.redhat.com/documentation/en-us/red_hat_application_migration_toolkit/4.2/html/getting_started_guide/supported_configurations)

![Supported Source Platform Migration Paths](RHAMT_1.png)

## LTS Java Oracle

[https://www.oracle.com/java/technologies/java-se-support-roadmap.html](https://www.oracle.com/java/technologies/java-se-support-roadmap.html)

## Migration Java

Migrer une application de Java 8 à Java 11 n'impose pas de modulariser le code de l'application.

Mais la JRE a été modularisée depuis Java 9. Par exemple [les classes de JAXB ont été déplacées dans un module](https://www.jesperdj.com/2018/09/30/jaxb-on-java-9-10-11-and-beyond/). Il y a donc des actions à mener pour les réinclure dans le(s) classpath(s).

### migrer le code applicatif en modules






