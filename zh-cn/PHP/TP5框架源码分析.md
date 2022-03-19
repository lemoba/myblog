## TP5框架源码分析

> 获取源码：composer create-project topthink/think=5.1.* tp5
>
> 文档地址：[地址](https://www.kancloud.cn/manual/thinkphp5_1/353946)

## 一、类的自动加载

### 1. spl_autoload_register

**说明**：

```php
spl_autoload_register([ callable $autoload_function[, bool $throw = true[, bool $prepend = false]]] ) : bool
```

**参数**

- `autoload_function`

  欲注册的自动装载函数。如果没有提供任何参数，则自动注册 autoload 的默认实现函数[spl_autoload()](mk:@MSITStore:C:\Users\Administrator\Desktop\doc\php_manual_zh.chm::/res/function.spl-autoload.html)。       

- `throw`

  此参数设置了 `autoload_function` 无法成功注册时，spl_autoload_register()是否抛出异常。       

- `prepend`

  如果是 true，**spl_autoload_register()** 会添加函数到队列之首，而不是队列尾部。 

**返回值**

成功时返回 `TRUE`， 或者在失败时返回 `FALSE`。 