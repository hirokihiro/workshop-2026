---
title: しめきりボード 月500円プラン
class: simple500
---

<style>
.slidev-layout {
  padding: 0 !important;
  background: #f5f7fb;
  color: #111827;
  font-family: -apple-system, BlinkMacSystemFont, "Hiragino Sans", "Yu Gothic", "YuGothic", "Noto Sans JP", sans-serif;
}
.slidev-layout * {
  box-sizing: border-box;
  letter-spacing: 0 !important;
}
.s {
  width: 100%;
  height: 100%;
  padding: 34px 44px 24px;
  display: grid;
  grid-template-rows: 24px 1fr 18px;
  gap: 16px;
  overflow: hidden;
}
.top, .foot {
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: #7b8495;
  font-size: 11px;
  font-weight: 800;
}
.brand {
  display: inline-flex;
  align-items: center;
  gap: 8px;
}
.brand::before {
  content: "";
  width: 10px;
  height: 10px;
  border-radius: 3px;
  background: #2563eb;
}
.main {
  min-height: 0;
  display: grid;
  align-items: center;
}
.split {
  display: grid;
  grid-template-columns: 1fr 390px;
  gap: 38px;
  align-items: center;
}
.split.flip {
  grid-template-columns: 390px 1fr;
}
.tag {
  color: #2563eb;
  font-size: 13px;
  font-weight: 900;
  text-transform: uppercase;
  margin-bottom: 12px;
}
.ttl {
  color: #0f172a;
  font-size: 43px;
  line-height: 1.14;
  font-weight: 950;
  max-width: 760px;
}
.ttl.small {
  font-size: 36px;
  line-height: 1.18;
}
.ttl .line {
  display: block;
}
.lead {
  color: #475467;
  font-size: 17px;
  line-height: 1.5;
  margin-top: 18px;
  max-width: 620px;
}
.phone {
  width: 320px;
  margin: 0 auto;
  background: #111827;
  border-radius: 30px;
  padding: 12px;
  box-shadow: 0 26px 54px rgba(15, 23, 42, 0.25);
}
.screen {
  min-height: 410px;
  border-radius: 22px;
  background: #fff;
  padding: 16px;
}
.screen.dark {
  background: #0f172a;
  color: #fff;
}
.appbar {
  display: flex;
  justify-content: space-between;
  align-items: baseline;
  margin-bottom: 12px;
}
.appbar b {
  color: #111827;
  font-size: 18px;
}
.screen.dark .appbar b {
  color: #fff;
}
.appbar span {
  color: #0f766e;
  font-size: 15px;
  font-weight: 900;
}
.mini-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 7px;
  margin-bottom: 10px;
}
.mini {
  border-radius: 8px;
  background: #eff6ff;
  padding: 8px;
}
.mini b {
  display: block;
  color: #2563eb;
  font-size: 16px;
  line-height: 1;
}
.mini span {
  color: #64748b;
  font-size: 9px;
  font-weight: 900;
}
.task {
  border-radius: 9px;
  border: 1px solid #e5e7eb;
  padding: 11px;
  margin-top: 8px;
  background: #fff;
}
.task.red { background: #fff1f2; border-color: #fecdd3; }
.task.yellow { background: #fffbeb; border-color: #fde68a; }
.task.green { background: #ecfdf5; border-color: #bbf7d0; }
.task strong {
  display: block;
  color: #111827;
  font-size: 14px;
  line-height: 1.25;
}
.task span {
  display: flex;
  justify-content: space-between;
  color: #64748b;
  font-size: 11px;
  font-weight: 900;
  margin-top: 7px;
}
.price {
  border-radius: 18px;
  background: #0f172a;
  color: #fff;
  padding: 30px;
  box-shadow: 0 26px 56px rgba(15, 23, 42, 0.18);
}
.price .yen {
  font-size: 76px;
  line-height: 1;
  font-weight: 950;
}
.price .yen small {
  font-size: 24px;
}
.price p {
  color: #cbd5e1;
  font-size: 17px;
  line-height: 1.55;
  margin: 16px 0 0;
}
.cards {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 16px;
}
.card {
  background: #fff;
  border: 1px solid #d8dee8;
  border-radius: 14px;
  padding: 20px;
  min-height: 180px;
  box-shadow: 0 16px 36px rgba(15, 23, 42, 0.07);
}
.card .icon {
  width: 46px;
  height: 46px;
  border-radius: 12px;
  display: grid;
  place-items: center;
  background: #eff6ff;
  color: #2563eb;
  font-size: 24px;
  font-weight: 950;
  margin-bottom: 16px;
}
.card b {
  display: block;
  color: #111827;
  font-size: 21px;
  line-height: 1.25;
}
.card span {
  display: block;
  color: #64748b;
  font-size: 14px;
  line-height: 1.45;
  margin-top: 9px;
}
.short {
  max-width: 560px;
}
.receipt {
  background: #fff;
  border: 1px solid #d8dee8;
  border-radius: 16px;
  padding: 24px;
  box-shadow: 0 18px 42px rgba(15, 23, 42, 0.12);
}
.receipt-row {
  display: flex;
  justify-content: space-between;
  gap: 20px;
  padding: 13px 0;
  border-bottom: 1px dashed #cbd5e1;
  color: #344054;
  font-size: 18px;
  font-weight: 800;
}
.receipt-row.total {
  border-bottom: 0;
  color: #be123c;
  font-size: 30px;
  font-weight: 950;
}
.flow {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 14px;
}
.step {
  background: #fff;
  border: 1px solid #d8dee8;
  border-radius: 14px;
  padding: 18px;
  min-height: 220px;
  display: grid;
  grid-template-rows: auto auto 1fr auto;
  gap: 10px;
  box-shadow: 0 14px 34px rgba(15, 23, 42, 0.07);
}
.step .no {
  color: #2563eb;
  font-size: 13px;
  font-weight: 950;
}
.step b {
  color: #111827;
  font-size: 22px;
  line-height: 1.15;
}
.step span {
  color: #64748b;
  font-size: 13px;
  line-height: 1.45;
}
.pill {
  width: fit-content;
  border-radius: 999px;
  background: #eff6ff;
  color: #2563eb;
  padding: 7px 10px;
  font-size: 11px;
  font-weight: 900;
}
.poster {
  min-height: 390px;
  border-radius: 18px;
  background: #0f172a;
  color: #fff;
  padding: 42px;
  display: grid;
  align-content: center;
  overflow: hidden;
  position: relative;
}
.poster::after {
  content: "¥500";
  position: absolute;
  right: 34px;
  bottom: 28px;
  color: rgba(147, 197, 253, 0.22);
  font-size: 116px;
  font-weight: 950;
}
.poster b {
  color: #93c5fd;
  font-size: 14px;
  text-transform: uppercase;
}
.poster strong {
  display: block;
  max-width: 720px;
  color: #fff;
  font-size: 50px;
  line-height: 1.1;
  margin-top: 14px;
}
.poster span {
  display: block;
  color: #cbd5e1;
  font-size: 19px;
  line-height: 1.5;
  max-width: 680px;
  margin-top: 18px;
}
.compare {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 18px;
}
.compare-card {
  border-radius: 16px;
  padding: 24px;
  min-height: 330px;
  border: 1px solid #d8dee8;
  background: #fff;
}
.compare-card.blue {
  background: #eff6ff;
  border-color: #bfdbfe;
}
.compare-card b {
  color: #111827;
  font-size: 30px;
}
.compare-card ul {
  margin: 22px 0 0;
  padding: 0;
  list-style: none;
  display: grid;
  gap: 14px;
}
.compare-card li {
  color: #475467;
  font-size: 16px;
  line-height: 1.45;
}
.offer {
  display: grid;
  grid-template-columns: 0.86fr 1.14fr;
  gap: 22px;
  align-items: stretch;
}
.offer-left {
  border-radius: 18px;
  background: #0f172a;
  color: #fff;
  padding: 34px;
  display: grid;
  align-content: center;
}
.offer-left b {
  color: #93c5fd;
  font-size: 13px;
  text-transform: uppercase;
}
.offer-left strong {
  color: #fff;
  font-size: 36px;
  line-height: 1.16;
  margin-top: 14px;
}
.offer-left .yen {
  color: #93c5fd;
  font-size: 62px;
  line-height: 1;
  font-weight: 950;
  margin-top: 24px;
}
.offer-right {
  background: #fff;
  border: 1px solid #d8dee8;
  border-radius: 18px;
  padding: 24px;
  display: grid;
  align-content: center;
  gap: 12px;
}
.benefit {
  display: grid;
  grid-template-columns: 36px 1fr;
  gap: 12px;
  align-items: center;
  border-radius: 10px;
  background: #f8fafc;
  padding: 13px;
}
.benefit b {
  display: grid;
  place-items: center;
  width: 36px;
  height: 36px;
  border-radius: 10px;
  background: #eff6ff;
  color: #2563eb;
}
.benefit span {
  color: #344054;
  font-size: 15px;
  line-height: 1.35;
  font-weight: 800;
}
.btn {
  border-radius: 10px;
  background: #2563eb;
  color: #fff;
  text-align: center;
  padding: 14px;
  font-size: 15px;
  font-weight: 950;
}
</style>

<section class="s">
  <div class="top"><span class="brand">しめきりボード</span><span>月500円プラン</span></div>
  <div class="main">
    <div class="split">
      <div>
        <div class="tag">For students</div>
        <div class="ttl"><span class="line">次の解約忘れを、</span><span class="line">月500円で止める。</span></div>
        <div class="lead">忘れると損する期限だけを、残り日数と金額で見える化します。</div>
      </div>
      <div class="phone">
        <div class="screen">
          <div class="appbar"><b>期限リスク</b><span>12,800円</span></div>
          <div class="mini-grid">
            <div class="mini"><b>3</b><span>期限</span></div>
            <div class="mini"><b>今日</b><span>最優先</span></div>
            <div class="mini"><b>¥500</b><span>保険</span></div>
          </div>
          <div class="task red"><strong>動画サブスク無料体験</strong><span><b>今日まで</b><b>1,980円</b></span></div>
          <div class="task yellow"><strong>Adobe 学割更新</strong><span><b>あと3日</b><b>12,000円</b></span></div>
          <div class="task green"><strong>病院の再診</strong><span><b>あと7日</b><b>予約取り直し</b></span></div>
        </div>
      </div>
    </div>
  </div>
  <div class="foot"><span>Student subscription pitch</span><span>01 / 10</span></div>
</section>

<!--
学生には「便利な管理」ではなく、「次の解約忘れを止める」と伝えます。月500円は機能代ではなく、損失回避の保険として話します。
-->

---

<section class="s">
  <div class="top"><span class="brand">01 Pain</span><span>損した瞬間</span></div>
  <div class="main">
    <div class="split flip">
      <div class="receipt">
        <div class="receipt-row"><span>動画サブスク</span><span>1,980円</span></div>
        <div class="receipt-row"><span>Adobe 学割</span><span>12,000円</span></div>
        <div class="receipt-row"><span>家具レンタル</span><span>2,500円</span></div>
        <div class="receipt-row total"><span>忘れて失った金額</span><span>16,480円</span></div>
      </div>
      <div>
        <div class="tag">Pain</div>
        <div class="ttl small"><span class="line">気づいた時には、</span><span class="line">もう課金されている。</span></div>
        <div class="lead">通知もメールも流れる。痛みは、忘れた後に金額で来ます。</div>
      </div>
    </div>
  </div>
  <div class="foot"><span>Loss is visible after it happens</span><span>02 / 10</span></div>
</section>

<!--
入口は不便さではなく、損した記憶です。1,980円、12,000円のように、金額で痛みを見せます。
-->

---

<section class="s">
  <div class="top"><span class="brand">02 Price Anchor</span><span>500円の納得感</span></div>
  <div class="main">
    <div class="split">
      <div>
        <div class="tag">Price anchor</div>
        <div class="ttl small"><span class="line">1回防げば、</span><span class="line">約4ヶ月分の元が取れる。</span></div>
        <div class="lead">500円は、1,980円の解約忘れと比べて伝えます。</div>
      </div>
      <div class="price">
        <div class="tag" style="color:#93c5fd;">Monthly plan</div>
        <div class="yen">500<small>円/月</small></div>
        <p>1,980円を1回防げば、約4ヶ月分を回収できます。</p>
      </div>
    </div>
  </div>
  <div class="foot"><span>500 yen is a loss-prevention fee</span><span>03 / 10</span></div>
</section>

<!--
500円は高機能アプリ代ではなく、損を防ぐための小さな保険料として説明します。
-->

---

<section class="s">
  <div class="top"><span class="brand">03 Product</span><span>使いたくなる体験</span></div>
  <div class="main">
    <div class="cards">
      <div class="card"><div class="icon">¥</div><b>損失額が見える</b><span>忘れたらいくら失うかが分かります。</span></div>
      <div class="card"><div class="icon">!</div><b>危ない順に並ぶ</b><span>今日やるべき期限がすぐ分かります。</span></div>
      <div class="card"><div class="icon">✓</div><b>元が取れた感覚</b><span>避けた損失額が記録に残ります。</span></div>
    </div>
  </div>
  <div class="foot"><span>Product value</span><span>04 / 10</span></div>
</section>

<!--
学生が買うのは通知ではありません。損失額が見えること、危ない順に並ぶこと、元が取れた感覚が残ることです。
-->

---

<section class="s">
  <div class="top"><span class="brand">04 Free vs Paid</span><span>無料ツールとの違い</span></div>
  <div class="main">
    <div class="compare">
      <div class="compare-card">
        <b>無料カレンダー</b>
        <ul>
          <li>予定全体に混ざる</li>
          <li>通知を見落とす</li>
          <li>忘れた後に明細で気づく</li>
        </ul>
      </div>
      <div class="compare-card blue">
        <b>月500円プラン</b>
        <ul>
          <li>損する期限だけ見える</li>
          <li>失う金額で危険度が分かる</li>
          <li>1回防げば数ヶ月分回収</li>
        </ul>
      </div>
    </div>
  </div>
  <div class="foot"><span>Why paid</span><span>05 / 10</span></div>
</section>

<!--
無料カレンダーで十分な人には売りません。無料ツールで忘れて損した人に、損失専用の安心として提案します。
-->

---

<section class="s">
  <div class="top"><span class="brand">05 Checkout</span><span>課金直前画面</span></div>
  <div class="main">
    <div class="split">
      <div>
        <div class="tag">Payment moment</div>
        <div class="ttl small"><span class="line">「500円です」ではなく、</span><span class="line">「1,980円を止めます」。</span></div>
        <div class="lead">支払い前に、次に失いそうな金額を見せます。</div>
      </div>
      <div class="phone">
        <div class="screen">
          <div class="appbar"><b>プレミアム</b><span>初月無料</span></div>
          <div class="task red"><strong>次に失いそうな金額</strong><span><b>動画サブスク</b><b>1,980円</b></span></div>
          <div class="price" style="padding:18px;border-radius:12px;box-shadow:none;margin-top:10px;">
            <div class="yen" style="font-size:42px;">500<small>円/月</small></div>
            <p style="font-size:12px;margin-top:8px;">期限前通知・クラウド保存つき</p>
          </div>
          <div class="task green"><strong>1回防げば約4ヶ月分</strong><span><b>元が取れる</b><b>OK</b></span></div>
          <div class="btn" style="margin-top:12px;">初月無料で守りはじめる</div>
        </div>
      </div>
    </div>
  </div>
  <div class="foot"><span>Checkout screen</span><span>06 / 10</span></div>
</section>

<!--
月500円だけを出すと高く見えます。次に失いそうな1,980円を並べると、価格の意味が変わります。
-->

---

<section class="s">
  <div class="top"><span class="brand">06 Conversion</span><span>無料から有料への流れ</span></div>
  <div class="main">
    <div class="flow">
      <div class="step"><div class="no">STEP 1</div><b>損失診断</b><span>過去に失った金額を見る。</span><div class="pill">自分ごと化</div></div>
      <div class="step"><div class="no">STEP 2</div><b>1件登録</b><span>次の課金日を登録する。</span><div class="pill">行動確認</div></div>
      <div class="step"><div class="no">STEP 3</div><b>回避額表示</b><span>防げる金額を見る。</span><div class="pill">価格納得</div></div>
      <div class="step"><div class="no">STEP 4</div><b>500円提案</b><span>有料プランを提示する。</span><div class="pill">支払意思</div></div>
    </div>
  </div>
  <div class="foot"><span>Conversion journey</span><span>07 / 10</span></div>
</section>

<!--
いきなり月500円を出しません。損失診断、1件登録、回避額表示の後に、有料プランを提案します。
-->

---

<section class="s">
  <div class="top"><span class="brand">07 Validation</span><span>支払意思の検証</span></div>
  <div class="main">
    <div class="cards">
      <div class="card"><div class="icon">?</div><b>価値理解</b><span>10人中6人以上が、500円の価値を説明できる。</span></div>
      <div class="card"><div class="icon">+</div><b>実期限登録</b><span>10人中5人以上が、期限を1件登録したい。</span></div>
      <div class="card"><div class="icon">¥</div><b>支払意思</b><span>10人中4人以上が、月500円でも使いたい。</span></div>
    </div>
  </div>
  <div class="foot"><span>Payment validation</span><span>08 / 10</span></div>
</section>

<!--
検証するのは感想ではありません。価値理解、実期限登録、支払意思を見ます。
-->

---

<section class="s">
  <div class="top"><span class="brand">08 Message</span><span>学生に刺すコピー</span></div>
  <div class="main">
    <div class="poster">
      <b>Main message</b>
      <strong><span class="line">月500円で、</span><span class="line">次の解約忘れを止める。</span></strong>
      <span>忘れると損する期限だけを、金額つきで見える化。</span>
    </div>
  </div>
  <div class="foot"><span>Student-facing copy</span><span>09 / 10</span></div>
</section>

<!--
「便利な期限管理」では弱いです。「次の解約忘れを止める」と言い切ります。
-->

---

<section class="s">
  <div class="top"><span class="brand">09 Offer</span><span>最後の提案</span></div>
  <div class="main">
    <div class="offer">
      <div class="offer-left">
        <b>Student offer</b>
        <strong><span class="line">次の課金日を、</span><span class="line">今日から見える場所へ。</span></strong>
        <div class="yen">500円/月</div>
      </div>
      <div class="offer-right">
        <div class="benefit"><b>1</b><span>今日やる期限が見える</span></div>
        <div class="benefit"><b>2</b><span>忘れた時の損失額が分かる</span></div>
        <div class="benefit"><b>3</b><span>期限前に通知が届く</span></div>
        <div class="benefit"><b>4</b><span>初月無料。まず1件だけ登録</span></div>
        <div class="btn">初月無料で1件登録する</div>
      </div>
    </div>
  </div>
  <div class="foot"><span>Offer</span><span>10 / 10</span></div>
</section>

<!--
最後は「月500円で、次の解約忘れを止めませんか」です。初月無料で1件登録してもらいます。

想定 Q&A:
Q1. カレンダーでよくないですか。
A1. カレンダーは予定を見るものです。しめきりボードは、忘れるといくら損するかを見るものです。

Q2. 月500円は高くないですか。
A2. 1,980円の解約忘れを1回防げば、約4ヶ月分の元が取れます。高機能アプリ代ではなく、損失回避の保険料として提案します。

Q3. 無料なら使うけど有料は迷う人には？
A3. まず無料で1件登録してもらい、防げる金額を見せます。その後に500円を提示し、納得できる人だけ有料化します。
-->
