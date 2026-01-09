# Word Boxing 🥊

A competitive 1v1 word puzzle game where two players each choose a secret 5-letter word, then take turns trying to guess their opponent's word.

**[Play Now →](#)** *(add your hosted URL)*

---

## 🎮 How to Play

### Basic Rules

1. Each player secretly chooses a 5-letter word
2. Words are scored by letter rarity (Scrabble-style points)
3. **Lower-scoring word goes first** each round
4. On your turn, choose one action:
   - **Guess a letter** → Reveals all instances in opponent's word
   - **Solve** → Attempt to guess the entire word
5. First to solve opponent's word wins the round
6. **Best of 3 rounds** wins the match

### 🔤 Matched Letters

When battle begins, letters that appear in **both** words are automatically revealed (shown in gold). This creates strategic depth in word selection!

**Example:**
- Red picks "CRANE"
- Blue picks "STORM"  
- Red sees: `_T_R_` (T and R match)
- Blue sees: `_R___` (R matches)

### 📊 Letter Scoring

```
Low (1pt):  A E I O U L N R S T
Mid (2-4):  D G B C M P F H V W Y
High (5+):  K J X Q Z
```

---

## 🎯 Game Modes

### 🟢 Beginner Mode
- Pick a **new word each round**
- Great for learning the game
- More forgiving strategy

### 🔴 Advanced Mode
- Plan **all 3 words upfront** before the match
- **No letter can repeat** across your 3 words
- Forces strategic letter distribution
- Example valid set: `CRANE`, `BLOAT`, `JUMPS`

---

## 🏆 Play Options

### 📱 Pass & Play (Same Device)
- Two players, one device
- Pass the phone/tablet between turns
- **Unrated** - just for fun

### 🌐 Online Multiplayer
- Create a game → Get a 5-letter code
- Share code with friend → They join
- Real-time battles
- **Rated** when both players are signed in

---

## 📈 Ranking System

### ELO Rating
- Starting rating: **1200**
- Win against higher-rated = more points
- Lose against lower-rated = more penalty
- First 10 games use higher K-factor (faster movement)

### Rank Tiers

| Tier | Rating | Badge |
|------|--------|-------|
| Rookie | < 1000 | 🥉 |
| Contender | 1000-1199 | 🥈 |
| Fighter | 1200-1399 | 🥇 |
| Champion | 1400-1599 | 🏆 |
| Legend | 1600+ | 👑 |

### What's Tracked
- Rating & peak rating
- Wins / Losses
- Win streak & best streak
- Last 20 match history

---

## 🔐 Account & Sign In

- **Google Sign-In** to save your progress
- View your profile by clicking your avatar
- Check the **🏆 Leaderboard** to see top players
- Guests can play but matches won't be rated

---

## 🛠 Setup (Self-Hosting)

### Requirements
- Firebase project (free tier works)
- Web hosting (Firebase Hosting, Netlify, GitHub Pages, etc.)

### Quick Start

1. **Create Firebase Project**
   ```
   https://console.firebase.google.com/
   ```

2. **Enable Services**
   - Authentication → Google Sign-In
   - Realtime Database

3. **Add Security Rules**
   - Copy rules from `wordboxing-firebase-rules.json`

4. **Update Config**
   - Edit `wordboxing-multiplayer.html`
   - Replace `firebaseConfig` with your project's config

5. **Deploy**
   ```bash
   # Firebase Hosting
   firebase deploy
   
   # Or just upload the HTML file to any static host
   ```

See `wordboxing-firebase-setup.md` for detailed instructions.

---

## 📁 Files

| File | Description |
|------|-------------|
| `wordboxing-multiplayer.html` | Main game (all-in-one) |
| `wordboxing-firebase-setup.md` | Firebase setup guide |
| `wordboxing-firebase-rules.json` | Security rules |
| `wordboxing-project-docs.md` | Full technical documentation |

---

## 🎨 Features

- ✅ Pass & Play mode
- ✅ Online multiplayer
- ✅ Beginner & Advanced modes
- ✅ 4,757 word dictionary
- ✅ Google Sign-In
- ✅ ELO rating system
- ✅ Leaderboard
- ✅ Match history
- ✅ Mobile responsive
- ✅ No install required (pure HTML/JS)

---

## 🗺 Roadmap

### Coming Soon
- [ ] Sound effects
- [ ] Animations
- [ ] Rematch button (online)
- [ ] Share results

### Future
- [ ] Friends list
- [ ] Private matches
- [ ] Achievements
- [ ] Seasonal rankings
- [ ] Mobile app

---

## 🧰 Tech Stack

- **Frontend:** Vanilla HTML/CSS/JavaScript
- **Backend:** Firebase Realtime Database
- **Auth:** Firebase Authentication (Google)
- **Fonts:** Google Fonts (Oswald, Roboto)

---

## 📜 Version History

| Version | Changes |
|---------|---------|
| 0.6.0 | User auth, ELO ratings, leaderboard |
| 0.5.0 | Integrated Pass & Play |
| 0.4.0 | Advanced 3-word planning mode |
| 0.3.0 | Online multiplayer |
| 0.2.0 | Beginner/Advanced modes |
| 0.1.0 | Initial prototype |

---

## 📄 License

MIT License - feel free to fork and modify!

---

## 🤝 Credits

Created with ❤️ and Claude AI

---

*Ready to step into the ring? 🥊*
