设计六大原则：开闭原则、单一原则、里氏替换原则、依赖倒置原则、接口隔离原则、迪米特法则
1、开闭原则（Open closed Principle OCP）
	对扩展开放，对修改关闭。
含义：当应用的需求改变时，在不修改实体源代码的前提下，可以扩展模块的功能，使其满足新的需求。

2、单一原则（Single Responsibility Principle SRP）
	一个类只负责一个职责，有且仅有一个引起它变化的原因。
核心：控制类的粒度大小、讲对象解耦、提高其内聚性。
优点：降低复杂度、提高可读性、提高可维护性、降低变更引起的风险。

3、里氏替换原则（Liskov Substitution Principle LSP）
	子类可以扩展父类的功能，但不能改变父类原有的功能。
	里氏替换原则主要阐述了有关继承的一些原则。
	里氏替换原则是实现开闭原则的重要方式之一。

4、依赖倒置原则（Dependece Inversion Principle DIP）
	高层模块不应该依赖底层模块，两者都应该依赖于抽象；抽象不应该依赖于细节，细节应该依赖于抽象。
	是开闭原则的基础。
核心：面向接口编程，依赖于抽象，不依赖具体。

5、接口隔离原则（Interface Segregation Principle ISP）
	每个接口中不存在子类用不到却必须实现的方法，如果不然就要将接口拆分。
	
6、迪米特法则（Law of Demeter LOD）
	一个类对于依赖的类知道的越少越好。
	只与直接朋友通讯。
	类之间只要有耦合关系，就叫朋友关系。
	耦合分为依赖、关联、聚合、组合等。
	我们称出现在成员变量、方法参数、方法返回值的类称为直接朋友，局部变量、临时变量则不是直接朋友。
	
23种设计原则分类
创建模式：工厂方法模式、抽象工厂模式、单例模式、建造者模式、原型模式。
结构性模式：适配器模式、装饰器模式、代理模式、外观模式、桥接模式、组合模式、享员模式。
行为模式：策略模式、模板方法模式、观察者模式、迭代子模式、责任链模式、命令模式、备忘录模式、状态模式、访问者模式、中介模式、解释器模式。


1、单例模式（Singleton）
	只有一个实例对象、必须有单例类自己创建实例。
	单例模式分类懒汉式和饿汉式。
优点：只需创建一个实例，减少系统开销；省去neew 操作，降低内存使用，减轻GC压力。
缺点：没有接口，扩展困难；若要扩展，需要更改原来代码，违反开闭原则；单例模式功能通常写在一个类中，若涉及不合理，容易违反单一职责。

2、工厂模式（Factory）
    工厂模式分类简单工厂模式、工厂方法模式、抽象工厂模式。
    把被创建的对象称为“产品”，把创建产品的对象称为“工厂”。
2.1、简单工厂
    若创建的产品不多，只要一个工厂类，这就是简单工厂模式。
    简单工厂创建实例的方法通常为静态方法，因此又叫做静态工厂方法。
    简单工厂模式每增加一个产品就要增加一个对应的产品类和一个具体的工厂类，


