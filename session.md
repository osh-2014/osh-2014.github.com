---
layout: default
title: セッション内容
sessions:
  -
    title: "「テスト駆動開発」(調整中)"
    description: "調整中です。"
    speaker: "和田 卓人"
    kana: "わだ たくと"
    profile: "<p>タワーズ・クエスト株式会社 取締役社長、プログラマ、<strong>テスト駆動開発者</strong>。学生時代にソフトウェア工学を学び、オブジェクト指向分析/設計に傾倒する。その後様々な縁に導かれソフトウェアパターンやXP（eXtremeProgramming）を実践する人たちと出会い、後の<strong>テスト駆動開発</strong>の誕生を知る。<strong>テスト駆動開発</strong>に「完璧主義の呪い（完璧な設計を得るまではコードを書けないし良いシステムも出来ないという強迫観念）」を解いてもらってからは、文章を書いたり、講演を行ったり、ハンズオンイベントを開催するなどして、<strong>テスト駆動開発</strong>を広めようと努力している。</p><p>今日もグリーンバンド（<strong>テスト駆動開発者の証</strong>）を左手に着け、テストと共にコードを書いている。</p><p>『<a href=\"http://www.oreilly.co.jp/books/9784873114798/\">プログラマが知るべき97のこと</a>』<br>『<a href=\"http://www.oreilly.co.jp/books/9784873115894/\">SQLアンチパターン</a>』（オライリージャパン）監修。</p>"
    twitter: "t_wada"
    facebook: "twada"
    github: "twada"
  -
    title: "「未定」(調整中)"
    description: "調整中です。"
    speaker: "長沢 智治"
    kana: "ながさわ ともはる"
    profile: "調整中です。"
    twitter: "tomohn"
  -
    title: "「未定」(調整中)"
    description: "調整中です。"
    speaker: "山城戸 祐樹"
    kana: "やまきど ゆうき"
    profile: "調整中です。"
    twitter: "kakenavi"
---

# セッション内容

随時、情報を公開していきます。

# セッションを予定しているスピーカー

{% for session in page.sessions %}
* [{{ session.speaker }}](#{{ session.twitter }}){% endfor %}

# セッション

{% for session in page.sessions %}
<div class="session">
<h2>{{ session.title }}</h2>

{{ session.description }}

<h3 id="{{ session.twitter }}">
  <small>speaker</small> {{ session.speaker}} <small>{{ session.kana }}</small></h3>
{{ session.profile }}
<p>
{% assign twitter = session.twitter %}
{% include twitter %}
{% assign github = session.github %}
{% include github %}
{% assign facebook = session.facebook %}
{% include facebook %}
</p>
</div>
{% endfor %}
