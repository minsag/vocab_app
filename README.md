# VocabQuest 📚

A clean, offline-friendly vocabulary trainer. Drop your CSV file in the repo and it loads automatically.

## 🚀 Live Demo
> After enabling GitHub Pages: `https://YOUR-USERNAME.github.io/YOUR-REPO-NAME`

---

## 📁 File Structure

```
/
├── index.html        ← The app (single file, no build needed)
├── vocabulary.csv    ← Your word list (edit this!)
└── README.md
```

---

## 📋 CSV Format

The file must be named **`vocabulary.csv`** and placed in the root of the repo.

```csv
Vocabulary,Type,Phonetic,Definition,Example,Synonym,Antonym
crucial,adj,/kruːʤəl/,extremely important,Your role is crucial,vital,unimportant
agreement,noun,/əˈɡriː/,harmony in opinion,They nodded in agreement,consensus,disagreement
```

**Columns:**
| Column | Required | Description |
|--------|----------|-------------|
| Vocabulary | ✅ | The English word |
| Type | ✅ | adj / noun / verb / adv |
| Phonetic | ✅ | IPA pronunciation |
| Definition | ✅ | English definition |
| Example | optional | Example sentence |
| Synonym | optional | Comma-separated synonyms |
| Antonym | optional | Comma-separated antonyms |

> ⚠️ The header row is automatically skipped. Both **comma** and **tab** separated files are supported.

---

## 🎮 Game Modes

| Mode | Description | Difficulty |
|------|-------------|------------|
| 🃏 Flash Cards | Flip to reveal definition + auto-pronounce | Easy |
| 🎯 Multiple Choice | Choose correct definition from 4 options | Medium |
| 🔄 Reverse Quiz | See definition, guess the word | Medium |
| ⌨️ Type the Word | Type the correct word from definition | Hard |
| 🔗 Synonym Match | Match words with their synonyms | Hard |

---

## 🔊 Pronunciation

Built-in text-to-speech using the Web Speech API. Works best on:
- **Chrome** → Google US English
- **Edge** → Microsoft Aria/Jenny (Natural AI voice)
- **Safari** → Samantha / Karen

You can manually select any available voice from the dropdown in Flashcard mode.

---

## 🌐 Enable GitHub Pages

1. Go to your repo → **Settings** → **Pages**
2. Under *Source*, select **Deploy from a branch**
3. Choose **`main`** branch, **`/ (root)`** folder
4. Click **Save**
5. Your site will be live at `https://USERNAME.github.io/REPO-NAME` within a minute

---

## ✏️ How to update your word list

1. Edit `vocabulary.csv` directly on GitHub (click the file → pencil icon)
2. Commit the change
3. Reload the app — it fetches the latest CSV automatically

---

## 📌 Notes

- No server, no build step, no dependencies — pure HTML/CSS/JS
- Works offline after first load (if you save the page)
- The app fetches `vocabulary.csv` relative to `index.html`, so they must be in the same folder
