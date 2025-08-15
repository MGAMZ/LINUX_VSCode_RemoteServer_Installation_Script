# Define VSCode Version
# Please change this config according to your requirements.
commit_id="360a4e4fd251bfce169a4ddf857c7d25d1ad40da"

if [ ! -f ~/vscode-server-linux-x64.tar.gz ]; then
    wget https://vscode.download.prss.microsoft.com/dbazure/download/stable/${commit_id}/vscode-server-linux-x64.tar.gz -O ~/vscode-server-linux-x64.tar.gz
fi
if [ ! -f ~/vscode_cli_alpine_x64_cli.tar.gz ]; then
    wget https://vscode.download.prss.microsoft.com/dbazure/download/stable/${commit_id}/vscode_cli_alpine_x64_cli.tar.gz -O ~/vscode_cli_alpine_x64_cli.tar.gz
fi

# Extract the first package
# Folder: vscode-server-linux-x64
tar zxf ~/vscode-server-linux-x64.tar.gz -C ~/
# Extract the second package
# File: code
tar zxf ~/vscode_cli_alpine_x64_cli.tar.gz -C ~/

# mv 1.1 cli
mkdir -p ~/.vscode-server/cli/servers/Stable-${commit_id}/
cp -r ~/vscode-server-linux-x64 ~/.vscode-server/cli/servers/Stable-${commit_id}/
mv ~/.vscode-server/cli/servers/Stable-${commit_id}/vscode-server-linux-x64 ~/.vscode-server/cli/servers/Stable-${commit_id}/server
echo "1.1 Done."

# mv 1.2 bin
mkdir -p ~/.vscode-server/bin/
mv ~/vscode-server-linux-x64 ~/.vscode-server/bin/
mv ~/.vscode-server/bin/vscode-server-linux-x64 ~/.vscode-server/bin/${commit_id}
echo "1.2 Done."

# mv 2
mv ~/code ~/code-$commit_id
mv ~/code-$commit_id ~/.vscode-server/
echo "2 Done."

# clean
rm -f ~/vscode-server-linux-x64.tar.gz
rm -f ~/vscode_cli_alpine_x64_cli.tar.gz
