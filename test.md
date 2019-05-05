#第一行



##ff

```
​```
function add(a,b){
 return a+b;
}

​```
```

var list = (names) =>  names.map(x => x.name).join(', ').replace(/(.*),(.*)$/, "$1 &$2")



**function list(names)** **{**
**var** **xs = names.map(****p =>** **p.name)**
**var** **x = xs.pop()**
**return** **xs.length ? xs.join(****", "****) +** **" & "** **+ x : x ||** **""**
**}**

正则表达式语法  断言 （?=.*[a-z]）  表示至少包含一个

``````javascript
currying  function

function add(n){
  // Let the currying begin!
  var arr=[...arguments];
  var _add=function(){
  arr.push(...arguments);
  return _add;
  }

  _add.toString=function(){
    return arr.reduce((a,b) => a+b);
    }
    

return _add;

}
``````

``````
var add = function(n) {
  const f = x => add(n + x)
  f.valueOf = () => n
  return f;
}
``````
gaidong
nodemon  监视文件变动
