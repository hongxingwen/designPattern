# 创建者模式（builder模式）


我们创建一个类，给类传参，同时设置属性，但很多属性是有条件限制，（而且我们用对象字面量的方法设置属性没法监控到如果属性改变应该做什么变化），如果都放在构造函数里面去判断的话：

* 会导致构造函数（constructor）函数特别大，增加了new的成本，
* 会增加维护的成本，这就不符合设计模式的原则了。


所以，我们应该创建另一个类，让这个类去做判断，这个类基于前面的那个类，这个类就是一个创建者，它让属性的配置变得更加灵活，并且提高了代码的可维护性。




示例：

创建一个学生的类，再创建一个创建学生的属性的类。
