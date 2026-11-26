<div align="center">

# rowlientr
**Script & Plugin Developer** · Systems, Automation & Tooling

<br/>

<a href="https://discord.com/users/378272432429203457">
  <img src="https://img.shields.io/badge/GitHub-rowlientr-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
</a>
<img src="https://komarev.com/ghpvc/?username=rowlientr&color=blueviolet&style=for-the-badge&label=Profile+Views&base=235147" alt="Profile Views" />

<br/><br/>

**[Discord Profile](https://discord.com/users/378272432429203457)** · **[GitHub](https://github.com/rowlientr)**

</div>

<br/>

<p align="center">
  <a href="https://discord.com/users/378272432429203457">
    <img src="https://lanyard.cnrad.dev/api/378272432429203457?theme=dark&bg=0d1117&borderRadius=10px&hideBadges=true&hideActivity=false" alt="Discord Presence" />
  </a>
</p>

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
