### dom查询
> $ic() // 获取节点，库所有dom方法都是根据$ic获取到dom节点后进行的
```javascript
// 页面load后执行该方法
$ic(function() {
})
// 直接复制dom
$ic(document)
// 查询所有div
$ic('div')
```

> find (expr = '*') // 根据查询子孙节点 内部使用querySelectorAll
```javascript
$ic('ul').find('li')
```

> findOne (expr) // 查询子孙中的第一个节点 内部使用querySelector
```javascript
$ic('ul').findOne('li')
```

>  children (expr = undefined) // 查询所有孩子节点(不包括孙子)，传递expr表示查找某种类型孩子
```javascript
$('body').children()
``` 

> parent (expr = undefined) // 获取直接父亲节点(亲生父亲)，传递expr表示查找某种类型的直接父亲节点
```javascript
$('li').parent('ul')
```

> parents (expr = undefined) // 获取所有祖先(父亲，爷爷..)，传递expr表示查找某种类型的祖先节点
``javascript
$('li).parents()
```

> sibling (expr = undefined) // 获取兄弟节点
```javascript
$('li').sibling('.active')
````
