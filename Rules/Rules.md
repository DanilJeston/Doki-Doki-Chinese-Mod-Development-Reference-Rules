# Doki Doki Chinese Mod Development Reference Rules

## 第一章 总则

1. 为标准化中文 DDLC Mod 开发，规范中文 DDLC Mod 开发，特制定本参考规则。
2. 本规则仅供参考，开发者可根据自身需求决定是否遵守本规则。
3. 本规则仅适用于由 imgradeone 更新的中文 DDLC Mod 开发模板：[DDLCModTemplate-Chinese-future](https://github.com/DokiMod/DDLCModTemplate-Chinese-future)



## 第二章 代码

1. 由于当前中文开发模板（以下简称模板）的特殊性，为方便后续升级，所有 Mod 代码应存放在独立于模板内容的文件夹中（特殊文件夹除外，如： `python-package`）。
2. 当需要覆写原版内容时，应遵守本章第 1 条，为文件按照 Ren'Py 加载顺序<sup>1</sup>加上前缀，保证代码在原版内容后加载（GUI 界面、特殊 label 等除外）。
3. 所有 Python 代码应遵守 PEP8 风格。
4. 



## 第三章 资源

1. 为区分原版内容与 Mod 内容，所有 Mod 资源应添加前缀、后缀，或定义在 `mod` 命名空间中。
2. **原则上，Mod 中不应包含原版内容。**

---

## 附录：

注释：

1. Ren'Py 按照 Unicode 顺序加载文件，如：`1` 开头的文件优先级会对于开头为 `0` 的文件一级、`c` 开头的文件优先级会对于开头为 `a` 的文件两级。
