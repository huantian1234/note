# 路由
### histroy对象
#### 方法
##### back()
此异步方法转到浏览器会话历史的上一页，与用户单击浏览器的 Back 按钮的行为相同。等价于 history.go(-1)。
##### forward()
异步方法转到浏览器会话历史的下一页，与用户单击浏览器的 Forward 按钮的行为相同。等价于 history.go(1)。
##### go()
通过当前页面的相对位置从浏览器历史记录（会话记录）异步加载页面。比如：参数为 -1 的时候为上一页，参数为 1 的时候为下一页。当你指定了一个越界值（例如：当会话历史记录中没有之前访问的页面时，则传参的值为 -1，那么这个方法没有任何效果也不会报错。调用没有参数的 go() 方法或者参数值为 0 时，重新载入当前页面。Internet Explorer 允许你指定一个字符串，而不是整数，以转到历史记录列表中的特定 URL。
##### replaceState()
篡改地址栏(doge)

## React实现
### 组件
#### BrowserRouter
初始化时设置state。用creatContext无限向下传递。
#### Router
通过context获取地址，与组件地址进行比对。显示正确的组件。