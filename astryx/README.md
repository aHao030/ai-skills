# Astryx

[Astryx](https://github.com/meta/astryx) 是 Meta 开源的 React 设计系统，提供界面组件、主题、页面模板和供 AI 查询的开发工具。

- 本机已安装官方 npm 发布版 `@astryxdesign/cli@0.7.13`，并通过 `astryx init --user` 启用电脑级 AI 使用指引。
- 安装已验证，组件搜索和模板列表均能正常读取。
- [source/](source/) 完整保存上游 `main` 的 10,476 个文件，提交为 `9a3f29608e789a8de0d461bb0393f8cfde422867`，源码内的 CLI 版本标记为 `0.7.14`。
- 保存日期为 2026-11-11，时区为 Asia/Shanghai。来源和版本记录见 [UPSTREAM.json](UPSTREAM.json)。
- 原始源码及 [MIT 许可证](source/LICENSE) 完整保留。

本机可以直接查询组件、模板和设计规范。

```sh
astryx search button
astryx component Button
astryx template --list
astryx docs tokens
```

Windows PowerShell 也可以使用 `astryx.cmd` 调用。

以后开发 React 页面时，可让 AI 使用 Astryx 查找适合的组件和模板，并按 [上游接入说明](source/packages/core/README.md) 为具体项目安装组件依赖。Astryx 要求 React 19 或以上版本。

源码快照固定在上述提交。更新时同步 `source/`，保留原始许可证并更新来源记录。本机工具可以使用 `npm install --global @astryxdesign/cli@版本号` 更新。
