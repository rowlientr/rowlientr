<div align="center">

# rowlientr
**Script & Plugin Developer** · Systems, Automation & Tooling

<br/>

<a href="https://github.com/rowlientr">
  <img src="https://img.shields.io/badge/GitHub-rowlientr-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
</a>
<a href="https://discord.com/users/378272432429203457">
  <img src="https://komarev.com/ghpvc/?username=rowlientr&color=5865F2&style=for-the-badge&label=PROFILE+VIEWS&base=235147" alt="Profile Views" />
</a>

<br/><br/>

**[Discord Profile](https://discord.com/users/378272432429203457)** · **[Repositories](https://github.com/rowlientr?tab=repositories)**

</div>

<br/>

<p align="center">
  <a href="https://discord.com/users/378272432429203457">
    <img src="https://lanyard.cnrad.dev/api/378272432429203457?theme=dark&bg=161b22&borderRadius=12px&borderColor=5865F2&showDisplayName=true&idleMessage=Writing%20Scripts%20%26%20Plugins..." alt="Discord Presence" />
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
