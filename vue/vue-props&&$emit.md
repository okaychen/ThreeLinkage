# vue组件间参数传递

![自己总结的一篇文章](https://www.cnblogs.com/okaychen/p/7674211.html)

父传子，通过prop，会使父子prop之间形成一个`单向下行绑定`，父级的prop更新会下流到子组件，但是反过来就不行。可以防止从子组件意外改变父组件状态，从而导致你应用的数据流向难以理解。

子传父，子组件通过`$emit` 传入事件名称来触发一个事件，父组件通过v-on来监听子组件实例。