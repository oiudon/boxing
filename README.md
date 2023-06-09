<h1>ボクシング適正階級AI判定</h1>
<img src="https://user-images.githubusercontent.com/125285302/226239070-d52120b1-070f-48c0-877f-5a7126b9bc36.jpg">
<a href="https://ongakuriron.com/boxing">ボクシング適正階級AI判定</a>
<h2>概要</h2>
<p>年齢、身長、リーチ（両腕を開いたときの左手中指先端から右手中指先端までの長さ）を入力し、<br>ボクシングの適正階級を機械学習で割り出す（分類）Webアプリケーションです。</p>
<p>このWebアプリの機械学習部分（データの準備～モデルの作成まで）をまとめました。</p>
<h2>使用言語など</h2>
<table>
  <tr>
    <th>名称</th>
    <th>説明</th>
  </tr>
  <tr>
    <td>Python</td>
    <td>プログラミング言語</td>
  </tr>
  <tr>
    <td>pandas</td>
    <td>Python用データ解析ライブラリ</td>
  </tr>
  <tr>
    <td>scikit-learn</td>
    <td>Python用機械学習ライブラリ</td>
  </tr>
  <tr>
    <td>Flask</td>
    <td>Webアプリケーションフレームワーク</td>
  </tr>
  <tr>
    <td>HTML/CSS</td>
    <td>マークアップ言語</td>
  </tr>
  <tr>
    <td>Jupyter Notebook</td>
    <td>Python用統合開発環境</td>
  </tr>
  <tr>
    <td>Visual Studio Code</td>
    <td>ソースコードエディタ</td>
  </tr>
</table>
<p>機械学習部分ではPython、pandas、scikit-learn、Jupyter Notebookを使用しました。</p>
<h2>使用方法</h2>
<ol>
  <li>年齢、身長、リーチを入力。</li>
  <li>「階級判定」ボタンを押す。</li>
</ol>
<img src="https://user-images.githubusercontent.com/125285302/226238926-3b489907-87e1-469d-a116-8e907f0a6379.jpg">
<h2>機械学習部分解説</h2>
<h3>データの準備</h3>
<ol>
  <li>ボクシング専門誌「<a href="https://www.ringtv.com/ratings/">ザ・リング</a>」の各階級ランキングトップ10に入る選手を中心にデータを収集。</li>
  <li>各選手のデータ（名前、年齢、身長、リーチ、スタイル、階級）を.csvファイルにまとめる。</li>
</ol>
<h3>前処理～学習～検証～モデル作成</h3>
<ol>
  <li>Jupyter Notebookで作成した.csvファイルをDataFrameとして読み込む。</li>
  <li>読み込んだDataFrameを特徴量（年齢、身長、リーチ）と正解データ（階級）に分割する。</li>
  <li>scikit-learnのSVM（サポートベクターマシン）で学習～検証を繰り返し、精度を上げていく。</li>
  <li>精度が確保できたらモデル（.pklファイル）として保存する。</li>
</ol>
<p>詳細は<a href="https://github.com/oiudon/boxing/blob/main/boxing.ipynb">boxing.ipynb</a>をご参照ください。</p>
