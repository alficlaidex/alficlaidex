<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:1f6feb,100:58a6ff&height=200&section=header&text=Alfi&fontSize=64&fontColor=ffffff&fontAlignY=36&animation=fadeIn&desc=Software%20Developer%20%C2%B7%20Backend%20%26%20Automation&descSize=18&descAlignY=58" alt="header" width="100%" />

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=22&duration=2800&pause=900&color=58A6FF&center=true&vCenter=true&width=640&lines=Building+production+systems;Node.js+%C2%B7+Python+%C2%B7+Next.js+%C2%B7+C%23;Clean+architecture%2C+boring+infrastructure;Ship+it.+Keep+it+running.)](https://git.io/typing-svg)

<br/>

[![Node.js](https://img.shields.io/badge/Node.js-20.9%2B-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org/)
[![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Next.js](https://img.shields.io/badge/Next.js-15-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)](https://nextjs.org/)
[![C#](https://img.shields.io/badge/C%23-.NET-239120?style=for-the-badge&logo=sharp&logoColor=white)](https://dotnet.microsoft.com/)
[![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)](https://www.sqlite.org/)

![Profile views](https://komarev.com/ghpvc/?username=alficlaidex&color=1f6feb&style=flat-square&label=PROFILE+VIEWS)
![Followers](https://img.shields.io/github/followers/alficlaidex?style=flat-square&color=1f6feb&logo=github)

</div>

---

## 👨‍💻 About

I build backend services, automation, and web apps, and I own them end to end:
from the architecture decision to the `pm2` process serving traffic.

```js
const alfi = {
  role: "Software Developer",
  primary: ["JavaScript", "Node.js"],
  also: ["Python", "Next.js", "C#/.NET"],
  focus: ["backend services", "automation", "web apps"],
  philosophy: "ship clean, keep infrastructure boring, write code that survives production",
};
```

| | |
|---|---|
| 🧱 **Architecture** | Small, composable modules with clear boundaries |
| 🛡️ **Reliability** | Atomic reloads, persisted state, no downtime on deploy |
| 🚀 **Delivery** | pm2 + Cloudflare Tunnel, HTTPS by default |
| 🔧 **Tooling** | Python and shell for automation, CI-friendly everything |

---

## 🚀 Selected Projects

### 🤖 Claidex-Bot

> Full-featured WhatsApp automation platform built on `zapo-js`: multi-prefix command routing, rich nativeFlow menus, and local SQLite state.

```mermaid
flowchart LR
    WA([WhatsApp]) <--> ZJ[zapo-js socket]
    ZJ --> R{{Command router<br/>multi-prefix}}
    R --> G[Permission guard<br/>admin / staff]
    G --> H[Handlers<br/>ai · downloader · game · group<br/>rpg · shop · owner · general]
    H --> DB[(SQLite)]
    H --> M[Media pipeline<br/>FFmpeg · sharp]
    H --> P[Puppeteer<br/>rendering]
    HR[[Atomic hot reload]] -.-> R
```

| | |
|---|---|
| **Categories** | `ai` · `downloader` · `game` · `group` · `rpg` · `shop` · `owner` · `general` |
| **Core** | Atomic hot reload, admin/staff permission model, anti-link & welcome flows, sticker/media toolkit |
| **RPG engine** | Characters, combat, quests, crafting, shop, travel, all persisted in SQLite |
| **Media** | YouTube/IG downloader (no API key), FFmpeg transcoding, sharp image pipeline |
| **Infra** | pm2 · Cloudflare Tunnel · WebSocket pairing/QR · Puppeteer rendering |

<br/>

### 🖼️ Claidex Collage

> Web app for composing photo collages with watermark and nameplate overlays. Live at **[collage.cloudku.us.kg](https://collage.cloudku.us.kg)**

```mermaid
sequenceDiagram
    autonumber
    participant B as Browser (canvas)
    participant A as Node.js API
    participant E as Export
    B->>B: Compose collage, watermark, nameplate
    B->>A: POST /api/collage (multipart)
    A->>A: Validate upload, store positioning metadata
    A->>E: Render / export
    E-->>B: Final image
```

| | |
|---|---|
| **Stack** | Node.js · canvas (client-side) · multipart API (`POST /api/collage`) |
| **Design** | Rendering stays on the client; the API stays thin (upload, metadata, export) |
| **Deploy** | pm2 behind Cloudflare Tunnel, HTTPS at `collage.cloudku.us.kg` |

---

## 🛠️ Tech Stack

<div align="center">

<img src="https://skillicons.dev/icons?i=js,nodejs,python,nextjs,react,cs,dotnet,sqlite,cloudflare,linux,git,github&perline=12" alt="skills" />

</div>

| Language / Framework | Use |
|---|---|
| **JavaScript / Node.js** | Primary: bots, APIs, realtime (ws), tooling |
| **Python** | Scripts, automation, data tooling |
| **Next.js** | React web apps, SSR, dashboards |
| **C# / .NET** | Windows-native and enterprise integrations |
| **SQLite · Puppeteer · FFmpeg · sharp** | Persistence, browser automation, media pipeline |
| **pm2 · Cloudflare Tunnel** | Process management, secure public exposure |

---

## 📊 GitHub Analytics

<div align="center">

<img height="180" src="https://github-readme-stats.vercel.app/api?username=alficlaidex&show_icons=true&theme=github_dark&hide_border=true&title_color=58A6FF&icon_color=79c0ff&bg_color=0d1117" alt="stats" />
<img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=alficlaidex&layout=compact&theme=github_dark&hide_border=true&title_color=58A6FF&bg_color=0d1117" alt="top languages" />

<br/>

<img src="https://streak-stats.demolab.com?user=alficlaidex&theme=github-dark-blue&hide_border=true&background=0d1117" alt="streak" />

<br/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=alficlaidex&bg_color=0d1117&color=58a6ff&line=1f6feb&point=ffffff&area=true&area_color=1f6feb&hide_border=true&custom_title=Contribution%20Activity" alt="activity graph" width="100%" />

<br/>

<img src="https://github-profile-trophy.vercel.app/?username=alficlaidex&theme=onedark&no-frame=true&no-bg=true&column=7&margin-w=10" alt="trophies" />

</div>

---

## 🌐 Connect

<div align="center">

[![WhatsApp Channel](https://img.shields.io/badge/WhatsApp%20Channel-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://www.whatsapp.com/channel/0029VbCOLKRKrWQtIO1vzN0E)
[![TikTok](https://img.shields.io/badge/TikTok-%40claidexdeveloper-000000?style=for-the-badge&logo=tiktok&logoColor=white)](https://www.tiktok.com/@claidexdeveloper)
[![Collage](https://img.shields.io/badge/Claidex%20Collage-live-1f6feb?style=for-the-badge&logo=cloudflare&logoColor=white)](https://collage.cloudku.us.kg)

<!-- Add when ready:
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/YOUR_HANDLE)
[![Telegram](https://img.shields.io/badge/Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/YOUR_HANDLE)
-->

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:1f6feb,100:58a6ff&height=100&section=footer" alt="footer" width="100%" />
