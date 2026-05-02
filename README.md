# 🚀 gh-project-launcher

**Универсальный установщик, обновлятор и лаунчер для проектов с GitHub**  
Автоматически настраивает окружение, устанавливает зависимости и запускает проект одной командой.

[![Windows](https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white)](start.bat)
[![Linux](https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black)](start.sh)
[![macOS](https://img.shields.io/badge/macOS-000000?logo=apple&logoColor=white)](start.sh)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## ✨ Возможности

- 🧠 **Определяет тип проекта сам** – Python, Node.js, Batch, HTML.
- 🔧 **Устанавливает Git, Python, Node.js** через системный менеджер пакетов (Windows – winget/choco, Linux – apt/dnf/pacman, macOS – brew).
- 🔐 **Настраивает SSH для приватных репозиториев** – ключ сохраняется, прописывается `~/.ssh/config` с `IdentitiesOnly yes`.
- 🌍 **Поддерживает публичные репозитории** (HTTPS) – без лишних вопросов.
- 🔄 **Автообновление самого скрипта** (Windows – из репозитория, Linux/macOS – при желании).
- 🎨 **Цветной вывод** и поддержка русского/английского интерфейса.
- 📦 **Создаёт виртуальное окружение Python и ставит зависимости** (`pip install -r requirements.txt`).
- 📦 **Устанавливает npm-пакеты** (`npm install` при наличии `package.json`).
- 🏁 **Запускает проект** – `python __main__.py`, `node server.js`, `index.html`, `start.bat` – что подходит.

## 📥 Быстрый старт

### Windows
1. Скачайте [start.bat](start.bat) в пустую папку.
2. Запустите `start.bat` (двойным щелчком).
3. При первом запуске введите **SSH‑URL** репозитория и **приватный SSH‑ключ**.
4. Всё! Скрипт установит нужное ПО, склонирует проект, создаст окружение и запустит приложение.

### Linux / macOS
1. Скачайте [start.sh](start.sh) и сделайте исполняемым:
   ```bash
   chmod +x start.sh
   ./start.sh
