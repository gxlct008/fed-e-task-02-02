# fed-e-task-02-02

选择题
1、下面关于 Vue.js 的数据响应式描述正确的是：

C. Dep 对象的作用是收集依赖，每一个属性都会对应一个 Dep 对象，当属性变化时会调用 Dep 对象的 notify 方法发送通知更新视图。

答： C

2、下面关于响应式原理描述错误的是：

C. Vue.js 内部当数据变化后，直接更新真实 DOM。

答： C

简答题

1、当我们点击按钮的时候动态给 data 增加的成员是否是响应式数据，如果不是的话，如果把新增成员设置成响应式数据，它的内部原理是什么。


let vm = new Vue({
  el: '#el'
  data: {
    o: 'object',
    dog: {}
  },
  method: {
    clickHandler () {
      // 该 name 属性是否是响应式的
      this.dog.name = 'Trump'
    }
  }
})


答：
不是响应式的，因为在初始化的时候，这个成员是不存在的。
