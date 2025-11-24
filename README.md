# JupyterLab_JupyterAI_Course
## 安装 JupyterLab 和 JupyterAI
[https://github.com/jupyterlab/jupyter-ai?tab=readme-ov-file](https://jupyter-ai.readthedocs.io/en/v2/users/index.html)

```bash
用管理员进入powershell
pip install jupyterlab~=4.0

pip install 'jupyter-ai[all]'
运行
jupyter lab
```

## 配置JupyterAI的模型
点击JupyterAI窗口的右上角的配置按钮，按下图配置（使用 https://gptgod.online/  miclub01@outlook.com账户登录
<img width="625" height="854" alt="image" src="https://github.com/user-attachments/assets/7e0b8ed3-c502-4469-ab70-3da0f14f958b" />

## Curriculum
### 1. Andrew Ng's introductory class on deeplearning.ai is 45min
- https://www.deeplearning.ai/short-courses/jupyter-ai-coding-in-notebooks/   （需Google账号登录一下，后续就不需要特别网络环境了）
- https://www.bilibili.com/video/BV1oxkQB1ENT 中文配音版

## 后记：之前用conda安装有点小问题，虽然不影响使用，但不如pip install干净。
```bash
用管理员运行Conda 命令行
conda install -c conda-forge jupyterlab

conda install conda-forge::jupyter-ai conda-forge::langchain-openai conda-forge::langchain-ollama
运行
jupyter lab
```
如此安装完以后cell无法像后面课程一样拖拉到对话框（但可以使用“send message with selection”基本等价，可能有些东西还没装或者版本比较老），后来问了AI运行了”pip install -U jupyter-ai-jupyternaut”命令后安装了一些新东西后启动有问题后面又“pip uninstall jupyter-ai-jupyternaut”了，启动正常了，但也留下了2个chat窗口其中一个已经可以把cell拉进对话框了。**所以如果新装可能直接用上面文档中推荐的pip install 而不是conda install更好！**
