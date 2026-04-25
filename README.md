## Raquel Rodrigues 

- 💻 UI Designer / Front-End Developer
- 👩🏾‍💻 Pronomes: ela/dela


<div>
  <a href="https://github.com/ewebeca">
  <img height="150em" src="https://github-readme-stats.vercel.app/api?username=ewebeca&theme=ocean_dark&show_icons=true"/> 
</div>

<div style="display: inline_block"><br>
<img align="center" alt="html" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/html5/html5-original.svg" />
<img align="center" alt="css" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/css3/css3-original.svg" />
<img align="right" alt="soft-gif" height="120" width="120" src="https://i.picasion.com/pic92/9c8f7ff03ba4bd067e752f641ccbdebd.gif">

##

<div>
 <a href="https://www.youtube.com/@ewebeca" target="_blank"><img src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white"></a>
  <a href="https://www.instagram.com/ewebeca" target="_blank"><img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank"></a>
 	<a href="https://www.twitch.tv/nraquelita" target="_blank"><img src="https://img.shields.io/badge/Twitch-9146FF?style=for-the-badge&logo=twitch&logoColor=white" target="_blank"></a> 
  <a href="https://www.x.com/ewebeca" target="_blank"><img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white"_blank"></a> 
</div>
  <a href="https://www.linkedin.com/in/raquel-rodrigues11/" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
</div>

<div> name: Generate snake animation

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"

  workflow_dispatch:

  push:
    branches:
    - master

jobs:
  generate:
    permissions:
      contents: write
    runs-on: ubuntu-latest
    timeout-minutes: 5

    steps:
      - name: generate snake.svg
        uses: Platane/snk/svg-only@v3
        with:
          github_user_name: ewebeca
          outputs: dist/snake.svg?palette=github-dark


      - name: push snake.svg to the output branch
        uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN } </div>

## GitHub Activity

