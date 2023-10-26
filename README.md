# 我的helix设置
## 预览：
![image](https://github.com/Jysume/helix-config/assets/148839950/6daa7797-f8e5-40e2-8ac5-8d8f48dcc828)

## 一、我自己使用的helix的设置，附上几个透明的主题
直接使用版本为23.05，最近helix刚更新的23.10版本，因为`winget`和ubuntu未推送最新版本，我继续使用23.05
## 二、在helix 23.10中使用
**1、将`languages.toml`中的每一个`[[language]]`下的`language-server`更改为`language-servers`**

**2、将`language-servers`后的参数修改为数组即可**

**例：**
```tmol
[[language]]
name = "python"
diagnostic-severity = "Warning"
language-server = { command = "pylsp" }
```
**修改后**
```tmol
[[language]]
name = "python"
diagnostic-severity = "Warning"
language-server = ["pylsp","ruff"]
```
