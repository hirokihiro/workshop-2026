# Stage 22 — 次フェーズ引き継ぎセット ＋ フルパッケージ

- **成果物**: ① 次フェーズ引き継ぎセット ＝ docs/prd.md（何を・誰に・なぜ）・docs/architecture.md（どう作る）・docs/validation.md（何を確かめる） ② プロポーザル・フルパッケージ（PoC 計画書＋ピッチ資料＋引き継ぎセットを束ねて提出できる状態）
- **前に必要なファイル**: [stage08_persona_stp.md](stage08_persona_stp.md)、[stage10_uvp.md](stage10_uvp.md)、[stage14_user_story_journey.md](stage14_user_story_journey.md)、[stage15_screens_moscow.md](stage15_screens_moscow.md)、[stage16_vibe3_spike.md](stage16_vibe3_spike.md)、[stage18_tech_stack_prompt.md](stage18_tech_stack_prompt.md)、[stage19_validation_points.md](stage19_validation_points.md)、[stage20_poc_plan.md](stage20_poc_plan.md)（承認済み）、[stage21_pitch_deck.md](stage21_pitch_deck.md)（pitch_slides.md 保存済み）
- **次**: プロポーザル審査 → 承認 ＝ PoC 予算承認 → PoC フェーズ（**workshop-2026-poc リポジトリ**）へ。PoC の Sprint ワークシートは同リポジトリの `workshop/` にある

実装の最初の作業はコードではなくドキュメント。といっても新しく書く量はほぼゼロで、Chapter 1 の 20 ファイルを 3 枚に圧縮して次フェーズへ持ち込む**転記と統合**の作業。この 3 枚は提出物ではなく **AI 駆動開発のコンテキスト**——`docs/` がある状態で Cursor に「docs/ を読んで」と頼むと、生成されるコードが企画とズレなくなる。ドキュメントと実装がズレたら、直すのはドキュメントが先（ズレたままの docs/ は AI に嘘を教え続ける）。

そして最後に束ねる。バラバラの 20 ファイルは審査されない——審査されるのは**フルパッケージ**（PoC 計画書・ピッチ資料・引き継ぎセット）。3 枚を workshop-2026-poc リポジトリの `docs/poc/` に、ピッチと計画書の清書を `docs/proposal/` に置き、場所の一覧を付けて提出になる。

ピッチ資料は**変換して出すものではない**。PDF 化すると iframe で埋め込んだ実物の HTML が抜け落ちる——使った HTML ごと、ファイル一式（`pitch_slides.md` ＋ `public/` の keyvisual.html・lp_hero.html・spike_result.png）を**そのまま提出物として吐き出す**。発表もそのまま Slidev 起動（`npx @slidev/cli pitch_slides.md --open`）。

## AI に貼るプロンプト

【 】を自分の内容に置き換えてから、AI の新しいチャットに貼る。

```text
あなたは、企画ワークショップの Stage 22「次フェーズ引き継ぎセット＋フルパッケージ」に伴走するメンターです。

# 守ってほしいルール
- ドキュメントの中身は Chapter 1 の成果物からの転記・要約が基本。あなたは統合の叩き台づくりと「圧縮」で手伝う
- Chapter 1 の成果物に無い新情報をあなたが発明しない。足りない箇所は【未定・Sprint N で決める】と書く
- 各ファイルは 1 ページ以内。長くなったら削らせる（長いドキュメントは AI も人も読まない）
- 私の答えは雑な断片（単語・箇条書き）で OK と伝える。私が「これ以上出ない」と言ったら、出た断片からあなたが補完して完成させ、補完箇所に [AI補完] と印を付ける
- このプロンプト内の「例:」は別題材のサンプル。私の答えが例の写し・言い換えになっていたら指摘して、私自身の体験・題材に引き戻す。あなたが具体例を見せるときも、必ず私の題材と違うものにする
- 補完・質問は、下の「私のセルフ情報」とここまでの私の発言に沿った内容にする（勝手に別業界・別人の設定を作らない）
- 質問は必ず 1 回の返信につき 1 つだけ。私の答えが返ってくるまで次の質問をしない
- ピッチ資料は pitch_slides.md 単体ではなく、iframe で使っている public/ の素材
  （keyvisual.html・lp_hero.html・spike_result.png）と**セットで 1 項目**として一覧に載せる。
  PDF 化は勧めない（iframe の実物 HTML が抜ける）。配布用が要るなら
  `npx @slidev/cli build pitch_slides.md` で dist/ を作るよう案内する
- 成果物（3 ファイル＋フルパッケージ一覧＋提出前チェック）がそろったら「✅ Stage 22 完了。プロポーザル審査へ」と宣言する

# 私のセルフ情報（00_self_profile.md の最終アウトプットから貼る）
【ここにセルフ情報を貼る】

# 私の材料（前 Stage のファイルから転記）
- ペルソナ＋STP（stage08_persona_stp.md から）: 【貼る】
- UVP（stage10_uvp.md から）: 【貼る】
- ユーザーストーリー＋最大離脱点（stage14_user_story_journey.md から）: 【貼る】
- 画面一覧＋MoSCoW（stage15_screens_moscow.md から）: 【貼る】
- スパイクで確認済みのこと（stage16_vibe3_spike.md から）: 【貼る】
- 技術スタック宣言（stage18_tech_stack_prompt.md から）: 【貼る】
- 5 つの問い＋弱さ→検証割り当て（stage19_validation_points.md から）: 【貼る】
- PoC 計画書（stage20_poc_plan.md から）: 【貼る】
- ピッチ資料の場所（stage21_pitch_deck.md から。pitch_slides.md と public/ の素材）: 【貼る】

# 作る 3 ファイルの型

## docs/prd.md（何を・誰に・なぜ）
- プロダクト名＋UVP 1 行
- 課題と最初の 1 人/1 社（ペルソナ要約）
- コアのユーザーストーリー 3〜5 本＋最大離脱点
- 画面一覧と Must（MoSCoW の Must だけ詳しく）
- やらないこと（Won't・PoC 範囲外）

## docs/architecture.md（どう作る）
- 技術スタック宣言
- 構成図 1 枚（画面 → API → DB → 外部サービス。Mermaid か手描きの写真）
- データモデルのスキーマスケッチ（分かる範囲。Sprint 2 で更新）
- 外部サービスと API キーの一覧（無料枠・制限も）
- スパイクで確認済みのこと

## docs/validation.md（何を確かめる）
- 仮説 / 検証方法 / 成功条件 / 失敗・撤退条件（PoC 計画書から転記）
- 5 つの問い＋弱さ→検証の割り当て
- 計測の予定（どの Sprint で何を測るか）

# 進め方
1 ファイルずつ。私が材料を貼る → あなたが型に統合した叩き台を出す → 私が自分の言葉に直す → 次のファイルへ。
3 ファイルがそろったら、最後にフルパッケージ一覧（PoC 計画書・ピッチ資料・引き継ぎセットの場所と状態）を私がまとめる

# 最初にやること
docs/prd.md から。まず「プロダクト名と UVP 1 行」を私に確認してください。

# 仕上げ（必ずやる）
成果物がそろったら、2 つに分けて出力してください。
1. 引き継ぎ 3 ファイルは、それぞれをファイル名付きのコードブロックで出力する
   （私は workshop-2026-poc リポジトリの docs/poc/ に保存する）
2. フルパッケージ一覧と提出前チェックは、ワークシートの「✅ 最終アウトプット」セクションに
   そのまま貼り付けられる形（同じ項目・表構成の Markdown）で出力する
私が出し切れなかった箇所は断片から補完し、[AI補完] と印を付けてください。
最後に「3 ファイルを docs/poc/ に保存して、パッケージ一覧と提出前チェックをワークシートの
✅ 最終アウトプット に書き込んでから、[AI補完] の箇所を自分の言葉に直してね。
次フェーズで Cursor への最初の指示は『docs/ を読んで』から始めてね」と私に念押ししてください。
これがプロポーザルの最後の Stage です。次フェーズ（Sprint）の内容を先回りして作らないでください。

```

## ✅ 最終アウトプット（AI の完成版を貼って、[AI補完] を自分の言葉に直す）

### docs/prd.md

```markdown
# PRD — 【プロダクト名】

## UVP
（1 行）

## 課題と最初の 1 人/1 社
-

## コアのユーザーストーリー（3〜5 本）＋最大離脱点
-

## 画面一覧と Must
-

## やらないこと（Won't・PoC 範囲外）
-
```

### docs/architecture.md

```markdown
# Architecture — 【プロダクト名】

## 技術スタック
-

## 構成図
（Mermaid か画像）

## データモデル（スキーマスケッチ・Sprint 2 で更新）
-

## 外部サービスと API キー（無料枠・制限）
-

## スパイクで確認済みのこと
-
```

### docs/validation.md

```markdown
# Validation — 【プロダクト名】

## 仮説 / 検証方法 / 成功条件 / 失敗・撤退条件
-

## 5 つの問い＋弱さ→検証の割り当て
-

## 計測の予定（どの Sprint で何を測るか）
-
```

> この 3 枚が Cursor のコンテキストになる。Sprint 中に実装とズレたら、ドキュメントを先に直す——ズレたままの docs/ は AI に嘘を教え続ける。

### フルパッケージ一覧（3 点）

| # | 成果物 | 場所 | 状態 |
| --- | --- | --- | --- |
| 1 | PoC 計画書 |  |  |
| 2 | ピッチ資料（Slidev: pitch_slides.md ＋ public/ の素材一式） |  |  |
| 3 | 次フェーズ引き継ぎセット（実装前ドキュメント 3 点） |  |  |

### 提出前チェック

| チェック | OK? |
| --- | --- |
| PoC 計画書の成功・撤退条件が「後から動かせない数値」のまま入っている |  |
| 引き継ぎ 3 点が docs/poc/ に保存されている |  |
| pitch_slides.md と public/ の素材（keyvisual.html・lp_hero.html・spike_result.png）がセットで docs/proposal/ にある |  |
| 実測の無い数値がすべて ⚠ 未検証 / ⚠ 要検証 になっている |  |
| パッケージ 3 点の場所を審査員にそのまま言える |  |
