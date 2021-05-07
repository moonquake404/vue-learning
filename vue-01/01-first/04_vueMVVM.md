# 定义：

#### View 层：

视图层。在前端开发中通常就是 DOM 层。主要作用是给用户展示各种信息。

#### Model 层：

数据层。数据可能是固定的死数据，更多的是来自服务器，从网络上请求到的数据。
在计数器案例中就是抽取出的 obj。

#### ViewModel 层：

视图模型层。视图模型层是 View 与 Model 沟通的桥梁。
一方面实现了 Data Binding（数据绑定），把 Model 的改变实时反映到 View 中。
另一方面实现了DOM Listener，即DOM监听，当DOM发生一些事件（点击，滚动，touch等）时，可以监听到，并在需要的情况下改变对应的Data。

# 计数器的MVVM

计数器中，View是DOM，Model是抽取出来的obj，ViewModel是创建的Vue对象实例。

首先，ViewModel通过Data Binding让obj中的数据实时地在DOM中显示。

其次，ViewModel通过DOM Listener来监听DOM事件，并通过methods中的操作来改变obj中的数据。