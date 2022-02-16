### Olá! Me chamo Lucas! 👋
Um software developer apaixonado por tecnologia, buscando transformar sonhos em realidade através da programação.

[![LinKeDin](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/lucas-souza-305283232/)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](https://mail.google.com/mail/u/0/#inbox)
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/LucasSo14747148)

![lucas GitHub stats](https://github-readme-stats.vercel.app/api?username=lucassouza01&show_icons=true&theme=dracula)

## Tecnologias que utilizo no dia a dia.
 
 <div style="display": inline_block><br/>
 <img aling="center" alt="html5" src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white"/> 
 <img aling="center" alt="css" src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white"/> 
 <img aling="center" alt="javascript" src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"/> 
 </div><br>

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=Lucassouza01&layout=compact)](https://github.com/anuraghazra/github-readme-stats) <br>
Email:lucassouza.dev01@gmail.com <br>
name: Generate Datas

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:

jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: rafaballerini
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}




