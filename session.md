---
layout: default
title: セッション内容
sessions:
  -
    title: "「テスト駆動開発」(調整中)"
    description: "調整中です。"
    speaker: "和田 卓人"
    kana: "わだ たくと"
    profile: "調整中です。"
    twitter: "t_wada"
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

</div>
{% endfor %}
