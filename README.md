# JupyterLab_JupyterAI_Course
**JupyterLab是Jupyter Notebook的更新版本，是一个面向Python数据科学和机器学习领域的轻量级IDE了，并且有现代AI编程助手的加持！！！**

## 安装 JupyterLab 和 JupyterAI
[https://github.com/jupyterlab/jupyter-ai?tab=readme-ov-file](https://jupyter-ai.readthedocs.io/en/v2/users/index.html)

```bash
用管理员进入powershell
pip install jupyterlab~=4.0

pip install 'jupyter-ai[all]' 或者
pip install jupyter-ai langchain-openai langchain-ollama

运行
jupyter lab
```
**如此安装完以后cell无法像后面课程一样拖拉到对话框（但可以使用“send message with selection”基本等价，可能有些东西还没装或者版本比较老）**，更详细的情况见后记<BR>

## 配置JupyterAI的模型
点击JupyterAI窗口的右上角的配置按钮，按下图配置（使用 https://gptgod.online/  miclub01@outlook.com账户登录
<img width="625" height="854" alt="image" src="https://github.com/user-attachments/assets/7e0b8ed3-c502-4469-ab70-3da0f14f958b" />

## Curriculum
### 1. Andrew Ng's introductory class on deeplearning.ai is 45min
- https://www.deeplearning.ai/short-courses/jupyter-ai-coding-in-notebooks/   （需Google账号登录一下，后续就不需要特别网络环境了）
- https://www.bilibili.com/video/BV1oxkQB1ENT 中文配音版

## 其他选择

### 2022年成立公司的https://marimo.io/ 完全开源项目，号称下一代Python Notebook （也有工具可convert ipynb文件用以兼容）
marimo feels like a notebook but is stored as pure Python program that's Git-friendly, reusable as a module, executable as a script, shareable as an app, reproducible in execution and packaging, and designed for data (with SQL and LLM support built-in). <BR>
- 可复现性（notebook隐变量等过于随意）
- 可交互性（有**前端设计**）
- 可重用性
  - 可控版本（因为是纯.py，所以**Git友好**）
  - 可分享发布（成**web应用**）
- **后端数据库**和AI友好

JupyterLab 在短期内仍将是主流，因为已有广泛安装基础、社区认知强、生态丰富，即**传统数据探索、教学、科研，JupyterLab 还是稳定可靠的选择**。但在中长期（尤其当**数据科学／ML／AI 的生态更多偏向生产部署、版本控制、可复用、团队协作**） 的话，marimo 有很强的潜力进入 “主流选择之一”，甚至在某些细分场景（比如 AI／ML 原型到部署的流程）中可能逐渐占据优势。

## 后记：之前用conda安装有点小问题，虽然不影响使用。
```bash
用管理员运行Conda 命令行
conda install -c conda-forge jupyterlab

conda install conda-forge::jupyter-ai conda-forge::langchain-openai conda-forge::langchain-ollama
运行
jupyter lab
```
**如此安装完以后cell无法像后面课程一样拖拉到对话框（但可以使用“send message with selection”基本等价，可能有些东西还没装或者版本比较老），后来问了AI运行了”pip install -U jupyter-ai-jupyternaut”命令后安装了一些新东西后启动有问题后面又“pip uninstall jupyter-ai-jupyternaut”了，启动正常了，但也留下了2个chat窗口其中一个已经可以把cell拉进对话框了。但后来发现没地方配Model了，所以放弃！**
