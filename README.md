### Hi there 👋

<!--
**lMelkorl/lMelkorl** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

![lMelkorl's github stats](https://github-readme-stats.vercel.app/api?username=lMelkorl&show_icons=true&bg_color=282C35&icon_color=1CFF8E&text_color=9E9E9E&hide_border=true)

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=lMelkorl&layout=compact&bg_color=202529&icon_color=1CFF8E&text_color=9E9E9E&hide_border=true)

name: 📌 Starred topics
category: github
description: |
  This plugin displays [starred topics](https://github.com/stars?filter=topics).

  Check out [GitHub topics](https://github.com/topics) to search interesting topics.
examples:
  +with icons: https://github.com/lowlighter/metrics/blob/examples/metrics.plugin.topics.icons.svg
  +with labels: https://github.com/lowlighter/metrics/blob/examples/metrics.plugin.topics.svg
index: 4
supports:
  - user
scopes: []
inputs:

  plugin_topics:
    description: |
      Enable topics plugin
    type: boolean
    default: no
    extras:
      - metrics.run.puppeteer.scrapping

  plugin_topics_mode:
    description: |
      Display mode

      - `labels`: display labels
      - `icons`: display icons *(topics without icons will not be displayed)*
      - `starred`: alias for `labels`
      - `mastered`: alias for `icons`
    type: string
    default: starred
    values:
      - labels
      - icons
      - starred
      - mastered

  plugin_topics_sort:
    description: |
      Sorting method

      - `stars`: sort by most stars
      - `activity`: sort by recent activity
      - `starred`: sort by starred date
      - `random`: sort randomly
    type: string
    default: stars
    values:
      - stars
      - activity
      - starred
      - random

  plugin_topics_limit:
    description: |
      Display limit
    type: number
    default: 15
    min: 0
    max: 20
    zero: disable
