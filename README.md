# WEBDevelopment
WEB Development Study

# ES6
## 变量
1.var变量重复定义不报错；没有块级作用域；不能限制修改
新的ES6中规定使用：
let   定义变量
const 定义常量
可以有块级定义


2.函数＋参数
  箭头函数－－简写：
  1.只有一个参数，可以省略圆括号
  2.只有一个语句，还是return可以省略｛｝
  3.参数扩展－－剩余参数 ...arg
  4.展开数组 ...arg = 12,5,18

3.数组
  map     映射  ［31，56，87，19］＝》［不及格，不及格，及格，不及格］
  ```JavaScript
  arr.map(item=>item*2);
  ```
  reduce  汇总  ［...,...,...,...］=> xx
  ```JavaScript
  arr2 = arr.reduce((temp,item,index)=>{
    if (index < arr.length)
    {
      return temp+item;
    }
    else {
      return (temp+item)/arr.length;  

    }
  });
  ```


  filter  过滤  
  ```JavaScript
  arr2 = arr.filter(item=>item%2);
  ```

  forEach 迭代、遍历
  ```JavaScript
  arr.forEach((item,index)=>{
    alter(`第${index}是${item}`);
  });
  ```



  4.字符串
    字符串模版，可以在字符串中放一个变量和原样输出

  5.面向对象
    引入了class来定义类;super;extends
```JavaScript
  class User{
    constructor(name,pass){
      this.name = name;
      this.pass = pass;
    }

    login(){
      alert("登录成功");
    }
  }

  class VIPUser extends user{
    constructor(name,pass,level){
      super(name,pass);
      this.level = level;
    }

    download(){
      alert("下载");
    }
  }


  let v = new VIPUser("blue",'aaaa',4);

  alter(v instanceof User);

```


6.promise   是专门用来解决异步操作

  同步－－只有操作完事了，才可以往下执行；一次只能做一个事
  异步－－这个操作进行中，其他操作也能开始；一次可以做多个事
  异步的优势：
  a.用户体验好
  b.高效

  同步的优势：简单
  创建Promise对象，然后使用Promise对象
```JavaScript
let p = new Promise(function(resolve,reject){
  $.ajax({
    usl:'data/1.txt',
    dataType : 'json'
  })
})
```


---------------------------------------------------------------
MarkDown--个人简介
读一下每个开源许可证的内容，并写一个总结。
https://www.codewars.com
4.注册github账号
5.编译babel（研究一下如何编译ES6）
---------------------------------------------------------------

1.ES6和ES7收尾
2.模块化
