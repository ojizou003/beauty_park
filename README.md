# Beauty Park Scraper

美容院検索サイト [Beauty Park](https://www.beauty-park.jp/) の情報をスクレイピングするためのツールです。

## 概要

このプロジェクトは、Beauty Parkサイトから以下の情報を収集します：

1. 都道府県ごとのURLリスト
2. 市区町村ごとの美容院URLリスト
3. 各美容院の詳細情報

## 構成

- `00_selenium_sample.ipynb` - Seleniumを使用した基本的なスクレイピングのサンプル
- `01_get_district.ipynb` - 都道府県のURLを取得するノートブック
- `02_get_shop_url_list.ipynb` - 市区町村ごとの美容院URLリストを取得するノートブック
- `03_get_shop_list.ipynb` - 各美容院の詳細情報を取得するノートブック
- `district_urls.pkl` - 取得した都道府県URLのキャッシュ
- `memo.md` - 開発メモ

## 使用技術

- Python 3.13+
- Selenium - Webブラウザの自動操作
- BeautifulSoup4 - HTMLのパース
- pandas - データ処理
- requests - HTTPリクエスト
- tqdm - プログレスバー

## インストール

```bash
# uvを使用
uv sync

```

## 使い方

1. `01_get_district.ipynb` を実行して都道府県のURLを取得
2. `02_get_shop_url_list.ipynb` を実行して美容院URLリストを取得
3. `03_get_shop_list.ipynb` を実行して各美容院の詳細情報を取得

## 注意事項

- サイトのサーバーに負荷をかけないよう、適切な待機時間を設けてください
- 利用規約を遵守し、スクレイピングの頻度に注意してください
- 取得したデータの利用は個人の責任において行ってください

## ライセンス

このプロジェクトはMITライセンスの下で提供されています。