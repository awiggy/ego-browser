# Ego Browser Skill

供 AI 助手操作 **ego lite 浏览器**的 Skill 资料与配套安装脚本。

**这不是浏览器本体，也不是独立运行的网页应用。** 仅下载这个仓库，不会自动拥有浏览器自动化能力；它依赖 ego lite 应用提供的 `ego-browser` 命令。

## 可以做什么

根据仓库中的 Skill 定义，配合所需浏览器运行环境，可用于打开网页、点击、填写表单、读取页面、截图与网页测试。具体操作接口见 [SKILL.md](SKILL.md)。

## 文件说明

| 文件 | 用途 |
| --- | --- |
| [SKILL.md](SKILL.md) | 面向 AI 助手的操作规范与示例 |
| [references/install.md](references/install.md) | ego lite 依赖、安装与初始化说明 |
| [scripts/install.sh](scripts/install.sh) | macOS 浏览器安装辅助脚本 |

## 使用前确认

1. 区分「保存 Skill 文件」与「安装浏览器运行环境」；两者不是一回事。
2. 核对 ego lite 的来源并完成应用初始化。
3. 在终端用下面的只读命令检查 CLI 是否可用：

```bash
command -v ego-browser
```

没有输出，只能说明当前终端未找到该命令；可能未安装，也可能 PATH 尚未配置。

安装说明包含下载、安装应用及调整 macOS 隔离属性的步骤。运行脚本前请自行审阅，不建议未经检查直接执行；优先遵循操作系统的安全提示。

## 来源与维护说明

本仓库是保存的 Skill 资料，不代表 awiggy 开发了 ego lite 浏览器。现有资料指向的产品地址为 <https://lite.ego.app/>；所述功能以仓库资料为依据，未在本次文档整理中进行实际运行验证。

现有版本未附独立 LICENSE；公开可见不等于获得任意再分发或商业使用授权，复用前请确认原始来源及许可。
