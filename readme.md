## 介绍
这个是一个UI使用 ant blazor的 blazor server 应用，并使用了blazor pro的模板页面，当然后续改写很多组件，方便了解和扩展开发。

最终目的是打造一个离线可用的blazor 开发模板平台，支持查看组件，支持查看文档，增加图标预览支持。

## 准备工作

### 1 安装dotnet
```bash
curl https://dot.net/v1/dotnet-install.sh -O dotnet-install.sh > dotnet-install.sh
chmod +x ./dotnet-install.sh 
./dotnet-install.sh --version latest
```
调整环境变量，增加到`.bashrc`或者`.zshrc`：
```bash
# dotnet 
export DOTNET_ROOT=$HOME/.dotnet
export PATH=$PATH:$DOTNET_ROOT:$DOTNET_ROOT/tools
# dotnet end
```

### 2 安装`ant design blazor` 模板
```bash
dotnet new --install AntDesign.Templates
```
## 相关了解
### net8 的渲染模式
https://learn.microsoft.com/zh-cn/aspnet/core/blazor/components/render-modes?view=aspnetcore-8.0#apply-a-render-mode-programatically

四种交互模式，默认静态，继承父组件


### vscode 找不到 dotnet命令
```bash
ln -s $HOME/.dotnet/dotnet /usr/local/bin/dotnet
```
创建一个软连接管事
