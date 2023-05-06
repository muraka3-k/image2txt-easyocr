# image2txt-easyocr

証明書関係の画像にOCR処理で文書情報を抽出

- 画像を読み込む<br>
![読み込み画像](https://user-images.githubusercontent.com/52340949/236626109-5f48eadc-0cad-4f35-840a-d231cba6a5ca.png)

- 画像の一番大きい領域の端部を検出する<br>
![端部検出](https://user-images.githubusercontent.com/52340949/236626130-fa5e8eab-8249-419a-b4ba-647a95387785.png)

- 画像の一番大きい領域で台形補正を行う<br>
![台形補正後](https://user-images.githubusercontent.com/52340949/236626145-e84654af-9e4f-4641-8a4d-55ced76c8bf1.png)

- 台形補正後の画像でOCRを実行する<br>
![OCR対象領域](https://user-images.githubusercontent.com/52340949/236626161-55fcd023-5181-4e4b-b57d-a528069cd6b5.png)


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

