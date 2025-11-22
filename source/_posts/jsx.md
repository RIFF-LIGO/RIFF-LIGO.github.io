---
title: JSX初步学习
date: 2025-06-22 14:34:02
tags: react
cover: 
categories: 前端基础
---
# React学习初步之jsx

初步定义：javascript和xml的结合，表示在js中写html的结构，是在react中编写UI模版的方式

![](https://cdn.nlark.com/yuque/0/2025/png/55336718/1747821263848-671391ea-d8e9-40f5-a928-65cef34eed8f.png)，红色部分就是jsx

这样的优势：

1. 既有HTML的声明式的写法又有可编程能力
2. js的语法扩展，因为浏览器本身无法识别js中的html，需要借助解析工具让浏览器识别。

#### 高频场景
1. 识别js表达式（使用大括号语法）包括
+ 字符串
+ 变量
+ 函数调用
+ 样式
2. 注意js中的语句不行（if for while等）

#### jsx实践
1. 实现列表渲染

```javascript

const list=[{name:'li',age:10},
  {name:'liu',age:12}
]
function App() {
  return (
    <div className="App">
      <ul>
        {list.map((item,index)=>{
          return <li key={index}>{'name:'+item.name+'    key:'+item.age}</li>
        })}
      </ul>
    </div>
  );
}

export default App;

```



2. 实现条件渲染
+ 通过逻辑运算符&&（）
+ 三元表达式（分支）
+ 自定义函数+ifelse语句
3. 事件绑定

```javascript
<button onClick={handleClick}>点击加一</button>
//传递自定义参数的话
<button onClick={（e）=>handleClick(name,e)}>点击加一</button>
```



