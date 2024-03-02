
<h1>
<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/deepgram-python-demo/main/docs/cat_icon.png" height=200px align="left"/>
Deepgram Python Demo <br>
</h1>


このREADMEでは、Deepgram SDKを使用してマイクからの音声をリアルタイムで文字起こしするツールのセットアップとスクリプト実行方法を説明します。

<h2>セットアップ</h2>

Deepgramリアルタイム文字起こしツールを使用するには、まず環境をセットアップする必要があります。以下の手順に従ってください。 
1. 新しいconda環境を作成します。

```lua
conda create -n deepgram python=3.11
``` 
2. 作成したconda環境をアクティブにします。

```Copy code
conda activate deepgram
``` 
3. 必要なパッケージをインストールします。

```Copy code
pip install deepgram-sdk
pip install python-dotenv
pip install PyAudio
```

これで、Deepgram SDKと必要な依存関係がセットアップされました。
## スクリプト

このスクリプトは、マイクを入力として使用し、話されている内容から会話の洞察をリアルタイムで検出するLive API (Real-Time) Exampleです。このスクリプトを実行するには、マイクロフォンを使用するための追加のコンポーネントが正しくインストールされている必要があります。
### スクリプトの実行方法 
1. 下記のスクリプトを`main.py`などのPythonファイルにコピーします。
2. コマンドラインまたはターミナルで、スクリプトが保存されているディレクトリに移動します。 
3. 以下のコマンドを実行してスクリプトを起動します。

```css
python main.py
```
4. スクリプトが実行され、マイクからの入力がリアルタイムで文字起こしされます。録音を停止するには、コンソールでEnterキーを押します。
### スクリプトの説明 
- `DeepgramClient`を使用してDeepgram APIと通信します。
- リアルタイムAPIへの接続を管理し、マイクロフォンからの音声データを送信します。
- リアルタイムで受信した音声データの文字起こし結果をコンソールに出力します。
- 終了処理を行い、正常に処理を終了させます。

このツールを使用することで、会話や音声データをリアルタイムでテキストに変換し、新たな洞察を得ることができます。例えば、会議やインタビューのリアルタイム文字起こし、ライブイベントの字幕生成などに活用できます。
