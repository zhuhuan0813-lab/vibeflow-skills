# 舱盖 FFD 与 STAR-CCM+ 简易教程

这套工具用来对示例机身舱盖生成 10 组变形方案，再通过 STAR-CCM+ 比较气动结果。这个 README 告诉你从哪里下载、下载后先做什么；详细操作和代码注释放在 HTML 中。

## 第一步：下载

**[点击这里下载运行文件 ZIP](https://raw.githubusercontent.com/zhuhuan0813-lab/vibeflow-skills/main/canopy-ffd-starccm/%E8%BF%90%E8%A1%8C%E6%96%87%E4%BB%B6.zip)**

第一次使用只需要下载这一个包，里面已经包含说明、代码备注、注释源码和示例模型。无需登录 GitHub，也无需安装 Git。

如果只想看文档，可以单独下载 [使用教程 HTML](./使用教程.html?raw=true) 或 [代码备注 HTML](./代码备注.html?raw=true)，下载后用浏览器打开。

## 第二步：全部解压

右键下载的 `运行文件.zip` → **全部解压**，打开解压后的 `project` 文件夹：

| 文件 | 用途 |
| --- | --- |
| `详细说明.html` | 先阅读：操作流程和环境准备 |
| `开始使用.cmd` | 双击打开操作菜单 |
| `代码备注.html` | 需要看实现原理时阅读 |

## 第三步：配置并运行

1. 双击 **开始使用.cmd**，首次按提示选择已安装的 Windows Python。
2. 菜单选 **5**，填写本机 STAR 和 WSL Python 等软件路径；然后选 **1 检查电脑**。
3. 检查通过后，选 **2 生成模型**；需要求解时再选 **3 开始气动计算**，完成后选 **4 查看结果**。

菜单 3 会启动 STAR 并使用计算许可；菜单 1 和 2 不求解 CFD。运行包不包含 Python、WSL、STAR 软件及许可，需按 HTML 说明准备环境。

需要同时下载仓库内的 AI 技能，可[下载整个仓库](https://github.com/zhuhuan0813-lab/vibeflow-skills/archive/refs/heads/main.zip)，或返回[仓库首页](https://github.com/zhuhuan0813-lab/vibeflow-skills)点击绿色 **Code → Download ZIP**。解压后进入 `canopy-ffd-starccm`，再解压其中的 `运行文件.zip`。

## 适用范围

默认比较原始机身与 10 组舱盖方案：50 m/s、迎角 0°、+X 来流、无旋翼，宏对应 STAR-CCM+ 2510 / 20.06.007-R8。软件、Python 环境和许可由使用者准备，几何依赖见原始脚本包的 `ffd/requirements.txt`。

本包适用于其中已分区的机身；新模型需要重新分区与验证。当前网格用于方案筛选，尚未建立网格无关性。公开版调整了软件路径缺省，未更改几何、物理参数或数值算法；本次上传没有重新运行 CFD。

