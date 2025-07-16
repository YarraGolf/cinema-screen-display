# 🎬 Yarra Golf Cinema Screen Display

This project powers a live display screen showing **today’s movie sessions** at the Yarrawonga Mulwala Golf Club Resort Cinema.

The display is hosted via **GitHub Pages** and reads session data from a `data.json` file updated automatically via Power Automate.

## 🖥️ Live Page

View the live cinema screen here:  
👉 [https://yarragolf.github.io/cinema-screen-display/](https://yarragolf.github.io/cinema-screen-display/)

## 📁 Project Structure

```
/
├── index.html        # Main display page (static HTML)
├── data.json         # Movie session data (auto-updated)
└── README.md         # Project description and setup info
```

## 🔄 How It Works

- `index.html` fetches `data.json` and displays sessions for the current day.
- The data includes:
  - 🎥 Title
  - 🕒 SessionTime
  - 🎟️ SeatsSold
- `data.json` is updated automatically from a Power Automate flow connected to the club’s session scheduling system.

## ⚙️ Technologies

- HTML, CSS, JavaScript
- GitHub Pages (static hosting)
- GitHub API (for updates)
- Power Automate (JSON writer)

## 📦 Deployment

There is no build process — this is a **static HTML site**.

To deploy updates:
- Edit `index.html` or `data.json` in the repo
- GitHub Pages will auto-deploy on commit to `main`

## 🚨 Troubleshooting

If the page displays `Error loading movie listings`:
- Confirm `data.json` is valid JSON
- Ensure it's publicly accessible at the correct path
- Check Power Automate flow is writing valid content

---

Maintained by the marketing team at [Yarra Golf](https://www.yarragolf.com.au)
