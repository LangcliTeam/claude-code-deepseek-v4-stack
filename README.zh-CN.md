<div align="center">

# Make Claude Code 17x cheaper with DeepSeek V4

[English](./README.md) | [简体中文](./README.zh-CN.md)
</div>

<div align="left">

Claude Code 是最优秀的自主编程代理——但它的费用为每月200美元，且有使用上限。而 DeepSeek V4 Pro 在 LiveCodeBench 上得分高达96.4%，每百万输出令牌仅需0.87美元。

[Langcli](https://github.com/LangcliTeam/langcli) 是一款开源的终端交互式AI编程助手，基于泄露的Claude Code代码构建。因此，Langcli的使用方式与标准Claude Code完全一致。

本教程将使用Langcli来演示如何搭配DeepSeek V4进行编程。

## 安装

##### 快速安装 (推荐)

macOS、Linux 和 WSL 用户执行以下命令安装 Langcli：

```bash
bash -c "$(curl -fsSL https://assets.langcli.com/installation/install-langcli.sh)"
```

Windows 用户执行以下命令安装(请以Administrator身份运行Power shell)：

```cmd
cmd /c "curl -fsSL -o %TEMP%\install-langcli.bat https://assets.langcli.com/installation/install-langcli.bat && %TEMP%\install-langcli.bat"
```
> **注意**：建议安装后重启终端，以确保环境变量生效。

##### 手动安装

请确保你已安装 Node.js 20 或更高版本。如果还没安装，请到[nodejs.org](https://nodejs.org/en/download)下载和安装.
```bash
npm i -g langcli-com
```

## 快速开始

##### API Key 准备
 打开[LangRouter官网](https://langrouter.ai/)，注册一个账号，保存api-key。备注：可免费体验的。

##### 运行
```bash
# 启动Langcli
langcli

# 之后在回话中输入:
hi
```

<img title="Langcli" height=400 alt="Alt text" src="./assets/hi.png">

## 如何做到便宜17倍的呢？
DeepSeek V4 是一个组合。V4 Flash 用于快速构建原型，而 V4 Pro 用于解决复杂问题。如果问题仍未解决，可以部署 Opus 4.6。
在你编程的过程中，你可以在Langcli中，动态无缝地切换deepseek v4 flash、deepseek v4 pro 和 Claude opus 4.6等模型，
而切换模型不会导致你的上下文丢失。发挥好v4 flash 和 v4 pro的能力，可以为你节省下大量的Tokens开支。

</div>
