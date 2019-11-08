# ThreeJS_Example
ThreeJS 使用 WEB-GL 来构建 3D web 场景的前端框架库。什么是threejs，很简单，你将它理解成three + js就可以了。three 表示 3D 的意思，js 表示 javascript 的意思。那么合起来，three.js 就是使用javascript 来写 3D 程序的意思。一言以蔽之，它能写出在浏览器上流畅运行的3D程序。

### 1，2 章
ThreeJS 中有三大组件。我们需要3个组建：场景（scene）、相机（camera）和渲染器（renderer）。有了这三样东西，才能将物体渲染到网页中去。

### 3 章
如果我们改变了物体的位置或者颜色之类的属性，就必须重新调用render()函数，才能够将新的场景绘制到浏览器中去。不然浏览器是不会自动刷新场景的。
为了实现循环，我们需要javascript的一个特殊函数，这个函数是requestAnimationFrame。
调用requestAnimationFrame函数，传递一个callback参数，则在下一个动画帧时，会调用callback这个函数。


**性能监视器Stats**

在Three.js中，性能由一个性能监视器来管理，它的介绍在https://github.com/mrdoob/stats.js 可以看到。
- 其中FPS表示：上一秒的帧数，这个值越大越好，一般都为60左右。
- MS表示渲染一帧需要的毫秒数，这个数字是越小越好。再次点击又可以回到FPS视图中。

使用动画引擎Tween.js来创建动画