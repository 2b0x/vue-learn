# vue-learn
vue学习记录
---
### vue路由

```<router-link to="/home">this is button</router-link>```  `通过router-link进行跳转，类似html的a标签`

```this.$router.push({path:'/path'});```  `通过$router.push进行跳转，类似js的window.loction`

所有通过router进行跳转的页面都会在<router-view></router-view>中显示

---


### 事件

#### 鼠标事件

事件对象： ```触发：@click = "function($event)" 　　接收：function(ev){ Coding... }```  

事件冒泡：

　　阻止事件冒泡：  
  
  ```
  　　1）ev.cancelBubble = true
  
  　　2）@click.stop = "function($event)" 
  ```
  
  默认行为：

　　譬如@contextmenu默认行为是模拟鼠标右键，但在这里阻止了默认行为，即把模拟鼠标右键给取消了  
  
  ```
  　　1）ev.preventDefault()
  
  　　2）@contextmenu.prevent = "function($event)" 
  ```
  
  #### 键盘事件
  
  ```触发：@keydown = "function($event)" 　　接收：function(ev){ ev.keyCode }//获取键盘键码 ```
  
  常见键码：
  
  回车：@keyup.13 　　@keyup.enter
  
  上下左右：@keyup.up 　　@keyup.down 　　@keyup.left 　　@keyup.right
  
  ---
  
  ### 属性：v-bind绑定属性
  
  
  
