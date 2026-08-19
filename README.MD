# M5Stopwatch Watch Case

M5Stack公式のストップウォッチ（M5Stopwatch）を腕時計として使用するための、カスタム取り付けベースの3Dモデルデータです。

---

## 📌 概要

M5Stopwatch本体に内蔵されている**磁石**と**ストラップホルダーの穴**を利用して、頑丈かつスマートに固定する設計になっています。
本体のベースデータは、M5Stack公式のハードウェアリポジトリ（[M5Stack/M5_Hardware](https://github.com/m5stack/M5_Hardware)）で公開されているSTLデータを元にリバースモデリングして作成しています。

* **ベルト幅**: 24mm
* **想定造形方式**: 光造形（SLA）
* ※光造形を想定して設計しているため、FDM（熱溶解積層方式）で出力する場合は、必要に応じて `STEP` データを改変してご使用ください。



---

## 🧲 固定方法・使用パーツ

* **マグネット**: ダイソー「超強力マグネットミニ (No.371) 直径6mm×厚さ3mm」を使用 [product link](https://jp.daisonet.com/products/4549131156621)
* 本体裏面の磁石およびストラップホルダーの固定穴を活用しています。

---

## 📂 データ構成とバリエーション

本リポジトリには、用途に合わせて `STL` と `STEP` の2種類のフォーマットを用意しています。

| モデル名 | 説明 | プレビュー(単体) | プレビュー(ASSY) |
| --- | --- | --- | --- |
| **BANDBASE1** | 初期モデルの腕時計用ベース | ![](/img/BANDBASE1.png) | ![](/img/BANDBASE1_ASSY.png) |
| **BANDBASE2** | より腕にフィットするように改良された最新モデル |  ![](/img/BANDBASE2.png) | ![](/img/BANDBASE2_ASSY.png) |
| **BASE** | バンドの取り付け部を無くしたベースモデル |  ![](/img/BASE.png) | ![](/img/BASE_ASSY.png) |

### 🎬 3Dビュー・プレビュー動画

* [BANDBASE1 動作確認用動画](/MOV/BANDBASE1.mov)
* [BANDBASE2 動作確認用動画](/MOV/BANDBASE2.mov)

---

## 📁 ディレクトリ構造

```text
m5-stopwatch-watch-case/
├── img/                  # プレビュー画像
├── MOV/                  # 3Dモデル動画
├── STEP/                 # STEPデータ（改変用）
│   ├── BANDBASE1.step
│   ├── BANDBASE2.step
│   ├── BANDBASE2A.step  (空気穴追加)
│   ├── BASE.step
│   └── StopWatch.step
├── STL/                  # 3Dプリント用STLデータ
│   ├── BANDBASE1.stl
│   ├── BANDBASE2.stl
│   ├── BANDBASE2A.stl  (空気穴追加)
│   └── BASE.stl
└── README.md

```

## 👤 作成者
- Kawacci


## 📄 ライセンス
- 本リポジトリは [MIT License](/LICENSE/LICENSE.txt) の下で公開されています。