1.是什么检查异常

    检查异常：在Java中所有不是RuntimeException派生的Exception都是检查型异常，检查异常要求在方法里捕获或者继续抛出；

2.什么是运行时异常
	
    运行时异常：没有用throws字句声明抛出它，还会编译通过，这种异常可以通过改进代码实现。

3.异常类的继承架构
	
	运行时异常：RuntimeException
	public class 异常类名 extends RuntimeException{
		
		//构造函数
	}

4.RuntimeException和Exception的区别：
	
	1.一个是在定义方法时不需要声明的，也不需要捕获
	2.一个是在定义方法时一定要捕获或抛出异常。