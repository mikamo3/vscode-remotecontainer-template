# vscode-remotecontainer-template

## 概要

vscodeのremotecontainerのtemplate
.devcontainerディレクトリに配置するDockerfile devcontainer.ymlをテンプレートより作成する

## 使い方

プロジェクトのルートディレクトリで以下を実行する

```bash
gendevcontainer templatename [projectname]  
```

実行すると
ルートディレクトリに指定したtemplatenameの内容で
.devcontainerディレクトリを作成し、Dockerfile devcontainer.ymlを配置する

projectnameを省略した場合、basedirよりprojectnameを自動設定

*.template内の`%PROJECTONAME%`は`projectname`で置換される

すでに.devcontainerディレクトリがカレントディレクトリに存在する場合、テンプレートの作成は行わない(ディレクトリの中身まではチェックしない)
