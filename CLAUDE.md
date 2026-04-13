# kuruma-quiz（はたらくのりもの クイズ）

## 概要
子供向けの「はたらくのりもの」クイズ＆ずかんアプリ（日本語）

## 構成
- `index.html` — メインファイル（HTML/CSS/JS全て含む単一ファイル）
- `sw.js` — Service Worker（ネットワークファースト戦略、v3）
- `manifest.json` — PWA設定
- `bgm.m4a` — BGM（はたらくくるま）
- `*.jpg` — 一部の乗り物写真（fire, bus, airplane, excavator, train, garbage）
- `icon-192.png`, `icon-512.png` — PWAアイコン

## 機能
- クイズモード: 18種類の乗り物から4択クイズ
- ずかんモード: 乗り物の情報・イラスト・音を閲覧
- スプラッシュ画面: 絵文字グリッド付きスタート画面
- BGM: はたらくくるま（連続再生）
- 効果音: 正解/不正解音（WAV blob生成）
- 乗り物固有の音（WAV blob生成）
- SVGイラスト: 全18車両
- 写真: 6枚（photoMapで管理）

## ホスティング
- GitHub Pages: tomonori2.github.io/norimono-zukan
- リポジトリ: github.com/Tomonori2/norimono-zukan

## 開発メモ
- スマホではGoogle TTS・SpeechSynthesis・乗り物音が動作しない（既知の制限）
- BGMと効果音（正解/不正解）はスマホでも動作する
- GitHubプッシュにはPersonal Access Token (classic)が必要（repoスコープ）
