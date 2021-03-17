# プロジェクト作成時に行うこと
VSCODEのプロジェクト作成後に始めに行うと良いことを紹介します。

- venvフォルダを作成
プロジェクトルートにて以下のターミナルでコマンドを実行してvenvフォルダを作成します。<BR>
`python -m venv venv`<BR>

- venvをアクティべート
以下を実行してアクティべートを行い、(venv)がターミナルの先頭に表示されることを確認します。<BR>
Windows<BR>
`. venv/scripts/activate`<BR>
Mac<BR>
`. venv/bin/activate`<BR>

- 必要モジュールのinstall
`pip install <モジュール>`

requirements.txtファイルがある場合は<BR>
`pip install -r requirements.txt`<BR>

- 他の方にソースコードを共有する時
以下を実行して出力されたファイルを含めて共有する<BR>
`pip freeze > requirements.txt`<BR>

- gitignoreファイルの作成
VSCODEの拡張機能のgitignoreをインストール（検索ワード：codezombiech.gitignore）<BR>  
Ctrl + Shift + P を押下してコマンドパレットを表示させる<BR>
gitignore と入力　➙　Add gitignore を選択 ➙　pythonと入力して選択<BR>
これでgitignoreファイルが作成され、余計な一時ファイルはgithubにpushされなくなります。
