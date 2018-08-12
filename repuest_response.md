一、req.setCharacterEncoding();

	1、请求对象的setCharacterEncoding()的方法什么时候会起到作用？
	当有请求信息接受时，比如：req.getParamer()方法接受到请求信息时setCharacterEncoding(),就会起到作用
	方法带的参数就指定那种显示的编码的类型。




二、resp.setContentType();

	1、响应对象的setContentType()方法什么时候起作用？
	当整个页面的加载时就是就会启用。


三、resp.setCharacterEncoding()

	响应对象的setCharacterEncoding()方法什么时候会起作用？
	当这个页面有打印输出流的out.Writer()方法发生时，setCharacterEncoding()才会起作用。



    列子：比如想要比英语翻译为中文，这个三个方法就如一个翻译器，方法的参数就是指定那个国家的语言。
    而请求对象则是接收时发生。开始你就要指定他是英语，响应对象的则是最后显示时，你可以用中文显示。




四、GBK与UTF-8编码的区别

	区别：1.GBK是在GB2312的基础上扩容后兼容的，GBK编码专门用来解决中文编码，不管是中英文都是双字节。
 	      2.GBK包含全部中文字符；

	      3.UTF-8编码是解决国际上字符的一种多字节编码，它是对英文8位(一个字节)，中文使用24位（三个字节）来编码
	      4.UTF-8则包含全世界所有国家需要用到的字符。
	      
	GBK缺点：要访问GBK网页，需要下载中问语言包支持。UTF-8就不存这个问题，可以直接访问。
	
	  