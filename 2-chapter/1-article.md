# 第1条 用静态工厂代替构造器

对于类而言，为了让客户端获取它自身的一个实例，最传统的方法就是提供一个公有的构造器。还有一种方法，也应该在每个程序员的工具箱中占有一席之地。类可以提供一个公有的*静态工厂方法*（static factory method），它只是返回一个类的实例静态方法。下面是一个来自**Boolean**（基本类型 boolean 的装箱类）的简单示例。这个方法将boolean基本类型值装换成一个 Boolean 对象的引用：

```java
public static Boolean valueOf(boolean b) {
    return (b ? TRUE : FALSE);
}
```



