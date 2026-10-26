# ZJS 中英文写作插件 1.0.0

本包把现有 `zjs-writing` 技能封装为纯技能插件。原六个技能文件逐字复制，保留 Kiterlin 的 MIT 许可；不含 MCP、应用连接、hook 或可执行脚本。

## 使用入口

- Codex 本机：已有独立技能时，可在新对话输入 `$zjs-writing`。插件目录安装与独立技能是两种入口，不必重复安装。
- ChatGPT 网页私有插件：在已启用创建功能的工作区，新建对话，`@` 选择 Plugin Creator，附上本插件 ZIP，要求导入为私有的“ZJS 中英文写作”，保持六个技能文件原文和许可。完成创建及安装后，新对话 `@` 搜索并选择插件。
- 工作区管理员 GitHub 导入：进入 **Admin > Plugins > Add > Import marketplace**。Source 填 `https://github.com/ashkanstennett-design/ZJS`；Path 留空；Branch 填 `codex/zjs-writing-v1`（或已含本包的实际分支/提交）。导入后检查结果并设置可用角色及安装策略，再以 `@` 调用。仓库结构见下。

```text
.agents/plugins/marketplace.json
plugins/zjs-writing/plugin.json
plugins/zjs-writing/skills/zjs-writing/SKILL.md
```

GitHub 推送、本机发现和网页安装分别验证。本打包结果只确认文件结构与内容完整，**未证明已创建或安装到 ChatGPT 网页端**。网页创建入口取决于账号和工作区权限；本机 marketplace 不会自动成为网页端插件。

在网页对话中选中 `@Plugin Creator` 后，可粘贴：

> 请创建并安装仅供我使用的私有插件“ZJS 中英文写作”。从 https://github.com/ashkanstennett-design/ZJS/tree/codex/zjs-writing-v1/plugins/zjs-writing 导入插件；若链接暂不可读，使用我附的 ZIP。保留技能六个原文件与 MIT 许可，不改写规则，不添加 MCP 或应用。完成后在新对话中测试 @ 调用，并明确报告创建和安装结果。

## 规则与许可

入口：[SKILL.md](skills/zjs-writing/SKILL.md)；原许可：[MIT LICENSE](skills/zjs-writing/LICENSE)；来源固定在技能内的 [source-manifest.json](skills/zjs-writing/references/source-manifest.json)。不承诺通过 AI 检测。

官方说明：[插件打包](https://developers.openai.com/plugins/build/plugins)、[网页创建与安装](https://learn.chatgpt.com/docs/build-plugins)、[GitHub 工作区导入](https://learn.chatgpt.com/docs/enterprise/plugin-management)。
