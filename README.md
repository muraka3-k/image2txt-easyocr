# image2txt-easyocr

証明書関係の画像にOCR処理で文書情報を抽出

- 画像を読み込む
![読み込み画像](https://file%2B.vscode-resource.vscode-cdn.net/Users/mkstd_eczep/workspace/image2txt-easyocr/output.png?version%3D1683377534015)
- 画像の一番大きい領域の端部を検出する
![端部検出](https://file%2B.vscode-resource.vscode-cdn.net/Users/mkstd_eczep/workspace/image2txt-easyocr/output2.png?version%3D1683377569148)
- 画像の一番大きい領域で台形補正を行う
![台形補正後](https://file%2B.vscode-resource.vscode-cdn.net/Users/mkstd_eczep/workspace/image2txt-easyocr/output3.png?version%3D1683377622507)
- 台形補正後の画像でOCRを実行する
![OCR対象領域](https://file%2B.vscode-resource.vscode-cdn.net/Users/mkstd_eczep/workspace/image2txt-easyocr/output4.png?version%3D1683377628008)

# インストール手順
```
git clone https://github.com/muraka3-k/image2txt-easyocr.git
cd image2txt-easyocr
poetry install
```

poetryをインストールしていない場合は以下のコマンドでインストールしてください。
```
curl -sSL https://install.python-poetry.org | python3 -
```
そして、環境に応じて、PoetryのPATHを通してください。

# 使用ライブラリ

* jupyter notebook
* OpenCV
* EasyOCR
* lxml

手動でインストールする場合は、以下のコマンドを使用してください。
```
pip install jupyter==1.0.0
pip install opencv-python==4.5.4.60
pip install opencv-contrib-python==4.5.4.60
pip install opencv-python-headless==4.5.4.60
pip install easyocr==1.6.2
pip install matplotlib==3.7.1

```

# Run
```
poetry shell
jupyter notebook
```

#　注意事項
- 簡易的な台形補正を実施しているため、背景と読み取り対象物の色の違いがあるようにしてください。

# Author

* Github   [muraka3-k](https://github.com/muraka3-k)

