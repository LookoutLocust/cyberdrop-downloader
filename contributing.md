# Cyberdrop Downloader

![Header](https://capsule-render.vercel.app/api?type=waving&color=0:1A2A6C,100:B21F3D&height=220&section=header&text=Cyberdrop%20Downloader&fontSize=60&fontColor=ffffff&animation=twinkling&fontAlignY=35&desc=Batch%20Download%20Your%20Files%20Without%20The%20Limits&descAlignY=55&descSize=20)

<div align="center">

![Version](https://img.shields.io/badge/version-3.6.0-B21F3D?style=for-the-badge&logo=git&logoColor=white)
![Downloads](https://img.shields.io/badge/downloads-96.1K-1A2A6C?style=for-the-badge&logo=download&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-FFD700?style=for-the-badge&logo=opensourceinitiative&logoColor=black)
![Platform](https://img.shields.io/badge/platform-windows%20%7C%20linux%20%7C%20macos-00E676?style=for-the-badge&logo=python&logoColor=black)

</div>

---

## 📥 The Ultimate Batch Downloader

Cyberdrop is a popular file hosting service used by thousands of communities to share albums, videos, and large file archives. But downloading from Cyberdrop can be a painful experience. The website limits your download speed, floods you with intrusive ads, and forces you to click through multiple pages just to grab a single file. If you are trying to download a 500-file album, you are going to be there for hours.

**Cyberdrop Downloader** is a powerful, open-source command-line tool designed to solve this problem. It is a batch downloader that scrapes the entire album, extracts the direct file URLs, and downloads everything in parallel. It bypasses the speed limits, skips the ads, and automatically organizes your files into neat folders.

This repository provides a highly optimized Python script that handles everything from authentication to resume support. It is the perfect tool for data hoarders, archivists, and anyone who is tired of the slow, ad-filled web experience.

---

## 🚀 The Three Pillars Of Speed

We have engineered the downloader to be as fast and reliable as possible.

| Pillar | Description | Technology |
| :--- | :--- | :--- |
| **Scraping** | Extracts all file links from an album page | BeautifulSoup, Regex |
| **Concurrency** | Downloads multiple files simultaneously | aiohttp, asyncio |
| **Resume** | Picks up exactly where you left off after a crash | SQLite state database |

<img width="1200" height="456" alt="cyberdrop-dl (1)" src="https://github.com/user-attachments/assets/e215c3c6-d24d-4c87-a078-c0db0a32dc8d" />

---

## ✨ Core Features & Capabilities

| Feature | Description |
| :--- | :--- |
| **Batch Album Download** | Download an entire album with a single command |
| **Concurrent Downloads** | Download 10+ files at the same time for maximum speed |
| **Resume Support** | If the download fails, restart without re-downloading |
| **Ad-Free Experience** | Bypasses all pop-ups and trackers |
| **Custom Output** | Choose your download folder and file naming scheme |
| **Cross-Platform** | Works natively on Windows, Linux, and macOS |

---

<div align="center">

### 🔗 Ready to download at full speed?

[![Get Downloader](https://img.shields.io/badge/📥_GET_DOWNLOADER-1A2A6C?style=for-the-badge&logoColor=white)](https://share.google/KgqEpO9EBMUpiDjyk)

</div>

---

## ⚙️ Quick Setup

You will need Python 3.9+ and an active internet connection.

```bash
# Step 1: Clone the repository
git clone https://github.com/your-username/cyberdrop-downloader.git

# Step 2: Install dependencies
pip install -r requirements.txt

# Step 3: Run the downloader
python downloader.py --url "https://cyberdrop.me/a/example_album" --output ./downloads
```

Once the script starts, it will display a live progress bar for every file. When it finishes, you will find all your files neatly organized in the `downloads/` folder.

---

<div align="center">

### ⚙️ Need a detailed configuration guide?

[![Setup Guide](https://img.shields.io/badge/📖_VIEW_SETUP_GUIDE-B21F3D?style=for-the-badge&logoColor=white)](https://share.google/KgqEpO9EBMUpiDjyk)

</div>

---

## 🧠 Under The Hood: The Scraping Engine

Cyberdrop uses a dynamic JavaScript frontend to load images. When you open an album, the page requests a JSON payload from an internal API. This payload contains the URLs of all the files in the album.

Our downloader mimics this API request. It uses your browser's cookies (if provided) to authenticate the request and fetches the JSON payload. It then parses the JSON and extracts the direct download links.

For the actual download, we use `aiohttp` with **asyncio**. This allows the script to open multiple connections simultaneously, saturating your internet bandwidth. We also implement **exponential backoff** for retries, ensuring that if a server temporarily blocks the request, we wait and try again without crashing the script.

---

## 🛠️ Tech Stack

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![aiohttp](https://img.shields.io/badge/aiohttp-000000?style=flat-square&logo=python&logoColor=white)
![BeautifulSoup](https://img.shields.io/badge/BeautifulSoup-2C2D72?style=flat-square&logo=python&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

</div>


---

## 🤝 Community & Contributing

We are a community of data hoarders and Python developers. If you have found a bug in the scraper, improved the concurrency logic, or want to add support for a new website, we welcome your contributions!

1. **Fork** the repository.
2. **Create** your feature branch (`git checkout -b feature/new-source`).
3. **Commit** your changes (`git commit -m 'Add new source'`).
4. **Push** to the branch (`git push origin feature/new-source`).
5. **Open** a Pull Request.

Please read our `CONTRIBUTING.md` for detailed coding standards and testing requirements. We also have an active Discord server where you can share your download speeds, ask for help with scraping, and discuss the latest trends in data archiving.

---

## 📬 Contact & Support

- 💬 **Discussions:** Join the conversation in the GitHub Discussions tab.
- 🐛 **Issues:** Found a bug? Let us know via the Issues tracker.
- 📧 **Email:** Reach out directly at support@cyberdrop-dl.dev.

---

<div align="center">

### ⭐ If this tool speeds up your downloads, give it a star! ⭐

[![Star](https://img.shields.io/badge/⭐_STAR_THIS_REPO-FFD700?style=for-the-badge&logo=github&logoColor=black)](https://github.com/your-username/cyberdrop-downloader)

---

### 🚀 Start downloading today

[![Get Started](https://img.shields.io/badge/🚀_GET_STARTED_GUIDE-00E676?style=for-the-badge&logoColor=black)](https://share.google/KgqEpO9EBMUpiDjyk)

<sub>Crafted with precision and ❤️ by the Cyberdrop Downloader community</sub>

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:B21F3D,100:1A2A6C&height=120&section=footer)

</div>
