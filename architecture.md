# Angular 架构

- 模块(module)
- 组件(component)
- 服务(service)
- 路由(router): 一种服务

# Angular使用的特定技术
- 装饰器(decorator)
  
# Angular 模块

## Angular模块和JavaScript模块的区别和联系
* JavaScript模块用于管理和加载JavaScript文件(systemjs)
* JavaScript模块是Angular模块的基础
* Angular模块分为两种，一个根模块和对个功能模块
* NgModule 为一个组件集声明了编译的上下文环境，它专注于某个应用领域、某个工作流或一组紧密相关的能力。 NgModule 可以将其组件和一组相关代码（如服务）关联起来，形成功能单元。(比如书店)
  * 根模块
  * 路由模块
  * 购书模块
  * 后台管理模块 

# Angular 组件
* 每个 Angular 应用都至少有一个组件，也就是根组件
* 每个组件都会定义一个类，其中包含应用的数据和逻辑，并与一个 HTML 模板相关联，该模板定义了一个供目标环境下显示的视图。
* @Component() 装饰器表明紧随它的那个类是一个组件，并提供模板和该组件专属的元数据
* 组件组成
  * 模板
  * 指令
  * 数据绑定

## Angular模板
模板会把 HTML 和 Angular 的标记（markup）组合起来，这些标记可以在 HTML 元素显示出来之前修改它们。
Angular 的标记有：
* **指令**会提供程序逻辑，比如：ngIf
* **绑定标记**会把你应用中的数据和 DOM 连接在一起。 有两种类型的数据绑定
  * 属性绑定
  * 事件绑定

## Angular服务

## Angular路由
路由器会把类似 URL 的路径映射到视图而不是页面，从而实现局部刷新。


