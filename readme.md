# VsCode 手动远程服务器安装

## 下载包

### X86平台

[下载第一个包：vscode-server-linux-x64.tar.gz](https://vscode.download.prss.microsoft.com/dbazure/download/stable/${commit_id}/vscode-server-linux-x64.tar.gz)

[下载第二个包：vscode_cli_alpine_x64_cli.tar.gz](https://vscode.download.prss.microsoft.com/dbazure/download/stable/${commit_id}/vscode_cli_alpine_x64_cli.tar.gz)

### Arm 平台

[下载第一个包](https://vscode.download.prss.microsoft.com/dbazure/download/stable/${commit_id}/vscode-server-linux-arm64.tar.gz)

[下载第二个包](https://vscode.download.prss.microsoft.com/dbazure/download/stable/${commit_id}/vscode_cli_alpine_arm64_cli.tar.gz)

## 迁移至路径

### 第一个包

使用tar zxvf解压

将解压后的文件夹`vscode-server-linux-x64`改名为`server`

放在这个路径下`~/.vscode-server/cli/servers/Stable-${commit_id}/`

### 还是第一个包

将解压后的文件夹`vscode-server-linux-x64`改名为`${commit_id}`

放在这个路径下`~/.vscode-server/bin/`

### 第二个包

将`code`改名为`code-${commit_id}`

放在`~/.vscode-server/`目录下
