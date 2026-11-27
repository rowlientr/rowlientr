<div align="center">

# rowlientr

<img src="https://komarev.com/ghpvc/?username=rowlientr&color=2f81f7&style=for-the-badge&label=PROFILE+VIEWS&base=235147" alt="Profile Views" />

<br/><br/>

*Script & Plugin Developer · Automation · Custom Tooling · Systems*

</div>

---

<div align="center">

## About Me

Developer working with **Python**, **Lua**, **JavaScript**, **C++**, and **C#**, focused on practical scripts, plugins, and automation tools with clean and maintainable structure.

Experienced with **VS Code**, **Git**, **GitHub**, **Docker**, **WordPress**, and **Linux** environments to build reliable and modular workflows.

</div>

---

<div align="center">

## Discord Presence

<a href="https://discord.com/users/378272432429203457">
  <img src="https://lanyard.cnrad.dev/api/378272432429203457?theme=dark&bg=0d1117&borderRadius=12px&hideBadges=true&showDisplayName=true&idleMessage=%C5%9Eu%20anda%20bu%20kullan%C4%B1c%C4%B1%20aktivite%20yapm%C4%B1yor" alt="Discord Presence" />
</a>

</div>

---

<div align="center">

## Languages & Tools

### Languages

<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
<img src="https://img.shields.io/badge/Lua-2C2D72?style=for-the-badge&logo=lua&logoColor=white" alt="Lua" />
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
<img src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white" alt="C++" />
<img src="https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=csharp&logoColor=white" alt="C#" />

### Web & Markup

<img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
<img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
<img src="https://img.shields.io/badge/WordPress-21759B?style=for-the-badge&logo=wordpress&logoColor=white" alt="WordPress" />

### Tools & Platforms

<img src="https://img.shields.io/badge/VS%20Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="VS Code" />
<img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git" />
<img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
<img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" alt="Linux" />

</div>

---

<div align="center">

## GitHub Stats

<img src="https://github-readme-stats.vercel.app/api?username=rowlientr&show_icons=true&bg_color=0d1117&title_color=58a6ff&icon_color=58a6ff&ring_color=58a6ff&text_color=e6edf3&border_color=30363d&hide_border=false" height="175" alt="GitHub Stats" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=rowlientr&layout=compact&bg_color=0d1117&title_color=58a6ff&text_color=e6edf3&border_color=30363d&hide_border=false" height="175" alt="Top Languages" />

<br/><br/>

<img src="https://streak-stats.demolab.com/?user=rowlientr&theme=dark&background=0d1117&border=30363d&stroke=30363d&ring=58a6ff&fire=58a6ff&currStreakLabel=58a6ff" alt="GitHub Streak" />

</div>

---

````python
from dataclasses import dataclass, field


@dataclass(frozen=True)
class DeveloperProfile:
    handle: str = "rowlientr"
    role: str = "Script & Plugin Specialist"
    spoken_languages: tuple[str, ...] = ("Turkish",)
    programming_languages: tuple[str, ...] = (
        "Python",
        "JavaScript",
        "C++",
        "C#",
        "Lua",
        "HTML5",
        "CSS3",
    )
    stack: tuple[str, ...] = (
        "VS Code",
        "Git",
        "GitHub",
        "Docker",
        "WordPress",
        "Linux",
    )
    focus_areas: list[str] = field(
        default_factory=lambda: [
            "Custom plugins & extensions",
            "Automation scripts & tooling",
            "Clean modular architecture",
        ]
    )
    open_to_collaboration: bool = True

    def summary(self) -> str:
        langs = ", ".join(self.programming_languages)
        tools = ", ".join(self.stack)
        return f"{self.handle} [{self.role}] | Stack: {langs} | Env: {tools}"


profile = DeveloperProfile()
if __name__ == "__main__":
    print(profile.summary())
