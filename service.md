# 服务 Service
- 从服务器获取数据
- 验证用户输入
- 直接往控制台中写日志

## DI
* @Injectable() 装饰器来提供元数据 
* Angular 会在启动过程中为你创建全应用级注入器以及所需的其它注入器

## 三级Provider

* 根级
```
@Injectable({
  providedIn: 'root',
})
```

* 模块级
```
@NgModule({
  providers: [
   BackendService,
   Logger
 ],
 ...
})
```

* 组件级别
```
@Component({
  selector:    'app-hero-list',
  templateUrl: './hero-list.component.html',
  providers:  [ HeroService ]
})
```

## 有哪些内置服务？
