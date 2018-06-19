## 5种Js输出
1. alert('hello word');  弹窗
2. confirm('hello word'); 消息框
3. console.log('hello word'); 控制台
4. prompt('请输入银行卡号'); 输入框
5. document.write('<strong>hello word</strong>'); 输出文本
## 特殊符号转义  \ 转义符  \r回车 \n换行
## 数据类型 （字符串、数字、布尔、数组、对象、Null、Undefined）
## 数字类型 （正数、负数、小数、0xff、077，100）
## 判断数据类型 
1. typeof    (string\number\boolean\undefined\function\object)
2. a instanceof Array (返回boolean)
3. Array.isArray(a)   (返回boolean)
## Infinity -Infinity(无限大、无限小)
## Date()对象  var myDate=new Date();
1. getFullYear()   2018  
2. getMonth()      (0-11)
3. getDay()        (0-6) 0是周日
4. Date()  (Tue Jun 19 2018 11:12:35 GMT+0800 (中国标准时间)) GMT标准时间
5. getHours()   小时
6. getMinutes() 分钟
7. getSeconds() 秒
## Math对象 用于执行数学任务
1. Math.floor()/Math.ceil()/Math.round()  (向下取整，向上取整，四舍五入)
2. Math.max(x,y)/Math.min(x,y)
3. Math.pow(x,y)
4. Math.random();
## 数据类型转换
1. String(a) / a.toString()
2. Number(a) / parseInt(a) /parseFloat(a)
3. Boolean()
## 数组的方法
1. arr1.concat(arr2)   连接数组
2. join		       数组转字符串
3. slice	       截取，原数组不变  左闭右开
4. splice	       替换，删除，添加
## 字符串方法
1. indexOf   查找
2. split 字符串分隔为数组