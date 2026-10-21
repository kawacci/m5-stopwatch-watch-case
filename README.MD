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
* プロテクター対応版は、現時点では `STL` になっています。

### 1. タフギア風プロテクターモデル（Gシリーズ） ★NEW
某G風のデザインを取り入れた、スナップフィット式のプロテクター付きモデルです。

| モデル名 | 説明 | プレビュー |
| :--- | :--- | :--- |
| **BANDBASE-G** (20 / 22 / 24mm) | プロテクター対応の腕時計用ベース（各ベルト幅対応） | ![BANDBASE-G](img/BANDBASE-G-24mm.png) |
| **COVER-G** | M5ロゴ入りのプロテクターカバー | ![COVER-G](img/COVER-G.png) |
| **COVER-G-none** | ロゴ無しのプロテクターカバー | ![COVER-G-none](img/COVER-G-none.png) |
| **StopWatch-G (ASSY)** | プロテクター装着時の全体イメージ | ![StopWatch-G](img/StopWatch-G.png) |

---

### 2. スタンダードモデル・従来モデル

| モデル名 | 説明 | プレビュー (単体 / ASSY) |
| :--- | :--- | :--- |
| **BANDBASE1** | 初期モデルの腕時計用ベース | ![BANDBASE1](img/BANDBASE1.png) ![BANDBASE1_ASSY](img/BANDBASE1_ASSY.png) |
| **BANDBASE2 / 2A** | より腕にフィットするように改良されたモデル（2Aは空気穴追加版） | ![BANDBASE2](img/BANDBASE2.png) ![BANDBASE2_ASSY](img/BANDBASE2_ASSY.png) |
| **BASE** | バンドの取り付け部を無くしたベースモデル | ![BASE](img/BASE.png) ![BASE_ASSY](img/BASE_ASSY.png) |

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
├── MOV/                  # 3Dモデル動画
├── STEP/                 # STEPデータ（改変用）
└── STL/                  # 3Dプリント用STLデータ

```

## 👤 作成者
- Kawacci


## 📄 ライセンス
- 本リポジトリは [MIT License](/LICENSE/LICENSE.txt) の下で公開されています。