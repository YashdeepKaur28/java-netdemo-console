# NetDemo — Java Console Shell 🖥️

A **Java Swing-based mini shell** that runs a command-line–style interface inside a GUI window. It demonstrates core Java concepts including **networking (sockets, InetAddress, URL), file I/O, runtime process execution, locale handling, and AWT/Swing GUI**.

## 📸 Preview

<img width="1075" height="625" alt="netdemo output" src="https://github.com/user-attachments/assets/b7385db4-9083-4e8f-94a9-fdf367d96cba" />


## 📖 Overview

**NetDemo** (internally titled *Molecule Virtual OS*) is a desktop application built with Java AWT that mimics a shell console. It provides a text prompt where users can type real commands that perform networking lookups, file operations, process execution, and system information queries — all without leaving the GUI.

This project was built to practice:
- Java **AWT & event handling** (`KeyListener`, `TextField`, `TextArea`)
- **Java Networking** (`InetAddress`, `Socket`, `URL`, `URLConnection`)
- **File I/O** (`FileInputStream`, `FileOutputStream`, `File`)
- **Runtime process execution** (`Runtime.exec`)
- **Locale & DateFormat** for internationalized time display


## ✨ Supported Commands

| Command | Meaning | Example |
|--------|---------|---------|
| `ip <host>` | Resolve hostname to IP addresses | `ip google.com` |
| `urlinfo <url>` | Show URL metadata (date, content type, last modified) | `urlinfo http://example.com` |
| `whois <domain>` | Query the internic WHOIS server | `whois internic.net` |
| `run <program>` | Launch an external program | `run notepad` |
| `find <file>` | Check if file(s) exist | `find readme.txt` |
| `date` | Show current date and time | `date` |
| `local -us` | Localized date/time for a country | `local -jp` |
| `sort <items>` | Sort given words alphabetically | `sort banana apple cherry` |
| `memcheck` | Show JVM memory usage | `memcheck` |
| `osinfo` | Show OS name, version, architecture | `osinfo` |
| `dir` | List files in current directory | `dir` |
| `cd <path>` | Change directory | `cd Programs` |
| `cd..` | Go to parent directory | `cd..` |
| `md <name>` | Create a new directory | `md newFolder` |
| `show <file>` | Print file contents | `show readme.txt` |
| `copy <src> <dest>` | Copy a file | `copy a.txt b.txt` |
| `ren <old> <new>` | Rename a file | `ren a.txt b.txt` |
| `kill <file>` | Delete a file | `kill old.txt` |
| `edit <file>` | Open edit mode on a file | `edit notes.txt` |
| `save <file>` | Save current buffer in edit mode | `save notes.txt` |
| `exit` | Exit edit mode | `exit` |
| `prompt <symbol>` | Change the prompt symbol | `prompt >>>` |
| `cls` | Clear the screen | `cls` |
| `bv / nv / ov / yv / gv` | Change console theme (Black / Normal / Orange / Yellow / Green) | `bv` |
| `help` or `?` | Show help table | `help` |
| `quit` | Exit the application | `quit` |


## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Language | Java (JDK 8+) |
| GUI | AWT (`Frame`, `Panel`, `TextField`, `TextArea`, `Scrollbar`) |
| Networking | `InetAddress`, `Socket`, `URL`, `URLConnection` |
| File I/O | `java.io.*` |
| Utilities | `StringTokenizer`, `Locale`, `DateFormat`, `Runtime` |
| Events | `KeyListener`, `WindowAdapter` |


## 🧠 Key Concepts Demonstrated

- **Networking:** `InetAddress.getAllByName()` for DNS, `Socket` for WHOIS on port 43, `URL.openConnection()` for HTTP metadata
- **File System:** `File`, `FileInputStream`, `FileOutputStream` for full CRUD on files
- **Process Management:** `Runtime.getRuntime().exec()` to launch external programs
- **Locale & i18n:** `DateFormat.getTimeInstance(FULL, Locale.X)` for country-specific formatting
- **GUI Programming:** AWT components with `BorderLayout`, custom fonts, and dynamic theming
- **Event Handling:** `KeyListener` for command history (↑ / ↓) and Enter key detection


## 🚀 Future Enhancements

- [ ] Migrate from AWT to **Swing** or **JavaFX** for a modern UI
- [ ] Add tab autocomplete for commands
- [ ] Support **piping** and command chaining (`cmd1 | cmd2`)
- [ ] Save command history to disk
- [ ] Cross-platform path handling (currently uses Windows-style `\`)
- [ ] Add a dark/light theme toggle in the menu bar
- [ ] Package as a runnable **JAR** for one-click launch


## 👩‍💻 Author

**Yashdeep Kaur**
- 🎓 B.Tech CSE, Punjabi University, Patiala (2026)
- 💼 Java Full Stack Trainee @ CodeSquadz
- 📧 Email: ykdeep2453@gmail.com
- 🔗 LinkedIn: [yashdeep-kaur-16aa083b1](https://linkedin.com/in/yashdeep-kaur-16aa083b1)
- 🐙 GitHub: [@YashdeepKaur28](https://github.com/YashdeepKaur28)


⭐ If you liked this project, consider giving it a star!
