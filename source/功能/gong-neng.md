# 功能

这里介绍一些基本功能以及API的使用

#### 通用输入/输出 (GPIO）

系统支持8个通用GPIO ，均支持FPOTA方式将外设管脚映射到GPIO上。 

- 可配置上下拉驱动模式
- 可配置输入输出信号
- 支持FPOTA映射功能

要使用GPIO功能，首先要FPOTA方式映射GPIO口，比如映射IO13（物理外设管脚）作为普通FUNC_GPIO0普通GPIO口，可以

```
fpioa_set_function(13, FUNC_GPIO0);	
```

常用API:

gpio_init
初始化 GPIO。

#### 功能映射FPIOA

