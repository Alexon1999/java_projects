-----------------------
JVM,JRE et JDK
----------------------
JVM (Java Virtual Machine), JDK (Java Development Kit) et JRE (Java Runtime Environment) sont trois composants indispensables de la plate-forme Java. Ils fonctionnent ensemble dans les applications Java.

---------------------------------------

la machine virtuelle Java (JVM), 
le kit de développement Java (JDK): créer des applications java 
l'environnement d'exécution Java (JRE): executer vos applications java


----------------------------------

- la machine virtuelle Java ou JVM est le composant de la plate-forme Java qui exécute les programmes ; 
- l’environnement d'exécution Java ou JRE crée la machine virtuelle Java ou JVM et s'assure que les dépendances sont disponibles pour les programmes Java ; 
  
- le kit de développement Java ou JDK permet de créer des programmes Java qui peuvent être exécutés par la JVM et le JRE.
  

* Compilation is done by the compiler (javac) which comes with JDK. This is the intermediate code called ByteCode. so javac compiles to bytecode and then execute on JVM 


<!-- * How it works ? -->
JVM = JIT Compiler + Java Interpreter + Garbage Collector
JRE = JVM + Library Classes
JDK = JRE + Development Tool

the source code(.java files) and bytecode(.class files)

Java compiler javac converts source code into bytecode. JIT Compiler and Java Interpreter inside JVM convert the bytecode into corresponding machine code.

<!-- ? History -->
- Java SE, JSE : Java Standard Edition : la base de java (core java)

- J2EE(Java 2 Entreprise Edition) :  pour créer des applications backend (cotés serveur)

- Après on l'appelle Java EE (JEE) Java Enterprise Edition
  
- en 2018, Oracle prend le projet Java EE (JEE) , et on a remplacé le nom par Jakarta EE

<!-- JEE applications can run on the same JRE as JSE -->
Alors que Java SE constitue le framework de référence pour Java — avec des bibliothèques standards répondant à la plupart des besoins —, Java EE complète ce framework avec des bibliothèques logicielles additionnelles dédiées à des applications professionnelles, facilitant par exemple le développement d'applications pour architecture distribuée. 

pourquoi utiliser JAVA EE ?
on l'utilise pour développer des applications de serveur (Backend applications)
si votre application exige un système distribué à très grande échelle, alors vous devriez envisager D'utiliser Java EE. Construit sur le dessus de Java SE, il fournit des bibliothèques pour l'accès à la base de données (JDBC, JPA), remote method invocation (RMI ), messaging ( JMS ), web services, XML processing, and defines standard API for Enterprise JavaBeans, servlets, portlets, Java Server Pages, etc...

Les JDK spécifiques à Java EE sont conçus de façon qu'une application réalisée avec Java EE fonctionne sur le même JRE qu'une application écrite avec Java SE, mais nécessitera cependant qu'en complément, les bibliothèques exploitées soient fournies par un conteneur Java tel que Payara, JBoss ou JOnAS.