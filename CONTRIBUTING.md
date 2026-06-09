# 👥 Contributing to Kingdom Trading Desk

This is a living tool built for the Kingdom team. Everyone on the team can suggest improvements, fix bugs, or add new features. Follow this guide so we can build fast without breaking things.

---

## 🔧 Setup

1. **Clone the repo**
```bash
git clone https://github.com/Cboyett77/kingdom-trading-desk.git
cd kingdom-trading-desk
```

2. **Open in browser** — just double-click `index.html`. No install needed.

3. **Edit with any code editor** — VS Code recommended.

---

## 🌿 Branch Strategy

```
main          ← always deployable, always working
feature/*     ← new features (e.g. feature/add-journal-panel)
fix/*         ← bug fixes (e.g. fix/checklist-not-saving)
design/*      ← visual/UI-only changes
```

**Never push directly to `main`.** Always branch, then open a Pull Request.

```bash
git checkout -b feature/your-feature-name
# make your changes
git add .
git commit -m "feat: describe what you built"
git push origin feature/your-feature-name
```

Then open a Pull Request on GitHub.

---

## ✅ Pull Request Checklist

Before submitting a PR, confirm:

- [ ] Tested in Chrome (open index.html locally)
- [ ] No console errors
- [ ] Light AND dark theme both look correct
- [ ] Mobile layout checked if you touched CSS
- [ ] PR description explains: what changed + why
- [ ] Screenshot attached if it's a UI change

---

## 📝 Commit Message Format

Use these prefixes for clean history:

| Prefix | Use for |
|---|---|
| `feat:` | New feature or panel |
| `fix:` | Bug fix |
| `design:` | Visual/CSS only change |
| `docs:` | README, comments, documentation |
| `refactor:` | Code cleanup, no behavior change |
| `data:` | Updating watchlist tickers, KPI targets, checklist tasks |

**Examples:**
```
feat: add journal entry panel to trading section
fix: checklist progress bar not resetting on new day
design: increase morning brief card contrast in dark mode
data: update default watchlist to include NVDA and AMZN
```

---

## 🛡️ Code Standards

- Keep everything in `index.html` (single-file architecture)
- Use existing CSS variables (`--gold`, `--teal`, `--green-2`, etc.) — don't hardcode colors
- JavaScript goes in the `<script>` block at the bottom
- New UI sections should follow the `.glass` card pattern
- Keep mobile breakpoints working (`@media (max-width: 760px)`)
- localStorage keys: prefix with `ktd_` to avoid conflicts

---

## 💡 Ideas for the Team to Build

Things that would make the desk even stronger:

- **Trade Journal** — log entries with date, ticker, grade, outcome, notes
- **P&L Tracker** — running daily/weekly/monthly profit display
- **News Feed Panel** — live macro news for pre-market prep
- **Risk Calculator** — position size based on account % risk
- **Streak Tracker** — consecutive green days, discipline streaks
- **Team Notes Board** — shared sticky notes / bias consensus
- **Alert Sound** — audio cue when a setup grade is clicked
- **Export Button** — download daily checklist as PDF

Pick one, branch off, build it, PR it in.

---

## ⚜ Kingdom Standard

> If it repeats, it needs a button. Every feature must remove mental energy, not add it.

When in doubt: keep it simple, keep it fast, keep it Kingdom.
