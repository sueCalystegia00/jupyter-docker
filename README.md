# Jupyter-Docker

Jupyter Notebook を VS Code の Remote Container で動かすための Docker 環境．

## 👋 How to Use

1. このリポジトリをクローンする．

2. VS Code の Remote Container で開く．

   ダイアログ or コマンドパレットから `Remote-Containers: Open Folder in Container...`を実行するか，
   VS Code 左下の`><`のアイコンから`Reopen in Container`を実行する．

3. `work`ディレクトリが作業スペースです．任意のファイルを作成し，作業してください．

## 📝 Note

1. ライブラリのインストール

   必要なライブラリは`.devcontainer/python/requirements.txt`に記述してください．

2. インタープリターの変更

   デフォルトのインタープリターは Python3 を指定していますが，
   今回利用しているイメージである jupyter/datascience-notebook には Julia も含まれているので，必要に応じてインタープリターを変更してください．

   > デフォルトのインタープリターを変更する場合は，`.devcontainer/devcontainer.json`の`"python.pythonPath"` を変更してください．
