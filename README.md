Lab-2
=====

Лабораторная 2
====
**Дата последней сдачи 21.10.2013**

ПРАКТИЧЕСКОЕ ЗАДАНИЕ №2
----
**Цель работы.**  
Познакомиться с технологией распределенных объектов на основе системы .NET Remoting.

**Краткие теоретические сведения.**  
Технология .NET Remoting является реализацией распределенных объектно-ориентированных систем на базе фреймворка Microsoft .NET (подобные технологии: CORBA, Java RMI).  
.NET Remoting позволяет приложению создать объект (именуемый remotable object) расположенный внутри процесса приложения; другом процессе, исполняющемся на этом компьютере или даже на другом компьютере, соединённом сетью.  
На стороне клиента любые запросы к удалённому объекту направляются средой выполнения .NET Remoting через объекты Channel, являющиеся обёрткой для средств транспортного уровня, таких как потоки TCP, потоки HTTP и именованные каналы. В результате, запросы к удаленным объектам для клиентского кода ничем не отличаются от локальных вызовов. Среда выполнения сама по себе выполняет сериализацию и передачу объектов в среде между клиентским и серверным доменами приложения.  
В процессе выполнения запросов любые вызовы методов, направленные объекту, включая идентификатор метода и любые передаваемые параметры, сериализуются в байтовый поток и передаются посредством канала связи, реализованного для конкретного протокола, принимающему прокси-объекту на серверной стороне («маршализируются»).  

**Задание.**  

Разработать на языке C# клиент-серверное приложение – чат.  
Клиентская программа:  
-	позволяет пользователю указать свой ник-нейм;
-	обеспечивает интерфейс ввода текстовых сообщений;
-	обеспечивает автоматическое отображение сообщений, отправленных другими участниками чата.

Серверная программа обеспечивает получение сообщений от всех участников чата и рассылку полученных сообщений подключенным клиентам с указанием имен пользователей, отправивших сообщение. 
**Необходимо обеспечить возможность подключения нескольких клиентов к серверу чата.** 
