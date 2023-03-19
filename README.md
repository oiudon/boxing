<h1>ボクシング適正階級AI判定</h1>
<img src="https://raw.githubusercontent.com/oiudon/boxing/main/img-item01.jpg">
<a href="https://ongakuriron.com/boxing">ボクシング適正階級AI判定</a>
<h2>概要</h2>
<p>年齢、身長、リーチ(両腕を開いたときの左手中指先端から右手中指先端までの長さ)を入力し、<br>ボクシングの適正階級を機械学習で割り出すWebアプリケーションです。</p>
<p>このWebアプリの機械学習部分（データの用意～モデルの作成まで）をまとめました。</p>
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
<h2>使用方法</h2>
<ol>
  <li>年齢、身長、リーチを入力。</li>
  <li>「階級判定」ボタンを押す。</li>
</ol>
<img src="https://raw.githubusercontent.com/oiudon/boxing/main/img-item02.jpg">
<h2>データの用意</h2>
<ol>
  <li>ボクシング専門誌「<a href="https://www.ringtv.com/ratings/">ザ・リング</a>」の各階級ランキングトップ10に入る選手を中心にデータを収集。</li>
  <li>各選手のデータ(名前、年齢、身長、リーチ、スタイル、階級)をcsvファイルにまとめる。</li>
</ol>
<h2>前処理～学習～検証～モデル作成</h2>
<ol>
  <li>Jupyter Notebookで作成したcsvファイルをDataFrameとして読み込む。</li>
  <li>読み込んだDataFrameを特徴量（年齢、身長、リーチ）と正解データ（階級）に分割する。</li>
  <li></li>
</ol>
