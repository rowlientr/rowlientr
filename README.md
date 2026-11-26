<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:3b1d6e,100:6d28d9&height=160&section=header&text=rowlientr&fontSize=40&fontColor=ffffff&animation=twinkling&fontAlignY=38&desc=Script%20%26%20Plugin%20Developer&descAlignY=60&descSize=15" width="100%" alt="Header Wave" />
</div>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=18&pause=1100&color=C084FC&center=true&vCenter=true&repeat=true&width=640&lines=Python+%7C+Lua+%7C+JavaScript+Developer;C%2B%2B+%26+C%23+Plugins+%7C+Automation+Scripts;Linux+%2C+Docker+%26+WordPress+Stack" alt="Animated Developer Role" />
</p>

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
