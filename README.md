# The Architect's Apprentice

**An interactive exploration of geometry through the lens of architecture in the Global South.**

[▶ Live Demo](https://funksoup.github.io/Architects_Apprentice/)

---

## About

The Architect's Apprentice presents geometry problems grounded in real buildings across the Global South. Each challenge is rooted in the actual dimensions of a landmark — from the Great Pyramid of Giza to the Tomb of Askia in Mali — and accompanied by cultural context about the site.

Submit an answer and the Claude AI gives you personalised Socratic feedback: if you're right, it deepens the question; if you're off, it nudges you toward the answer without giving it away. A hint and a step-by-step answer reveal are always available.

**24 challenges across 8 countries:**

| Country | Buildings |
|---------|-----------|
| 🇪🇹 Ethiopia | Bete Giyorgis (Lalibela) · Fasil Ghebbi (Gondar) · Obelisk of Axum |
| 🇲🇽 Mexico | El Castillo (Chichen Itza) · Pyramid of the Sun (Teotihuacan) · Monte Albán |
| 🇮🇳 India | Taj Mahal (Agra) · Qutb Minar (Delhi) · Jantar Mantar (Jaipur) |
| 🇪🇬 Egypt | Great Pyramid of Giza · Karnak Temple Complex · Abu Simbel |
| 🇰🇭 Cambodia | Angkor Wat · Bayon (Angkor Thom) · Banteay Srei |
| 🇵🇪 Peru | Machu Picchu · Sacsayhuamán (Cusco) · Chan Chan (Trujillo) |
| 🇯🇴 Jordan | Al-Khazneh (Petra) · Oval Forum (Jerash) · Wadi Rum |
| 🇲🇱 Mali | Great Mosque of Djenné · Sankore Mosque (Timbuktu) · Tomb of Askia (Gao) |

**Concepts covered:** Area · Perimeter · Trigonometry · Circles · Pythagoras · Symmetry · Slope & Angles

---

## Running locally

The game is a single `index.html` file — no build step, no dependencies.

```bash
git clone https://github.com/funksoup/Architects_Apprentice.git
cd Architects_Apprentice
open index.html
```

### API key setup

Socratic feedback is powered by the [Claude API](https://www.anthropic.com/api). You'll need an Anthropic API key.

1. Copy the example config file:
   ```bash
   cp config.example.js config.js
   ```
2. Open `config.js` and replace `YOUR_API_KEY_HERE` with your key:
   ```js
   window.ANTHROPIC_API_KEY = 'sk-ant-...';
   ```

`config.js` is gitignored and will never be committed. If you skip this step, the game will prompt you for a key at runtime instead.

> **Note for the live demo:** The live demo does not include an API key. You will be prompted to enter your own key when the page loads.

---

## Built with

- Vanilla HTML, CSS, and JavaScript (single file, no frameworks)
- [Claude API](https://www.anthropic.com/api) (`claude-sonnet-4-20250514`) for Socratic feedback
- Images from [Wikimedia Commons](https://commons.wikimedia.org/)
