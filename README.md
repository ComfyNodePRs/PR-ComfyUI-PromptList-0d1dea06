# ComfyUI-PromptList
ComfyUI-PromptListは、ComfyUI用のカスタムノードで、プロンプトの管理とYAMLファイルとの連携を容易にします。

## 機能

- prompts.yamlからプロンプトを読み込み、ポジティブプロンプトとネガティブプロンプトをそれぞれString形式で出力します。
- 新しいプロンプトをyamlへ書き込む
- 既存のプロンプトの修正

## インストール
[ComfyUI-Manager](https://github.com/ltdrdata/ComfyUI-Manager)をインストールしている場合
1. メインメニューのManager -> Install via Git URLの順にクリックする
2. ウインドウ上部に出てくるテキストボックスにURLを貼り付けてOKを押す  
   https://github.com/yourusername/ComfyUI-PromptList.git
3. インストールが完了したら、ComfyUIを再起動

[ComfyUI-Manager](https://github.com/ltdrdata/ComfyUI-Manager)をインストールしていない場合
1. ComfyUIのカスタムノードディレクトリに移動します。（通常は ComfyUI/custom_nodes/）
2. このリポジトリをクローンします。  
git clone https://github.com/yourusername/ComfyUI-PromptList.git
3. ComfyUIを再起動します。

## 使用方法

ComfyUIワークスペースにComfyUI-PromptListノードを追加します。
ノードには以下の入力があります：

selection: prompts.yamlのプロンプトリスト  
  
以下の項目に入力されている場合はselectionのプロンプトは出力されずにこちらのプロンプトが出力されます。  
Prompt Name: 新しいプロンプト名または更新するプロンプト名  
Positive Prompt: ポジティブプロンプトの内容  
Negative Prompt: ネガティブプロンプトの内容  
  
また、入力したプロンプト名とプロンプトはprompts.yamlに保存されます。  

## 注意事項

プロンプトリストはprompts.yamlファイルに保存されます。
編集したり新しいプロンプトを追加または編集を行った場合、変更を反映させる為にComfyUIのメインメニューにあるRefreshを押してください。

## ライセンス
このプロジェクトはMITライセンスの下で公開されています。

## その他
バグレポートや機能リクエストは、連絡が取れる手段であれば何でも構いません。
プルリクエストも歓迎します。

[NakamuraShippo](https://lit.link/admin/creator)
