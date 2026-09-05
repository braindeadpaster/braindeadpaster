<div align="center">

<a href="https://github.com/rz">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=32&duration=2800&pause=800&color=E63946&center=true&vCenter=true&width=900&lines=rezzy+//+cheat+developer;game+hacking+%2F+injectors+%2F+internals;C%2B%2B+%E2%80%A2+C%23+%E2%80%A2+Python;learning+the+kernel." alt="Typing SVG" />
</a>

<br />

<img src="https://komarev.com/ghpvc/?username=braindeadpaster&label=Profile%20views&color=e63946&style=for-the-badge" alt="Profile views" />
<img src="https://img.shields.io/github/followers/braindeadpaster?label=Followers&style=for-the-badge&color=e63946&labelColor=1a1a1a" alt="Followers" />
<img src="https://img.shields.io/badge/Focus-Game%20Hacking-e63946?style=for-the-badge&labelColor=1a1a1a" alt="Focus" />
<img src="https://img.shields.io/badge/Learning-Windows%20Kernel-fbbf24?style=for-the-badge&labelColor=1a1a1a&logo=windows&logoColor=white" alt="Learning" />

</div>

---

## whoami

```cpp
namespace rz {
    struct Developer {
        const char* alias      = "rezzy";
        const char* role       = "developer";
        const char* focus[3]   = { "Game Hacking", "Injectors", "Anti-Cheat Bypass" };
        const char* learning[2]= { "Windows Kernel", "Driver Development" };
        const char* daily[3]   = { "C++", "C#", "Python" };
        const char* tools[3]   = { "Visual Studio", "x64dbg", "Cheat Engine" };
        bool        paster    = true;
    };
}
```



---

## arsenal

<div align="center">

<img src="https://skillicons.dev/icons?i=cpp,cs,py,bash,cmake,visualstudio,vscode,git,github,windows,&perline=9" alt="Tech stack" />

<br /><br />

![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=csharp&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Visual Studio](https://img.shields.io/badge/Visual_Studio-5C2D91?style=for-the-badge&logo=visualstudio&logoColor=white)
![x64dbg](https://img.shields.io/badge/x64dbg-3B7DDD?style=for-the-badge&logoColor=white)
![Cheat Engine](https://img.shields.io/badge/Cheat_Engine-B60000?style=for-the-badge&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

</div>

---

## current projects

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>🍣 sashimi-unturned</h3>
      <p>
        <img src="https://img.shields.io/badge/status-active-e63946?style=flat-square" />
        <img src="https://img.shields.io/badge/started-09%2F02%2F2026-1a1a1a?style=flat-square" />
        <img src="https://img.shields.io/badge/lang-C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white" />
        <img src="https://img.shields.io/badge/type-external-e63946?style=flat-square" />
      </p>
      <p>Fully <b>external</b> Unturned cheat powered by an <b>undiscovered vulnerable driver</b> for memory access. Zero user-mode footprint on the target process.</p>
      <ul>
        <li>Driver-backed memory read/write from a separate process</li>
        <li>External overlay + aim logic, no injection into the game</li>
        <li>Avoids common user-mode integrity scans by design</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h3>🗺️ rzmapper</h3>
      <p>
        <img src="https://img.shields.io/badge/status-stable-2ea043?style=flat-square" />
        <img src="https://img.shields.io/badge/lang-C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white" />
        <img src="https://img.shields.io/badge/fork_of-kdmapper-8a2be2?style=flat-square" />
      </p>
      <p>My <b>kdmapper fork</b> weaponizing <code>cormem.sys</code> as the vulnerable driver primitive. Manual-maps unsigned drivers into kernel with cleaner artifact scrubbing.</p>
      <ul>
        <li><code>cormem.sys</code> IOCTL primitives for MmMap / physical R/W</li>
        <li>PiDDB, MmUnloadedDrivers, and KdpData scrub</li>
        <li>Section wipe + entry point hijack post-map</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>💉 rzinject</h3>
      <p>
        <img src="https://img.shields.io/badge/status-active-e63946?style=flat-square" />
        <img src="https://img.shields.io/badge/lang-C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white" />
        <img src="https://img.shields.io/badge/VAC-undetected-2ea043?style=flat-square" />
        <img src="https://img.shields.io/badge/BE-undetected-2ea043?style=flat-square" />
      </p>
      <p>Personal <b>manual-map injector</b> private. built on an undiscovered vuln driver. Confirmed clean on <b>VAC</b> and <b>BattlEye</b> at time of writing.</p>
      <ul>
        <li>Manual mapping w/ TLS, reloc, and import resolution</li>
        <li>APC + thread-hijack execution paths</li>
        <li>Module stomping, header wipe, VAD hide</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h3>🗃️ rzvulns</h3>
      <p>
        <img src="https://img.shields.io/badge/status-growing-e63946?style=flat-square" />
        <img src="https://img.shields.io/badge/type-driver_collection-8a2be2?style=flat-square" />
        <img src="https://img.shields.io/badge/scope-all_games-1a1a1a?style=flat-square" />
      </p>
      <p>Private-tier repository of <b>hidden / unknown vulnerable drivers</b> — signed, unpatched, and not sitting on <code>loldrivers.io</code>. Works across every AC that lets a signed driver load.</p>
      <ul>
        <li>Each entry: driver, IOCTL map, primitives, POC</li>
        <li>Categorized by primitive (phys R/W, virt R/W, MSR, exec)</li>
        <li>Curated to avoid burned / flagged certs</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>🎨 rzui <sub><i>(planned)</i></sub></h3>
      <p>
        <img src="https://img.shields.io/badge/status-planning-fbbf24?style=flat-square" />
        <img src="https://img.shields.io/badge/lang-C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white" />
        <img src="https://img.shields.io/badge/inspired_by-Dear_ImGui-8a2be2?style=flat-square" />
      </p>
      <p>UI framework in the spirit of <b>Dear ImGui</b>, purpose-built for cheat devs: ESP primitives, aimbot config widgets, hotkey binders, config serialization, and stealth-friendly rendering hooks baked in.</p>
      <ul>
        <li>DX9 / DX11 / DX12 / Vulkan backends</li>
        <li>Built-in ESP box / snapline / bone widgets</li>
        <li>Zero-allocation immediate mode, no CRT dependency</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h3>🧪 what's next</h3>
      <p>
        <img src="https://img.shields.io/badge/roadmap-open-e63946?style=flat-square" />
      </p>
      <ul>
        <li>Deeper Windows kernel + WDM driver dev</li>
        <li>Ship first stable release of <code>rzui</code></li>
        <li>Grow <code>rzvulns</code> catalog with tested POCs</li>
        <li>Port cheats between more games to sharpen RE workflow</li>
      </ul>
    </td>
  </tr>
</table>

---

## stats

<div align="center">

<img height="180" src="https://github-readme-stats.vercel.app/api?username=braindeadpaster&show_icons=true&count_private=true&hide_border=true&title_color=e63946&icon_color=e63946&text_color=ffffff&bg_color=0d1117" />
<img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=braindeadpaster&layout=compact&hide_border=true&title_color=e63946&text_color=ffffff&bg_color=0d1117&langs_count=8" />

<br />

<img height="180" src="https://streak-stats.demolab.com?user=braindeadpaster&hide_border=true&background=0d1117&stroke=e63946&ring=e63946&fire=e63946&currStreakLabel=e63946&sideLabels=ffffff&currStreakNum=ffffff&sideNums=ffffff&dates=ffffff" />

<br /><br />

<img src="https://github-profile-trophy.vercel.app/?username=braindeadpaster&theme=onedark&no-frame=true&no-bg=true&column=7&margin-w=10" />

<br /><br />

<img src="https://github-readme-activity-graph.vercel.app/graph?username=braindeadpaster&bg_color=0d1117&color=e63946&line=e63946&point=ffffff&area=true&hide_border=true" width="98%" />

</div>

---

## currently learning / grinding

<div align="center">

| area | depth | notes |
|:----:|:-----:|:-----:|
| **C++** | `████████░░` | daily driver, cheats + injectors |
| **C#** | `██████░░░░` | tooling, loaders, WPF frontends |
| **Python** | `██████░░░░` | offset dumpers, automation scripts |
| **Game Hacking** | `███████░░░` | external + internal, ESP, aimbot, memory |
| **Windows Kernel** | `██░░░░░░░░` | learning — drivers, IOCTLs, EPROCESS |
| **Driver Development** | `██░░░░░░░░` | learning — WDM basics, IOCTL dispatch |

</div>

---

## quote

<div align="center">

<img src="https://quotes-github-readme.vercel.app/api?type=horizontal&theme=dark" />

</div>

---

## reach

<div align="center">

<a href="https://github.com/braindeadpaster"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
<a href="https://getmodulehandlew/"><img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" /></a>
<a href="https://donthaveone/"><img src="https://img.shields.io/badge/Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white" /></a>

<br /><br />

<sub><i>everything here is for educational and research purposes. i don't ship what i don't understand.</i></sub>

<br />

<img src="https://capsule-render.vercel.app/api?type=waving&color=e63946&height=100&section=footer" width="100%" />

</div>
