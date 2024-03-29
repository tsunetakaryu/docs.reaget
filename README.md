# docs.reaget
##自述

REAPER 社区文档开发与维护。

上线页面：docs.reaget.com

Discord 社区：https://discord.gg/zXuMNXg

服务器维护：Tee

主编：Ryusa

编译工具：Dr. Explain



## 更新计划

1. “REAPER 离线文档”将在第三期更名为“REAPER 社区文档”。
2. 优化：
   1. 文章提炼，定制化功能单独整理
3. 新增：
   1. REAPER 6 新版本常见问题答疑
   2. ASIO LINK PRO 内录方法（过时）
      1. （替代）→FL ASIO 桥接实现 OBS 等工具内录的方法
   3. 工程目录的清理
   4. 限制工程长度
   5. 通过修改工程文件实现临时禁用某个插件的方法，或安全加载模式（全插件离线打开工程）
   6. RX 外部工具的链接使用
   7. 侧链的原理及使用（by qy）
   8. 快捷键相关（如何根据功能找快捷键等，Moy 已经造了轮子）
   9. MIDI 相关（by 牧笛）



## 规则

考虑到 Dr. Explain 不是模块化编辑器，对工程文件内容的变动将会影响整个文件，如果存在两人异步操作工程文件的情况，则在提交时会出现冲突。因此考虑如下方案：

- 方案一：开放本仓库的提交权限给贡献者，贡献者提供文章的源文件（建议格式 doc, docx, markdown），并将它们投放到对应的分类目录（**raw_posts**），随后进行提交。
  Dr. Explain 编辑者拉取最新的提交，将文章源文件整合至工程文件（**project**）内，再编译成 html 文件，随后进行提交（**release**）。
  服务器管理员将更新的 html 内容更新上线。
  此方案的缺点在于编辑者需要对源文件重新排版整合到工程文件中。
- 方案二：开放提交权限、提供 Dr. Explain 软件给贡献者，贡献者通过空白工程文件以页面为单位编辑文章内容（同时自行参考排版规范），随后将页面内容导出进行提交。
  Dr. Explain 编辑者拉取最新的提交，将页面文件整合至工程文件内（可能需要一些校验工作），再编译成 html 文件，随后进行提交。
  服务器管理员将更新的 html 内容更新上线。
  此方案的缺点在于贡献者需要额外学习成本，门槛较高；Dr. Explain 软件是否支持导出导入页面也需要进行验证。

目前采用方案一。

