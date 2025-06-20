### Olá, pessoal! 👋


  <div align="inline-block">
  <a href="https://github.com/muridev017">
<!--   <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=muridev017&langs_count=10&layout=compact"/> -->
</div>

<div align="center">
  <a href="https://github.com/muridev017">
  <img height="160em" src="https://github-readme-stats.vercel.app/api?username=muridev017&show_icons=true&theme=dracula&include_all_commits=true&count_private=true"/>
  <img height="160em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=muridev017&layout=compact&langs_count=7&theme=dracula"/>
</div>  

<Br>





<div style="display: inline_block"><br>
  
  <img align="center"  height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-plain.svg">
  
  <img align="center"  height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original.svg">
  
  <img align="center" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg">
  
  <img align="center"  height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg">
  
  <img align="center"  height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg">
  
  <img align="center"  height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/bootstrap/bootstrap-original.svg">
  
  <img align="center"  height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original.svg">
  
  <img align="center"  height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/c/c-original.svg">
  
  <img align="center"  height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg">
  
</div><br>
  
name: Generate Snake

on:
  schedule: 
    - cron: "0 */12 * * *" # roda a cada 12 horas
  workflow_dispatch:

jobs:
  build:
    name: Generate Snake Animation
    runs-on: ubuntu-latest

    steps:
      - name: Checkout repository
        uses: actions/checkout@v3

      - name: Generate the snake.svg
        uses: Platane/snk@master
        with:
          github_user_name: muridev017
          svg_out_path: dist/github-contribution-grid-snake.svg

      - name: Push snake.svg to the output branch
        uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}



<!--
**muridev017/muridev017** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.


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
