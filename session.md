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
    id: t_wada
  -
    title: "「これからのつながる開発環境とその秘訣(仮)」"
    description: "ソフトウェア開発はフィードバックループの連鎖の中で、開発者がクリエイティブな仕事を行い、アイデアをビジネス価値としてユーザーにデリバリーすることです。そこには複雑さ、未経験な分野への挑戦があり、協調することで問題に立ち向かっていくことが求められます。このセッションでは、最新の開発環境がいかに重要なのかをご紹介します。"
    speaker: "長沢 智治"
    kana: "ながさわ ともはる"
    profile: "<p>通りすがりのエバンジェリスト。ソフトウェア開発のライフサイクル全般を経験したのち、開発者から開発者を支援するコンサルタントやアーキテクト、エバンジェリストを経験。リアル、バーチャル関係なく、通りすがりながらなにかお手伝いできないかを考え、行動する日々。趣味は、海水魚飼育と仮面ライダー。</p><p>『<a href=\"http://www.amazon.co.jp/%E3%82%A2%E3%82%B8%E3%83%A3%E3%82%A4%E3%83%AB%E3%82%BD%E3%83%95%E3%83%88%E3%82%A6%E3%82%A7%E3%82%A2%E3%82%A8%E3%83%B3%E3%82%B8%E3%83%8B%E3%82%A2%E3%83%AA%E3%83%B3%E3%82%B0-%E5%9F%BA%E6%9C%AC%E6%A6%82%E5%BF%B5%E3%81%8B%E3%82%89%E7%B6%99%E7%B6%9A%E7%9A%84%E3%83%95%E3%82%A3%E3%83%BC%E3%83%89%E3%83%90%E3%83%83%E3%82%AF%E3%81%BE%E3%81%A7-%E3%83%9E%E3%82%A4%E3%82%AF%E3%83%AD%E3%82%BD%E3%83%95%E3%83%88%E9%96%A2%E9%80%A3%E6%9B%B8-Sam-Guckenheimer/dp/4822294684\" target=\"_blank\">アジャイルソフトウェアエンジニアリング</a>』<br>（日経BP）監訳者代表</p><p>Blog: <a href=\"http://softwareengineeringplatform.com\" target=\"_blank\">softwareengineeringplatform.com</a>, <a href=\"http://blogs.itmedia.co.jp/nagap/\" target=\"_blank\">ITとビジネスの可能性</a></p>"
    twitter: "tomohn"
    facebook: tomoharu.nagasawa
    id: "tomohn"
  -
    title: "「未定」(調整中)"
    description: "調整中です。"
    speaker: "山城戸 祐樹"
    kana: "やまきど ゆうき"
    profile: "調整中です。"
    twitter: "kakenavi"
    id: "kakenavi"
  -
    title: "「形から入るスクラム」"
    description: "開発現場でスクラムのプラクティスを使ってみて"
    speaker: "川口 稔"
    kana: "かわぐち みのる"
    profile: "すくすくスクラム広島スタッフ。ふだんは業務系システムの開発をしています。"
    id: kawaguchi
  -
    title: "「すくすくスクラム広島やってますよ～。(仮)」"
    description: "「すくすくスクラム広島」の活動内容、また活動をするようになってからの変化。活動することの伝播を目指す。"
    speaker: "田中 靖也"
    kana: "たなか やすなり"
    profile: "ひょんなことから「すくすくスクラム広島」スタッフへ。ふだんは業務系システムのSE的なお仕事をしている。チームパフォーマンスの最大化を意識し、継続的に成果を出し続けることを目標にしている。"
    id: tanaka
---

# セッション内容

随時、情報を公開していきます。

# セッションを予定しているスピーカー

{% for session in page.sessions %}
* [{{ session.speaker }}](#{{ session.id }}){% endfor %}

# セッション

{% for session in page.sessions %}
<div class="session">
<h2 class="session-title">{{ session.title }}</h2>

<p>{{ session.description }}</p>

<h3 id="{{ session.id }}">
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
