# Keil 配置

## 问题：uint32_t is not a type name
解决方法：  
1. vscode，F1快捷键，打开 ```c/c++:Edit Configurations(JSON)```
2. 添加配置
```
"includePath":[
    ...,
    "C:/Keil_v5/ARM/ARMCLANG/include"
],
"defines": [
    ...,
    "USE_HAL_DRIVER",
    "__CC_ARM",
    "M030GGC1AE"
]
```