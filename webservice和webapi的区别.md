1. webservice是基于SOAP协议的，数据格式是xml，webapi遵循
的http协议，它的Response可以被webapi 的MediaTypeFormatter
转换成Json XML 或者任何你想转换的格式。
2. webservice只能部署在IIS上，而webapi可以寄宿在不同的宿主上
（寄宿的本质就是利用一个具体的应用程序为webapi 提供一个运行的
环境并解决请求的接收和响应的回复），如webHost SelfHost方式。
3. webservice也可以通过ajax访问，webservice在data里面必须
用参数名paraStu进行赋值，而webapi和mvc模式下是不需要的，两者
都可以直接用实体接参数。
4. webapi无状态，相对webservice更轻量级。webapi支持如get post
等http操作，并且对限制带宽的设备，比如智能手机等支持的很好。
