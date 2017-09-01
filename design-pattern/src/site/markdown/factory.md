# 工厂方法模式

> 工厂模式（Factory Pattern）是 Java 中最常用的设计模式之一。
这种类型的设计模式属于创建型模式，它提供了一种创建对象的最佳方式。

## 1 介绍

### 1.1 模式动机

> 定义一个创建对象的接口，让其子类自己决定实例化哪一个工厂类，工厂模式使其创建过程延迟到子类进行。

### 1.2 模式定义

> 工厂方法模式(Factory Method Pattern)又称为工厂模式，
也叫虚拟构造器(Virtual Constructor)模式或者多态工厂(Polymorphic Factory)模式，
它属于类创建型模式。在工厂方法模式中，工厂父类负责定义创建产品对象的公共接口，
而工厂子类则负责生成具体的产品对象，这样做的目的是将产品类的实例化操作延迟到工厂子类中完成，
即通过工厂子类来确定究竟应该实例化哪一个具体产品类。

### 1.3 适用环境

> * 1、日志记录器：记录可能记录到本地硬盘、系统事件、远程服务器等，用户可以选择记录日志到什么地方。 
> * 2、数据库访问，当用户不知道最后系统采用哪一类数据库，以及数据库可能有变化时。 
> * 3、设计一个连接服务器的框架，需要三个协议，"POP3"、"IMAP"、"HTTP"，
可以把这三个作为产品类，共同实现一个接口。

### 1.4 模式应用

> * 1、您需要一辆汽车，可以直接从工厂里面提货，而不用去管这辆汽车是怎么做出来的，以及这个汽车里面的具体实现。 
> * 2、Hibernate 换数据库只需换方言和驱动就可以。

### 1.5 优点

> * 1、一个调用者想创建一个对象，只要知道其名称就可以了。 
> * 2、扩展性高，如果想增加一个产品，只要扩展一个工厂类就可以。 
> * 3、屏蔽产品的具体实现，调用者只关心产品的接口。

### 1.6 缺点

> * 1 每次增加一个产品时，都需要增加一个具体类和对象实现工厂，使得系统中类的个数成倍增加，
在一定程度上增加了系统的复杂度，同时也增加了系统具体类的依赖。

### 1.7 模式结构

> 工厂方法模式包含如下角色：

> * AbstractProduct：抽象产品
> * ConcreteProduct：具体产品
> * AbstractFactory：抽象工厂
> * ConcreteFactory：具体工厂

### 1.8 时序图

## 2 代码分析

## 3 模式分析

> 作为一种创建类模式，在任何需要生成复杂对象的地方，都可以使用工厂方法模式。
有一点需要注意的地方就是复杂对象适合使用工厂模式，而简单对象，
特别是只需要通过 new 就可以完成创建的对象，无需使用工厂模式。
如果使用工厂模式，就需要引入一个工厂类，会增加系统的复杂度。

## 4 实例

## 模式扩展

## 总结