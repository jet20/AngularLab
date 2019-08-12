# Angular模块

## @NgModule
* declarations: 本模块的组件(component)、指令(directive)和管道(pipe)
* providers: 本模块向全局服务中贡献的那些服务的创建器
* bootstrap —— 应用的主视图，称为根组件。它是应用中所有其它视图的宿主。只有根模块才应该设置这个 bootstrap 属性。