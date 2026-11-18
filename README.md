# ComfyLauncher

基于ComfyNexus优化的ComfyUI启动器

## 功能说明

本启动器主要为AI对话新增llama-cpp-python模型支持，在不启动ComfyUI的情况下，用户可以直接在启动器中使用llama-cpp-python模型进行对话，完成本地提示词生成和skill调用。（可直接调用[ComfyUI-omni-llm](https://github.com/Qo-qiao/ComfyUI-omni-llm)中的skill来使用


## 安装说明

- 1.安装git程序(压缩包已提供)
- 2.启动ComfyLauncher.exe程序，指定git和comfyui的路径
- 3.如需使用llama-cpp-python模型进行对话，请安装[llama-cpp-python依赖](https://github.com/JamePeng/llama-cpp-python/releases),下载好适合自己硬件的版本文件后，使用ComfyLauncher安装即可


## 更新日志

### v1.2.7

* 新增显存共享开关，在环境设置-加速与架构-性能设置中开启
* 调整侧边栏排版与选项，常用站点提级显示，增加自定义站点添加功能
* 模型管理添加了常用模型目录，方便查看、编辑等操作
* 修复了一些bug，精简了启动日志输出
* 底层依赖移除了xformers检测（新版本以不需要此功能），添加了llama-cpp-python检测
* AI对话新增了llama-cpp-python模型支持，用户可以添加LLM中的模型到AI对话中使用，不需要启动comfyui就可使用（使用了ai对话，启动comfyui时，请先卸载模型，防止显存溢出造成问题），AI对话添加了上下文自动压缩、thinking开关选项功能
* llama-cpp对话支持skill功能，用户可以在对话中调用skill，并且支持skill编辑


## 致谢
* [ComfyNexus](https://github.com/Allen-xxa/ComfyNexus) @Allen-xxa
* [llama-cpp-python](https://github.com/JamePeng/llama-cpp-python) @JamePeng
* [ComfyUI](https://github.com/comfyanonymous/ComfyUI) @comfyanonymous