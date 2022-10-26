# <center> JavaScript

## 组成

- ECMAScript  
- 文档对象模型（DOM）  
- 浏览器对象模型（BOM）

## 书写位置

- 内部式

```JavaScript
   <script>
      console.log("hi")
   </script>
```

- 外部式

```JavaScript
   <script src="example.js"></script>
```

- 内联式

```JavaScript
   <button onclick="alert('welcome')">点击</button>

   <a href="javascript: alert('welcome') ;">点击</a>
```

## ECMAScript

### 注释

- 单行注释

```JavaScript
   <script>
      // 单行注释
      // 快捷键：Ctrl + /
   </script>
```

- 多行注释

```JavaScript
   <script>
      /* 多行注释 */
      /* 快捷键：Alt + Shift + A */ 
   </script>
```

### 变量

- var

```JavaScript
   <script>
      // 声明变量
      var message
      console.log(message)

      // 初始化变量
      message =   'hi'
      console.log(message)

      // 更新变量
      message = 'world'
      console.log(message)

      // 重复声明(正确，不推荐)
      var message = 'hi'
      var message = 'world'
      console.log(message)
   </script>
```

- let

```JavaScript
   <script>
      // 亦可声明同时赋值
      let myName = 'Bob'
      console.log(myName)

      // 声明多个变量（初始化可选）
      var myAge = 18,
          myName = 'Bob',
          message = 'hi'

      console.log(myAge)   
      console.log(myName)
      console.log(message)

      // 重复声明（错误）
      let myName = 'Bob'
      let myName = 'Chris'
      console.log(myName)
   </script>
```

- const

```JavaScript
   <script>
      // 声明即赋值(要求)
      const myAge = 18;
      console.log(myAge)
   </script>
```

- 命名规则

```JavaScript
   1. 禁止以数字开头

   2. 禁止使用关键字以及保留字

   3. 由数字、字母、下划线（_）或美元符号（$）组成
```

- 命名规范

```javascript
   1. 命名语义化

   2. 驼峰命名法
```

<!-- // 没有var也可以声明变量（不推荐）仅声明，不赋值
// 可以先使用再声明（不合理）

// 5.1var声明（ECS6之前）
// 没有块级作用域
// #### 5.2let声明
// 有块级作用域 -->

### 数据类型

- 基本数据类型

```JavaScript
   <script>
      // Number


      // String


      // Boolean


      // Undefined


      // Null


      // BigInt


      // Symbol

   </script>
```

- 引用数据类型

```JavaScript
   <script>
      // Object

   </script>
```

- 类型检测

```JavaScript
- typeof 操作符
- 因为 ECMAScript 的类型系统是松散的，所以需要一种手段来确定任意变量的数据类型
 "undefined"表示值未定义；
 "boolean"表示值为布尔值；
 "string"表示值为字符串；
 "number"表示值为数值；
 "object"表示值为对象（而不是函数）或 null；
 "function"表示值为函数；
 "symbol"表示值为符号。
调用typeof
null 返回的是"object"。这是因为特殊值 null 被认为是一个对空对象的引用。
```

- 类型转换

```JavaScript
   // 隐式转换（经验总结）

#### 隐式转换为字符串

+号两边只要有一个是字符串，都会把另外一个转成字符串


  //数字+'' 隐式转换为字符串（数字+空字符串）
  2+'3'
  //输出23

#### 隐式转换为数字类型
  
除了+以外的算术运算符 比如 - * / 等都会把数据转成数字类型

//字符串隐式转换为数字类型
//字符串 -0 
//字符串*1
//字符串/1
  
  +'2'
  //输出2 数据类型为Number
  10+ +'3'
  //输出13,+空格+表示前面的数据加一个正数

   // 显式转换

#### 2.1转换为数字型

- Number(数据) 转成数字类型
- 如果字符串内容里有非数字，转换失败时结果为 NaN（Not a Number）即不是一个数字
- NaN也是number类型的数据，代表非数字
- parseInt(数据)  只保留整数 parseInt可以将以数字开头的字符串转换成开头的数字
- parseFloat(数据) 可以保留小数

#### 2.2转换为字符型:

- String(数据) 
- 变量.toString(进制)

#### 2.3转换为布尔型

Boolean

除了 0 ,''（空字符串）,null ,undefined,NaN其余转换为布尔值都是true

### 加号特别注意

- 如果+号左右只有一个值  解析的结果是正号 可用于隐式转换
- 如果两边都是数值(Number)类型 则是+号运算符
- +号的左右如果有一个数据是字符串数据类型的话  那么这个+号会被解析成连接符
- 数字相加  字符相连
```















































<!-- 
### 关键字

### 保留字

### 标识符

### 结束符
代表语句结束
英文分号 ;
可写可不写（现在不写结束符的程序员越来越多）
换行符（回车）会被识别成结束符 ,所以一个完整的语句，不要手动换行
因此在实际开发中有许多人主张书写 JavaScript 代码时省略结束符
但为了风格统一，要写结束符就每句都写，要么每句都不写

### 字面量
在计算机科学中，字面量是在计算机中描述事/物
例如：1000 就是 数字字面量， []是数组的字面量，{}是对象的字面量，‘hi’字符串字面量
 -->

<!-- IE、Firefox、Safari、Chrome 和 Opera

开发工具
vscode atom webstrom
浏览器
| chrome |
Firefox，safarl,le,opera
解析引擎

标准库对象（内置对象） -->

## DOM

## BOM
