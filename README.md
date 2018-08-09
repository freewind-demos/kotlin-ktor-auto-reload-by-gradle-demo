Kotlin Ktor Auto Reload Demo
============================

Reload changes automatically with [ktor](http://ktor.io).

相比在IDEA中不停Build，使用gradle体检会更好一点，推荐。

```
./gradlew run
```

打开<http://localhost:8080>能看到网站启动了，但此时还不能自动重载。

在另一个窗口：

```
./gradlew -t compileKotlin
```

这样修改Kotlin代码后，后者就会自动编译，前者就会自动重载。

然后的IDE中修改Kotlin代码，比如`call.respondText("Hello World! <change me for testing!>")`中返回的内容，然后刷新浏览器看看效果。


