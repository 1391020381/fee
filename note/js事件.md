# [事件介绍](https://developer.mozilla.org/zh-CN/docs/Learn/JavaScript/Building_blocks/Events)
 1. 事件处理器属性 dom.onclick
 2. 行内事件处理器-请勿使用 <button onclick="bgChange()">Press me</button>
 3. addEventListener() 和removeEventListener()


* window.addEventListener('error')捕获资源加载错误。因为它也能捕获js运行时错误，为避免重复上报js运行时错误，此时只有event.srcElement inatanceof HTMLScriptElement或HTMLLinkElement或HTMLImageElement时才上报
* [JS错误监控总结](https://segmentfault.com/a/1190000014672384)
# 事件对象 
* 事件处理函数内部的固定指定名称的参数, event evt e。被称为事件对象,它被自动传递给事件处理函数,以提供额外的功能和信息。
# ErrorEvent
* ErrorEvent事件对象在脚本发生错误时产生,它可以提供发生错误脚本文本的文件名,以及发生错误时所在的行号等信息

* message
* filename  包含了发生错误的脚本文件的文件名
* lineno 包含了错误发生时所在的列号
* error  发生错误时抛出的Error对象



# Event.target
* 触发事件的对象（某个DOM元素）的引用。当事件处理程序在事件的冒泡或者捕获阶段被调用时,它与 event.currentTarget不同

# event.currentTarget
* Event接口的只读属性 currentTarget表示的,标识是当前事件沿着DOM触发时事件的当前目标。它总是指向`事件绑定元素`，而 Event.target则是事件触发元素。


# EventTarget.addEventListener()
* EventTarget.addEventListener()方法将指定的监听器注册到 EventTarget上,当该对象触发指定的事件时,指定的回调函数就会被执行。