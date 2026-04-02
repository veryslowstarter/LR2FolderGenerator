# LR2 Folder Generator

LR2 プレイリスト難易度表から、RANDOM・BPM・BP（Almost Full Combo）フォルダを自動生成するツール。

## 機能

### 🎲 RANDOM フォルダ
- 難易度ごとのランダムセレクトフォルダを生成
- 全曲ランダムフォルダも同時生成可能

### 📊 BPM フォルダ
- 22段階のBPM範囲区分（0-99, 100-109, ..., 300+）
- 難易度ごとのBPMフォルダを生成
- 全曲BPMフォルダも同時生成可能

### 🎯 BP（ほぼFC）フォルダ
- ほぼフルコンボ（BP1～BP9）ごとのフォルダを生成
- minbp値でグループ分け

## 必要な環境

- Python 3.13 以上
- Tkinter（Python に付属）
- SQLite3（Python に付属）

## インストール・実行

### 方法1：直接実行（推奨）
```bash
python random_generator_gui.py
```

### 方法2：実行ファイルを使用
配布版の `LR2FolderGenerator.exe` をダウンロードして実行

### 方法3：自分でビルド
```bash
pip install pyinstaller
pyinstaller --onefile --windowed --name LR2FolderGenerator random_generator_gui.py
```

## 使用方法

1. アプリケーションを起動
2. 該当するタブ (RANDOM/BPM/BP) を選択
3. 難易度表フォルダを選択して「難易度を自動検出」
4. 必要に応じて設定を変更
5. 「生成開始」をクリック

## 対応する難易度表

- 発狂BMS難易度表
- Stella
- Dystopia / Dystopia Sub
- Overjoy / Overjoy(旧)
- BMS現代発狂譜面寄せ集め
- 縦連打コレクション
- その他、LR2 プレイリスト形式に対応した難易度表

## トラブルシューティング

### フォルダが認識されない
→ 難易度表フォルダか確認（\*.lr2folder ファイルが存在する必要があります）

### LR2 で新しいフォルダが表示されない
→ LR2 を再起動するか、JUKEBOX 機能で「すべて削除」を実行

## ライセンス

このプロジェクトはパブリックドメインです。

## 連絡先

問題報告やフィードバックは GitHub Issues までお願いします。
