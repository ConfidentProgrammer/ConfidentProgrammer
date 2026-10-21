<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&height=200&color=0:0b1020,55:1e3a5f,100:f59e0b&text=Deep%20Patel&fontColor=ffffff&fontSize=56&fontAlignY=36&desc=Passionate%20software%20engineer%20%C2%B7%20Canada&descAlignY=58&descSize=18&animation=fadeIn" alt="Deep Patel, passionate software engineer" />

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=19&duration=2600&pause=900&color=F59E0B&center=true&vCenter=true&width=640&lines=I+build+things+to+understand+them.;Python+backends+by+day.;Rust+%26+Windows+internals+by+night.;Measure+it.+Don%27t+assume+it.;Every+dependency+has+to+earn+its+weight." alt="I build things to understand them." />
</p>

```console
$ whoami
deep: a software engineer who builds things to understand how they work

$ cat now.txt
building   jotkey, a 7 MB Rust tray app: a daily engineering log + an encrypted snippet vault
day job    Python backends and JavaScript frontends
learning   Rust ownership, Win32 focus rules, applied cryptography, system design
```

## 🛠️ Things I've built

### ⌨️ jotkey · the app I use every day <sub>(repo going public soon)</sub>
One hotkey, two jobs: jot a line about my workday before I forget it, or type a saved secret into any window **without it ever touching the clipboard**.

- **55 ms** from hotkey to screen, measured rather than guessed · **7 MB** app · **2.6 MB** installer
- **Vault:** Argon2id → XChaCha20-Poly1305, crash-safe atomic saves, keys wiped from memory on lock
- **Types into other apps** with Win32 `SendInput`, and refuses when it can't be sure: admin windows (UIPI), a closed target, keys still held
- **Never watches the keyboard:** the hotkey is registered with Windows, with no global hook
- **SQLite** in WAL mode with versioned migrations · **end-to-end encrypted backup** to a private GitHub repo
- **230+ tests:** unit tests, integration tests on real SQLite, and end-to-end runs that drive the built app

`Rust` `Tauri 2` `TypeScript` `SQLite` `Win32`

### 🌳 [branching-llm-engine](https://github.com/ConfidentProgrammer/branching-llm-engine) · chat that forks like git
Conversations are stored as a tree, so you can branch from any message and follow two ideas without one polluting the other. Each branch pulls context only from its own ancestors, using vector search filtered by the ancestry path.

`Python` `FastAPI` `PostgreSQL + pgvector` `React Flow`

### 📦 [File-Sharing-Service-Backend](https://github.com/ConfidentProgrammer/File-Sharing-Service-Backend) · uploads that clean up after themselves
An orchestrator saves the record, stores the file and issues a download token. If any step fails, a compensating step removes the record, so nothing is left half-done. Expiring tokens, indexed lookups, Docker, a CI deploy.

`Java` `Spring Boot` `PostgreSQL` `Docker` `GitHub Actions`

### 🔎 [Opensearch-prototype](https://github.com/ConfidentProgrammer/Opensearch-prototype) · a search engine from scratch, to see how one works
An inverted index in Node: tokenizing, chunked indexing of large files, AND queries and fuzzy search. A learning prototype, on purpose.

### 🟩 [habit-heatmap](https://github.com/ConfidentProgrammer/habit-heatmap) · data-structures practice with a UI
An O(n) year-to-week grid, O(1) day lookups with a hash map, and a custom memo comparator, so a click repaints 1 square instead of 365.

## 🧰 Toolbox

<p>
  <b>Languages</b><br/>
  <img src="https://skillicons.dev/icons?i=py,ts,js,rust,java,kotlin,cpp,powershell&perline=12" alt="Python, TypeScript, JavaScript, Rust, Java, Kotlin, C++, PowerShell" />
</p>
<p>
  <b>Backend & data</b><br/>
  <img src="https://skillicons.dev/icons?i=fastapi,spring,nodejs,postgres,sqlite,firebase&perline=12" alt="FastAPI, Spring, Node.js, PostgreSQL, SQLite, Firebase" />
</p>
<p>
  <b>Frontend & desktop</b><br/>
  <img src="https://skillicons.dev/icons?i=react,vite,tailwind,redux,html,css,tauri,windows&perline=12" alt="React, Vite, Tailwind, Redux, HTML, CSS, Tauri, Windows" />
</p>
<p>
  <b>Shipping it</b><br/>
  <img src="https://skillicons.dev/icons?i=docker,githubactions,nginx,jenkins,git,postman,vscode&perline=12" alt="Docker, GitHub Actions, Nginx, Jenkins, Git, Postman, VS Code" />
</p>

**Also:** pgvector · Pinecone · RAG pipelines · Gemini API · Pydantic · Argon2id / XChaCha20-Poly1305 · Win32 (`SendInput`, DPAPI) · WebView2

## 🧭 How I build

- **Measure it, don't assume it.** Every speed claim in my projects has a number behind it.
- **One idea per commit.** If I can't read the whole diff, it's too big.
- **Tests are what stop regressions.** I write them in the same pass as the feature, and I say plainly what's still untested.
- **Every dependency has to earn its weight.**
- **Fail safe.** When jotkey can't be sure which window it's typing into, it types nothing.

## 📚 How I learn

Every concept I ship gets a study card: what it is, the `file:line` where it lives, why it's there, and one question to test myself. jotkey's deck has **70 cards** so far, from SQLite's WAL mode to why a typed secret should never touch the clipboard.

## 🐍 My contributions, eaten

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ConfidentProgrammer/ConfidentProgrammer/output/github-snake-dark.svg" />
  <img width="100%" alt="A snake eating my contribution graph" src="https://raw.githubusercontent.com/ConfidentProgrammer/ConfidentProgrammer/output/github-snake.svg" />
</picture>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&height=110&section=footer&color=0:f59e0b,45:1e3a5f,100:0b1020" alt="" />
