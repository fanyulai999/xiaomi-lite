- start 从页面到了组件？
 页面是老板， 组件是员工 页面是由组件组成的，
 start  老板也要知道状态，Page data 
 <countdown start="{{start}}"/>

 - 组件的数据 data(内部数据) + properties(外部)
 - properties 里的 observer  接受到值改变时执行 观察者
 - 从内向外触发事件
    内： this.triggerEvent({
        "event_name",
        data
    })
    外： bind(绑定自定义事件):event_name="真正执行接受消息的函数"