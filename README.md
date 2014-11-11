DesignPattern
=============

设计模式DEMO
说明：com.luulsj.www.designpattern.pattern1为设计模式的实现代码
           com.luulsj.www.designpattern.pattern1.test为对应的设计模式的测试类
=============
何为设计模式？
  每一个模式描述了一个在我们周围不断发生的问题，以及该问题的解决方案的核心。这样你就能一次又一次的使用该方案而不必做重复的劳动。
  描述为：在一定环境中解决某一问题的方案，包括三个基本元素----问题，解决方案和环境。

模式分为三种类型：
  创建模式：可以简单的理解为，使创建对象的方式看起来更牛逼，更高大上的模式。

=============
1.2014年11月10日12:07:33
单例设计模式：保证一个类只有一个实例，并提供一个访问它的全局访问点。
参考wiki:http://zh.wikipedia.org/wiki/%E5%8D%95%E4%BE%8B%E6%A8%A1%E5%BC%8F

2.2014年11月11日14:38:56
简单工厂模式
简单工厂模式的实质是由一个工厂类根据传入的参数，动态的决定应该创建哪一个产品类（这些产品类继承自一个父类或接口）的实例。
参考wiki:http://zh.wikipedia.org/wiki/%E5%B7%A5%E5%8E%82%E6%96%B9%E6%B3%95#.E7.AE.80.E5.8D.95.E5.B7.A5.E5.8E.82
用来处理在不指定对象具体类型的情况下创建对象的问题。
工厂方法模式的实质是“定义一个创建对象的接口，但让实现这个接口的类来决定实例化哪个类。工厂方法让类的实例化推迟到了子类中进行”
角色：
	工厂角色（Creator）：核心，它负责实现创建所有实例的内部逻辑。工厂类可以被外界直接调用，创建所需的产品对象。
	抽象产品角色（Product）：Creator创建的所有对象的父类，它负责描述所有实例所共有的特性。
	具体产品角色（Concrete Product）：Creator的创建目标。
note:由于简单工厂很容易违反高内聚责任分配原则，因此一般只在很简单的情况下应用。

