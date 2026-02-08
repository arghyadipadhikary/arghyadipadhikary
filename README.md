<h1 align="center">Hi 👋, I'm Arghyadip</h1>

---

### 🧑‍💻 About Me:

I am a passionate Full Stack Developer and  Cybersecurity nerd, pursuing my B.Tech in Computer Science and Technology.  
I have strong experience working with the Python, Java, and MySQL.  
- 🧠 Solved over **12 problems on LeetCode** and **20 on HackerRank**  

---

### 📫 Socials:

[![GitHub](https://img.shields.io/badge/GitHub-000?style=for-the-badge&logo=github)](https://github.com/arghyadipadhikary)


---

### 💻 Tech Stack:


![Docker](https://img.shields.io/badge/docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![TensorFlow](https://img.shields.io/badge/tensorflow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Python](https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![React](https://img.shields.io/badge/react-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Kali Linux](https://img.shields.io/badge/Kali_Linux-557C94?style=for-the-badge&logo=kalilinux&logoColor=black)


---

### 🛠️ Tools:

![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=for-the-badge&logo=visual-studio-code)
![Git](https://img.shields.io/badge/git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/github-181717?style=for-the-badge&logo=github&logoColor=white)

---

name: Generate Snake

on:
  schedule:
    - cron: "0 */12 * * *"
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - uses: Platane/snk@v3
        with:
          github_user_name: Arghyadip
          outputs: |
            dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}


