# 组件

## 组件生命周期

当用户在应用中穿行时，Angular 就会创建、更新、销毁一些组件。 你的应用可以通过一些可选的生命周期钩子（比如ngOnInit()）来在每个特定的时机采取行动。

## @Component

## 如何引用其他模块中的组件？
- a.module.ts
  - import b from b

## 模板
- 数据绑定
- 管道
- 指令

### 如何内联模板
```
ng g c hero -it
```

### MVVM
在 Angular 中，组件扮演着控制器或视图模型的角色，模板则扮演视图的角色。

## 数据绑定
- {{value}}: component --> dom
- [property]="value": component --> dom
- (event)="handler($event)": dom --> component
- [(ngModel)]="property": dom <--> component


### 模型类
应用代码直接在组件内部直接定义了数据。 作为演示还可以，但它显然不是最佳实践。

## 指令
- 组件从技术角度上说就是一个指令
  - 结构型指令：通过添加、移除或替换 DOM 元素来修改布局(ngIf, ngFor)
  - 属性型指令：会修改现有元素的外观或行为(ngModel, ngClass)

## 插值
```
<p>{{title}}</p>
<div><img src="{{itemImageUrl}}"></div>
```
插值其实是一个特殊语法，Angular 会把它转换为属性绑定。

## 模板表达式
{{模板表达式}}
[property]="模板表达式"

表达式上下文
- 表达式上下文就是这个组件实例
- 比如模板输入变量 (let customer)
- 模板引用变量(#customerInput)

表达式中的上下文变量是由模板变量、指令的上下文变量（如果有）和组件的成员叠加而成的，
模板变量是最优先的，其次是指令的上下文变量，最后是组件的成员

模板表达式不能引用全局命名空间中的任何东西，比如 window 或 document。它们也不能调用 console.log 或 Math.max。 它们只能引用表达式上下文中的成员。

## 模板语句
语句上下文可以引用模板自身上下文中的属性。 在下面的例子中，就把模板的 $event 对象、模板输入变量 (let hero)和模板引用变量 (#heroForm)传给了组件中的一个事件处理器方法。

## ngModelChange不起效果？
