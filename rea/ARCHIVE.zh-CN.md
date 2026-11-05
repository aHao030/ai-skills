# REA 源码存档说明

本目录保存 [morluto/rea](https://github.com/morluto/rea) 的固定版本源码快照。REA 通过 CLI 和 MCP 为 AI 助手提供本地二进制、应用和运行行为的逆向分析工具。

## 来源

- 原仓库：https://github.com/morluto/rea
- 分支：`main`
- 提交：`fe677f6cf9853fb12490dfb8ef23ccae3a551049`
- 软件包：`rea-agents`，版本 `6.8.0`
- 保存日期：2026-11-05（Asia/Shanghai）
- 内容：7,301 个上游文件，以及 5 个保留原始固定提交的 Git 子模块引用。
- 许可证：原作者代码采用 [MIT](LICENSE)，完整保留 [第三方声明](THIRD_PARTY_NOTICES.md) 和 `licenses/`。

## 查看与使用

从 [上游中文说明](docs/readme/README_zh.md)、[上游 README](README.md) 和 [安装文档](docs/installation.md) 开始。这里保存的是源码，存入 GitHub 不会自动安装或启用 REA。本次没有运行安装器、构建脚本或注册 MCP 服务。

上游源码保持原样，额外添加本说明和 [UPSTREAM.json](UPSTREAM.json) 记录来源。此快照不自动跟随上游更新。

## 第三方子模块

上游的 5 个第三方项目以 Git 子模块方式保存，各自的固定提交保持不变。它们的源码没有展开复制进本目录。本仓库根目录的 [`.gitmodules`](../.gitmodules) 已适配 `rea/` 前缀；本目录中的原始 `.gitmodules` 也完整保留。

需要子模块源码时，克隆 `ai-skills` 仓库后，在仓库根目录运行：

```sh
git submodule update --init --recursive -- rea/third_party
```

这个步骤会从各第三方项目的原始仓库下载固定版本源码。子模块地址和提交可在 `UPSTREAM.json` 中查看。

## 更新

更新时先比较上游提交，保留许可证、第三方声明和完整配套文件，再同步源码、子模块引用以及本仓库根目录的 `.gitmodules`。同时更新本说明和 `UPSTREAM.json` 中的版本、提交和日期。
