# 脱毛アフィリエイトLP プロジェクト

## ファイル構成

```
datsumo-lp/
├── index.html        # LP-A: 比較ランキング型
├── lp-b.html         # LP-B: 悩み共感型ストーリー
├── kpi-tracker.md    # KPI管理・撤退ルール
└── README.md         # このファイル
```

## LP概要

### LP-A（index.html）— 比較ランキング型
- **狙いキーワード**: 「脱毛 おすすめ 30代」「医療脱毛 比較」
- **ユーザー像**: 情報収集段階・複数サービスを比較検討中
- **構成**: ランキング表示 → 比較表 → チェックリスト → FAQ

### LP-B（lp-b.html）— 悩み共感型ストーリー
- **狙いキーワード**: 「自己処理 面倒」「ムダ毛 30代」「脱毛 始めたい」
- **ユーザー像**: 悩み強め・感情的動機・行動意欲高い
- **構成**: 悩み提示 → 共感 → 橋渡し → 推薦 → 緊急性 → CTA

## アフィリエイトリンクの設定方法

HTMLファイル内の以下のプレースホルダーを実際のA8.net/afb/アクセストレードのリンクに置換：

```
YOUR_A8_AFFILIATE_LINK_SBC   → 湘南美容クリニック（afb）
YOUR_A8_AFFILIATE_LINK_DIONE → Dione全身脱毛（アクセストレード）
YOUR_A8_AFFILIATE_LINK_MUSEE → ミュゼプラチナム（アクセストレード）
YOUR_A8_AFFILIATE_LINK       → メイン案件（最終決定後に設定）
```

## GitHub Pages でのデプロイ手順

```bash
git init
git add .
git commit -m "initial: 脱毛LP A/Bテスト用2パターン"
git remote add origin https://github.com/YOUR_USERNAME/datsumo-lp.git
git push -u origin main
```

GitHub リポジトリの Settings → Pages → Source: main branch / root

デプロイ後のURL:
- LP-A: `https://YOUR_USERNAME.github.io/datsumo-lp/`
- LP-B: `https://YOUR_USERNAME.github.io/datsumo-lp/lp-b.html`

## A/Bテスト実施方法

Google広告で2つのURLを設定：
1. 広告グループを2つ作成（「LP-A」「LP-B」）
2. 同一キーワード・同一予算で出稿
3. 各LP 500クリック到達後にCVRを比較
4. CVRの高い方を本番採用

## 必要なASP登録

- [ ] **afb（アフィビー）** - 湘南美容クリニック案件
- [ ] **アクセストレード** - ミュゼ・Dione案件
- [ ] **A8.net**（既登録） - 大美会クリニック等を検索・申請

## 薬機法 主要NGワード（厳守）

| NG表現 | 代替表現 |
|--------|---------|
| 永久脱毛 | 脱毛（エステ系では使用禁止） |
| 痛くない | 低刺激・肌にやさしい |
| 必ず効果が出る | 多くの方に選ばれています |
| 完全に毛がなくなる | 使用禁止 |
| 最安値 | 業界最安水準（根拠必要） |
| ○日で○○ | 使用禁止（確実性の示唆） |
| 治す・治療 | エステでは使用禁止 |

※医療脱毛クリニックの「永久脱毛」は医療機関のみ使用可
