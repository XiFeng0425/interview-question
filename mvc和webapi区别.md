1. mvc是建站的一种框架，倾向于返回用户的页面请求，api倾向于返回
用户数据请求
2. mvc直接继承System.Web.Mvc.Controller webapi继承
System.Web.Http.ApiController
3. MVC只能部署在IIS上，而webapi 可以寄宿在不同的宿主上，
（寄宿的本质就是利用一个具体的应用程序为WEBAPI 提供一个
运行环境，并解决请求的接收和响应的回复），如WEB HOST 
SELF HOST方式。
4. 接参数方式不一样：
mvc接口不管是get请求还是post请求都可以在方法名后面接参数形式，
或者直接接对象方式，但是webapi 接参数方式有点复杂，get请求
也可以直接在方法后面接到参数。
5. 返回结果的区别：
mvc返回System.Web.Mvc.JsonResult(return Json(model, System.Web.Mvc.JsonRequestBehavior.AllowGet))，在前段可以直接使用，
而webapi想要直接使用，需要返回JsonObject ，否则需要json.parse(obj)
转化。
