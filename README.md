<div align="center">

# rowlientr
**Script & Plugin Developer** · Python · Lua · JavaScript · C++ · C#

<br/>

<img src="https://skillicons.dev/icons?i=py,lua,js,cpp,cs,html,css,vscode,git,github,docker,wordpress,linux&perline=7&theme=dark" alt="Languages and Tools" />

</div>

<br/>

<p align="center">
  <a href="https://discord.com/users/378272432429203457">
    <img src="https://lanyard.cnrad.dev/api/378272432429203457?theme=dark&bg=0d1117&borderRadius=12px&hideBadges=true&showDisplayName=true&idleMessage=%C5%9Eu%20anda%20bu%20kullan%C4%B1c%C4%B1%20aktivite%20yapm%C4%B1yor" alt="Discord Presence" />
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
