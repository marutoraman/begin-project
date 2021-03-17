# プロジェクト作成時に行うこと
VSCODEのプロジェクト作成後に始めに行うと良いことを紹介します。

-1 venvフォルダを作成
プロジェクトルートにて以下のターミナルでコマンドを実行してvenvフォルダを作成します。
`python -m venv venv`

-1 venvをアクティべート
以下を実行してアクティべートを行い、(venv)がターミナルの先頭に表示されることを確認します。
Windows
`. venv/scripts/activate`
Mac
`. venv/bin/activate`

-1 必要モジュールのinstall
`pip install <モジュール>`

requirements.txtファイルがある場合は
`pip install -r requirements.txt`

-1 他の方にソースコードを共有する時
以下を実行して出力されたファイルを含めて共有する
`pip freeze > requirements.txt`

-1 gitignoreファイルの作成
VSCODEの拡張機能のgitignoreをインストール（検索ワード：codezombiech.gitignore）  
Ctrl + Shift + P を押下してコマンドパレットを表示させる
gitignore と入力　➙　Add gitignore を選択 ➙　pythonと入力して選択
これでgitignoreファイルが作成され、余計な一時ファイルはgithubにpushされなくなります。
