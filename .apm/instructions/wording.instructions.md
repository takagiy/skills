---
description: Choose plain, established words over forced translations, paraphrases, metaphors, slang and single characters.
---

When you write chat messages, documents, commit messages, code comments, or any other text, choose words following these rules.

- If it is a concept borrowed from English (e.g. a technical term), write it in katakana or English, never as a Japanese translation.
  - Never say something like 版, 窓, 種, 層, 印, 罰, 絵, 写し, 道具, 巻物, 移行, 部品, 後ろ, 聴衆, 担い手, 助け手, 入れる.
  - Say something like バージョン, ウィンドウ, シード, レイヤー, マーカー, ペナルティ, ダイアグラム, コピー, ツール, スクロール, マイグレーション, コンポーネント, バックグラウンド, リスナー, ハンドラー, ヘルパー, インストールする.
- If it is an action used as a noun, write the kango noun (漢語), never the noun form of a native verb.
  - Never say something like 比べ, 見分け, 直し, 試し回し, 足し, 分け, 戻し, 調べ, 広げ, 知らせ, 合わせすぎ.
  - Say something like 比較, 区別, 修正, 動作確認, 追加, 分割, 復元, 調査, 拡張, 通知, 過学習.
- If it has a name (e.g. a product, a name in the code or an API), write the name as it is written; never translate or respell it.
  - Never say something like ネオビム, ギット, 錆, 箱, 空間, 自動挿入, 保持, 記憶.
  - Say something like Neovim, Git, Rust, `bounds`, `herdr.space`, `auto_insert`, `--keep`, `memory`.
- If it has an established word, write that word, never a casual paraphrase or a metaphor.
  - Never say something like 器, 値打ち, 出どころ, 作り, 機能の印, 止める合図, 残す言葉の深さ.
  - Say something like インターフェイス, 効果, データの元, ファイル構成, フィーチャーフラグ, キャンセルトークン, ログレベル.
- If it is a concept that needs explaining, explain it in full, never with a shortcut or a metaphor.
  - Never say something like 育てた図, 伸びの出どころ, 終わり.
  - Say something like `--mode grow` で生成した図, スコアを上げた変更, 作業の終了条件.
- If it is a judgment of degree, state the degree plainly, never with slang emphasis.
  - Never say something like 最強, 神, 爆速.
  - Say something like 速い, 〜より遅い, 〜に向く.
- Always write an unambiguous explanation, never a single character.
  - Never say something like 罫, 群, 谷, 裾, 首, 島.
  - Say something like ヘッダーと本文の間の罫線, 同じカードに属するリスト項目, 従来の実装では抜け出せなかった局所解, 最も遅かったフレームの描画時間, 2 つのバブルを繋ぐくびれた部分, 分割統治法を使って処理する部分グラフ.
