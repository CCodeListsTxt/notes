QML 文档必须且只能包含一个根对象，根对象是 QML 文档的入口点，当 QML 文档加载时，其根对象以及内部所有子对象都会被创建并初始化。

# 对象声明

从语法上说，一个 QML 文档实际上定义了要创建的 QML 对象树。加载 QML 文档实际上就是获取该对象树的过程。

对象声明的语法为 `Type { }`，对象的属性和子对象在大括号中声明。

> ```js
> // 声明一个简单矩形对象
> Rectangle {
>     width: 640
>     height: 480
>     color: 'gray'
> }
> ```

## 子对象声明

QML 提供的对象类型都定义了 default property，通过该属性，可以在对象声明中随意嵌套子对象，并加入对象树中。
