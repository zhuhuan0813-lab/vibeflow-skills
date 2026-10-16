# VibeFlow 技能与舱盖 FFD 教程

本仓库包含两个 AI 技能，以及一套舱盖 FFD 变形与 STAR-CCM+ 批量计算教程。这个 README 是下载与使用入口；具体操作和代码说明放在 HTML 中。

## 从这里下载

- **[舱盖变形与计算：下载运行包](https://raw.githubusercontent.com/zhuhuan0813-lab/vibeflow-skills/main/canopy-ffd-starccm/%E8%BF%90%E8%A1%8C%E6%96%87%E4%BB%B6.zip)**：教程、代码备注、注释源码和示例模型都在包内。解压后打开 `project`，先读 `详细说明.html`，再双击 `开始使用.cmd`。
- **[给 AI 安装技能：下载技能包](https://raw.githubusercontent.com/zhuhuan0813-lab/vibeflow-skills/main/skills.zip)**：安装方法见下面的技能说明。
- **[下载整个仓库](https://github.com/zhuhuan0813-lab/vibeflow-skills/archive/refs/heads/main.zip)**：包含上述两部分；也可在[仓库首页](https://github.com/zhuhuan0813-lab/vibeflow-skills)点击绿色 **Code → Download ZIP**。

下载公开文件无需登录、无需安装 Git。ZIP 下载后先全部解压；HTML 下载后用浏览器打开。

## 技能说明

两个技能：飞行器设计、STAR-CCM+ 自动化。

- **[下载技能 ZIP](./skills.zip?raw=true)**
- **[下载中文 HTML 使用说明](./使用说明.html?raw=true)**：含技能安装、环境准备、路径填写模板和检查命令；下载后用浏览器打开。

解压 ZIP，将两个完整技能文件夹放进项目的 `.agents/skills/` 目录，再在 Codex 中打开项目。

可以不使用 VibeFlow。准备本次任务用到的软件，在 HTML 说明中填写路径清单后交给能执行本地命令的 AI。软件路径填到启动文件，Windows 与 WSL 分别说明；先检查环境，再验证小算例。

使用示例：

> 请使用 vibeflow-aircraft-design，根据我的模型和工况，整理建模与气动分析步骤。

> 请使用 vibeflow-starccm，检查我的仿真设置并生成批处理脚本，先不要启动计算。

本包仅含两个主技能及必要参考文件。实际计算需要相应软件、许可和项目输入；条件式引用的其他技能未打包，可按任务补充或由当前代理完成相应检查。

来源为现有 VibeFlow 技能文件，原文保留。本仓库没有另行授予开源许可；使用和再分发范围应按原提供方授权确认。

## 舱盖 FFD 与 STAR-CCM+ 教程

[打开教程目录](./canopy-ffd-starccm) · **[直接下载运行包](./canopy-ffd-starccm/运行文件.zip?raw=true)**

包含简版 HTML、代码备注、带注释源码及当前机身的已分区网格。解压后双击 `project/开始使用.cmd`，首次配置本机软件路径，再按菜单检查、变形和计算。
