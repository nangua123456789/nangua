## JS错误类型：
### 类型错误：
TypeError：guessSubmit.addeventListener is not a function”（类型错误：guessSubmit.addeventListener 不是函数）指什么不是函数。就是可能是某一个命令写错了
    
### 语法错误：
TypeError：git is null;什么什么为空

### 逻辑错误：
	
SyntaxError: missing ; before statement（语法错误：语句缺少分号）    
  
SyntaxError: missing ) after argument list（语法错误：参数表末尾缺少括号）   
  
SyntaxError: missing : after property id（语法错误：属性ID后缺少冒号）    
  
SystaxError: missing } after function body、（语法错误：函数体末尾缺少花括号）    
  
SyntaxError: unterminated string literal（语法错误：字符串字面量未正常结束）
	
### 变量类型：
Number、String、Array、Object、Boolean
### 数字类型：
整数、浮点数、双精度   

二进制 — 计算机的最基础语言—— 0 和 1   
    
八进制 — 基数8，每列使用0-7   
    
十六进制 — 基数16，每列使用0-9，然后使用a-f。 在CSS中设置颜色时，可能会遇到这些数字。   
    
### 字符串方法：
length: 获取字符串长度   

indexOf(str,n)从n开始搜索一个str，并将搜索的索引值返回   
    
charAr()返回指定索引位置的字符   

concat(n.m)合并字符串   

slice(n,m)返回字符串n到m之间位置的字符串

substring(n,m)返回从n开始的m的字符串   

toLowerCase()和toUpperCase()转换大小写

### 数组方法：
length属性：获取数组长度   

####方法：
push():向数组最后添加数组   

pop()删除最后的数组   

unshift():向数组头部添加数据  

shift():删除数组第一个元素  

concat():将两个数组合并

reverse()对数组进行倒序处理

join（）将数组转换为字符串

splice（）删除、修改或向数组中添加数据

### 事件机制：
addEventListener('事件',function) 创建事件；   

removeEventListener('事件'删除的函数)

##　获取数据
###　API

什么是API：应用程序接口（API，Application Programming Interface）是基于编程语言构建的结构，使开发人员更容易地创建复杂的功能。它们抽象了复杂的代码，并提供一些简单的接口规则直接使用。
API分为两种：浏览器API内置于Web浏览器中，能从浏览器和电脑周边环境中提取数据，用来做有用的复杂的事情；　还有第三方API两种
API如何工作：不同的JavaScript API以稍微不同的方式工作，但通常它们具有共同的特征和相似的主题。它们是基于对象的，API使用一个或多个 JavaScript objects 在您的代码中进行交互，这些对象用作API使用的数据（包含在对象属性中）的容器以及API提供的功能（包含在对象方法中）。

### 从服务器获取数据
注意：
在早期，这种技术被称为注意：在早期，这种通用技术被称为Asynchronous JavaScript and XML（Ajax）， 因为它倾向于使用XMLHttpRequest 来请求XML数据。 但通常不是这种情况 (你更有可能使用 XMLHttpRequest 或 Fetch 来请求JSON), 但结果仍然是一样的，术语“Ajax”仍然常用于描述这种技术。

###　基本AXAJ请求：
XMLHttpRRequest
Fetch
Fetch API基本上是XHR的一个现代替代品——它是最近在浏览器中引入的，它使异步HTTP请求在JavaScript中更容易实现，对于开发人员和在Fetch之上构建的其他API来说都是如此。
关于promises 
当你第一次见到它们的时候，promises会让你有点困惑，但现在不要太担心这个。在一段时间之后，您将会习惯它们，特别是当您了解更多关于现代JavaScript api的时候——大多数现代的JavaScript api都是基于promises的。
例子（这就是promises 的基本样子）：fetch(url).then(function(response) {
  response.text().then(function(text) {
    poemDisplay.textContent = text;
  });
});

