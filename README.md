- 👋 Hi, I’m @kosuke-kk
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
kosuke-kk/kosuke-kk is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

name: LAPRAS Card

on:
  workflow_dispatch:
  schedule:
    - cron: "0 0 * * *"

jobs:
  update-card:
    name: LAPRAS Card
    runs-on: ubuntu-latest
    steps:
      - uses: kawamataryo/lapras-card-readme@main
        with:
          SHARE_ID: "kosuke-kk"
          # 以下オプション
          # https://lapras-card-generator.vercel.app でカスタマイズしたデザインを設定可能
          # ICON_FIRST: "#030E21"
          # ICON_SECOND: "#1688BF"
          # BACKGROUND_FIRST: "#020E27"
          # BACKGROUND_SECOND: "#0E5593"
          # LANG: "ja"
          # CARD_WIDTH: "400"
          # UPDATE_TIME: "true"
