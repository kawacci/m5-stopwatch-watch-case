# M5Stopwatch Watch Case

[English](./README-EN.MD) | **日本語**

M5Stack公式のストップウォッチ（M5Stopwatch）を腕時計として使用するための、カスタム取り付けベースおよびプロテクターの3Dモデルデータです。

---

## 📌 概要

M5Stopwatch本体に内蔵されている**磁石**と**ストラップホルダーの穴**を利用して、頑丈かつスマートに固定する設計になっています。
本体のベースデータは、M5Stack公式のハードウェアリポジトリ（[M5Stack/M5_Hardware](https://github.com/m5stack/M5_Hardware)）で公開されているSTLデータを元にリバースモデリングして作成しています。

* **ベルト幅バリエーション**: 20mm / 22mm / 24mm
* **想定造形方式**: 光造形（SLA）を基本として設計していますが、FDM（熱溶解積層方式）でも出力可能です（FDMの場合は必要に応じて `STEP` データを改変してご使用ください）。

---

## 🧲 固定方法・使用パーツ

* **マグネット**: ダイソー「超強力マグネットミニ (No.371) 直径6mm×厚さ3mm」を使用 [product link](https://jp.daisonet.com/products/4549131156621)
* 本体裏面の磁石およびストラップホルダーの固定穴を活用しています。

---

## 📂 データ構成とバリエーション

本リポジトリには、用途に合わせて `STL` と `STEP` のフォーマットを用意しています。

### 1. タフギア風プロテクターモデル（Gシリーズ）

タフなデザインを取り入れた、スナップフィット式のプロテクター付きモデルです。

#### 🔹 アシンメトリー（オフセット）モデル ★NEW
ケースの大型化に伴う「手の甲への干渉」を防ぐため、ラグ（ベルト固定部）の位置を左右に逃がしたオフセット設計モデルです。装着する腕や手の甲の動きに合わせて `L`（左オフセット）/ `R`（右オフセット）を選択できます。

| モデル名 | 説明 | プレビュー |
| :--- | :--- | :--- |
| **BANDBASE-G-Offset**<br>`BANDBASE-SIDE[20/22/24]_[L/R].stl` | 手の甲への干渉を防止するアシンメトリーベース<br>（ベルト幅: 20/22/24mm × L/R 各6種） | <img src="img/BANDBASE-G-24mm_L.png" width="200" alt="BANDBASE-G-24mm_L"> |

---

#### 🔹 センターモデル（通常版）
| モデル名 | 説明 | プレビュー |
| :--- | :--- | :--- |
| **BANDBASE-G**<br>`BANDBASE-G-[20/22/24]mm.stl` | プロテクター対応の標準腕時計用ベース（各ベルト幅対応） | <img src="img/BANDBASE-G-24mm.png" width="200" alt="BASEBAND-G"> |
| **COVER-G** | M5ロゴ入りのプロテクターカバー | <img src="img/COVER-G.png" width="200" alt="COVER-G"> |
| **COVER-G-none** | ロゴ無しのプロテクターカバー | <img src="img/COVER-G-none.png" width="200" alt="COVER-G-none"> |
| **StopWatch-G (ASSY)** | プロテクター装着時の全体イメージ | <img src="img/StopWatch-G.png" width="200" alt="StopWatch-G"> |

---

### 2. スタンダードモデル・従来モデル（Original）

| モデル名 | 説明 | プレビュー (単体 / ASSY) |
| :--- | :--- | :--- |
| **BANDBASE1** | 初期モデルの腕時計用ベース | <img src="img/BANDBASE1.png" width="200" alt="BANDBASE1"> <img src="img/BANDBASE1_ASSY.png" width="200" alt="BANDBASE1_ASSY"> |
| **BANDBASE2 / 2A** | より腕にフィットするように改良されたモデル（2Aは空気穴追加版） | <img src="img/BANDBASE2.png" width="200" alt="BANDBASE2"> <img src="img/BANDBASE2_ASSY.png" width="200" alt="BANDBASE2_ASSY"> |
| **BASE** | バンドの取り付け部を無くしたベースモデル | <img src="img/BASE.png" width="200" alt="BASE"> <img src="img/BASE_ASSY.png" width="200" alt="BASE_ASSY"> |

---

## 🖨️ FDMプリント時の参考
FDM（熱溶解積層方式）で出力する場合のスライス例の一例です。必要に応じてサポートや配置を調整してください。

![FDMスライス例](img/FDM.png)

---

## 🎬 3Dビュー・プレビュー動画
* [BANDBASE1 動作確認用動画](MOV/BANDBASE1.mov)
* [BANDBASE2 動作確認用動画](MOV/BANDBASE2.mov)

---

## 📁 ディレクトリ構造

```text
m5-stopwatch-watch-case/
├── img/                  # プレビュー画像
├── LICENSE/              # ライセンスファイル
│   └── LICENSE.txt
├── MOV/                  # 3Dモデル動作確認用動画
├── STEP/                 # STEPデータ（改変・CAD編集用）
│   ├── BANDBASE1.step
│   ├── BANDBASE2.step
│   ├── BANDBASE2A.step
│   ├── BASE.step
│   ├── StopWatch.step
│   └── StopWatch_RealReverse.STEP
└── STL/                  # 3Dプリント用STLデータ
    ├── BANDBASE-G/        # プロテクター対応標準ベース（20/22/24mm）
    ├── BANDBASE-G-Offset/ # 手の甲干渉防止オフセットベース（20/22/24mm × L/R）
    ├── COVER-G/          # プロテクターカバー（ロゴあり/なし）
    └── Original/         # 初期モデル・スタンダードモデル
```

## 👤 作成者
- Kawacci


## 📄 ライセンス
- 本リポジトリは [MIT License](/LICENSE/LICENSE.txt) の下で公開されています。