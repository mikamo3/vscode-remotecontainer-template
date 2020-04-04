# vscode-remotecontainer-template

## 概要

vscodeのremotecontainerのtemplate
.devcontainerディレクトリに配置するDockerfile devcontainer.ymlをテンプレートより作成する

## 使い方

プロジェクトのルートディレクトリで以下を実行

```bash
gendevcontainer templatename [projectname]  
```

projectnameを省略した場合、basedirよりprojectnameを自動設定

すでに.devcontainerディレクトリがカレントディレクトリに存在する場合、テンプレートの作成は行わない(ディレクトリの中身まではチェックしない)
