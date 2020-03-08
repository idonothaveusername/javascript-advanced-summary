#《你不知道的JavaScript》中卷1、2、4章#
## 第1章  类型 ##
    //两个空格为换行
1、JavaScript有七种内置类型：  
空值（null）、未定义（undefined）、布尔值（boolean）、数字（number）、字符串（string）、对象（object）、符号（symbol，ES6中新增）   
【注：除对象外，其它统称为基本类型】  
2、`typeof null; // "object"`  
除null之外的六种类型均有同名的字符串值与之对应。
null也是基本类型中唯一一个“假值”  
3、function（函数）也是JavaScript的一个内置类型，但实际上它是object的一个子类型；具体来说，函数是“可调用对象”，它有一个内部属性[[Call]]，该属性使其可以被调用。  
函数不仅是对象，还可以拥有属性。  
length属性：该函数对象声明的参数的个数。  
4、数组不是一个特殊的类型，它也是对象，是object的一个“子类型”，数组元素按数字顺序来进行索引，其length属性是元素的个数。  
5、JavaScript中的变量是没有类型的，只有值才有。变量可以随时拥有任何类型的值。  
    `var a = 42;typeof a;//"number"      
    a = true;typeof a;//"boolean" `
     
[注：typeof 运算符总会返回一个字符串  
`typeof typeof 42；//"string"`]  
6、undefined和undeclared  
变量在未持有值的时候为undefined，此时typeof返回"undefined"，已经在作用域中声明但是还没赋值的变量；  
还没有在作用域中声明过的变量是undeclared的，此时typeof仍返回"undefined" 。  
7、变量没有类型，但它们持有的值有类型。类型定义了值的行为特征。  
## 第2章 值 ##  
2.1 数组  
`var a = [1,"2",[3]];a[2][0] === 3;//true`  
1、对数组声明后即可向其中加入值，不需要预先设定大小。  
`var a = [];`    
[注：使用delete运算符可以将单元从数组中删除，但是删除后，数组的length属性并不会发生变化]    




