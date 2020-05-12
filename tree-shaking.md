https://juejin.im/post/5e85ec79e51d4547153d0738
#对 tree-shaking 的了解

虽然生产模式下默认开启，但是由于经过 babel 编译全部模块被封装成 IIFEIIFE 存在副作用无法被 tree-shaking 掉需要配置 { module: false } 和 sideEffects: false
rollup 和 webpack 的 shaking 程度不同，以一个 Class 为例子


看完懵逼，继续深入研究

IIFE 是 Immediately Invoked Function Expression 的缩写
自己理解：webpack之类的模块化打包为了避免污染全局对象，定义一个立即执行的匿名函数来包裹代码

深入研究tree-shaking 
https://segmentfault.com/a/1190000012794598
