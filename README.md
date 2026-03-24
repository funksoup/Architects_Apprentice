# The Architect's Apprentice

**An interactive exploration of geometry through the lens of architecture in the Global South.**

[▶ Live Demo](https://architects-apprentice.vercel.app/)

---

![Landing page — choose a challenge](screenshots/ArchitectsApp_landing.png)

---

## About

The Architect's Apprentice presents geometry problems grounded in real buildings across the Global South. Each challenge is rooted in the actual dimensions of a landmark — from the Great Pyramid of Giza to the Tomb of Askia in Mali — and accompanied by cultural context about the site.

Submit an answer and the Claude AI gives you personalised Socratic feedback: if you're right, it deepens the question; if you're off, it nudges you toward the answer without giving it away. A hint and a step-by-step answer reveal are always available.

![A challenge in action](screenshots/ArchitectsApp_question.png)

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

The game is a single `index.html` file — no build step, no dependencies for the frontend.

```bash
git clone https://github.com/funksoup/Architects_Apprentice.git
cd Architects_Apprentice
open index.html
```

> **Note:** When running locally, `/api/claude` won't be available. To test the full experience including Claude feedback, deploy to Vercel (see below) or run a local server that handles the API route.

---

## Deploying to Vercel

The live demo runs on [Vercel](https://vercel.com) with a serverless function that proxies requests to the Claude API — no API key is exposed to the browser.

1. Fork or clone this repo and push to GitHub
2. Import the repo into Vercel (Add New Project → Import Git Repository)
3. In Vercel → Settings → Environment Variables, add:
   ```
   API_KEY=sk-ant-...
   ```
4. Deploy — Vercel will auto-deploy on every push to `main`

---

## Built with

- Vanilla HTML, CSS, and JavaScript (single file, no frameworks)
- [Claude API](https://www.anthropic.com/api) (`claude-sonnet-4-20250514`) for Socratic feedback
- [Vercel](https://vercel.com) serverless functions for secure API proxying
- Images from [Wikimedia Commons](https://commons.wikimedia.org/)

---

## Image credits

All images sourced from [Wikimedia Commons](https://commons.wikimedia.org/) under Creative Commons licences.

| Image | Author | Licence |
|-------|--------|---------|
| Bete Giyorgis, Lalibela | [Jialiang Gao](https://commons.wikimedia.org/wiki/File:Bete_Giyorgis_Lalibela_Ethiopia.jpg) | [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/) |
| Fasil Ghebbi, Gondar | [RyansWorld](https://commons.wikimedia.org/wiki/File:Fasiladas_Castle,_Gondar,_Amhara_Region,_Ethiopia.JPG) | [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/) |
| Obelisk of Axum | [Bair175](https://commons.wikimedia.org/wiki/File:Large_obelisk_in_Axum,_Ethiopia.jpg) | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) |
| El Castillo, Chichen Itza | [Daniel Schwen](https://commons.wikimedia.org/wiki/File:Chichen_Itza_3.jpg) | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) |
| Pyramid of the Sun, Teotihuacan | [Mariordo (Mario Roberto Durán Ortiz)](https://commons.wikimedia.org/wiki/File:Sun_Pyramid_05_2015_Teotihuacan_3304.JPG) | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) |
| Monte Albán, Oaxaca | [Pablo Fossas](https://commons.wikimedia.org/wiki/File:Monte_Alban,_Oaxaca._Agosto_2009.JPG) | [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/) |
| Taj Mahal, Agra | [Yann; edited by King of Hearts](https://commons.wikimedia.org/wiki/File:Taj_Mahal,_Agra,_India_edit2.jpg) | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) |
| Qutb Minar, Delhi | [Ramesam](https://commons.wikimedia.org/wiki/File:Qutub_minar,Delhi.JPG) | [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/) |
| Jantar Mantar, Jaipur | [S Sundararajan](https://commons.wikimedia.org/wiki/File:Jyotish_Yantralaya,_Jantar_Mantar.JPG) | [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/) |
| Great Pyramid of Giza | [kallerna](https://commons.wikimedia.org/wiki/File:Pyramid_of_Cheops_-_side.jpg) | [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/) |
| Karnak Temple Complex | [Taranis-iuppiter](https://commons.wikimedia.org/wiki/File:Karnak_temple_complex_2012.JPG) | [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/) |
| Abu Simbel | [Steve F-E-Cameron (Merlin-UK)](https://commons.wikimedia.org/wiki/File:SFEC_EGYPT_ABUSIMBEL_2006-003.JPG) | [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/) |
| Angkor Wat | [Satdeep Gill](https://commons.wikimedia.org/wiki/File:Angkor_Wat_with_its_reflection_(cropped).jpg) | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) |
| Bayon, Angkor Thom | [Diego Delso](https://commons.wikimedia.org/wiki/File:Bayon,_Angkor_Thom,_Camboya,_2013-08-17,_DD_37.JPG) | [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/) |
| Banteay Srei | [Michel Estermann](https://commons.wikimedia.org/wiki/File:Banteay_Srei.jpg) | [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/) |
| Machu Picchu | [Draceane](https://commons.wikimedia.org/wiki/File:Machu_Picchu,_2023_(012).jpg) | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) |
| Sacsayhuamán, Cusco | [Diego Delso](https://commons.wikimedia.org/wiki/File:Sacsayhuam%C3%A1n,_Cusco,_Per%C3%BA,_2015-07-31,_DD_05.JPG) | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) |
| Chan Chan, Trujillo | [Kevstan](https://commons.wikimedia.org/wiki/File:Vast_Abobe_Ruins_at_Chan_Chan.JPG) | [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/) |
| Al-Khazneh (Treasury), Petra | [Graham Racher / MrPanyGoff](https://commons.wikimedia.org/wiki/File:Al_Khazneh_Petra_edit_2.jpg) | [CC BY-SA 2.0](https://creativecommons.org/licenses/by-sa/2.0/) |
| Oval Forum, Jerash | [Kariman Mango](https://commons.wikimedia.org/wiki/File:Jerash_the_Oval_Plaza_in_springtime.jpg) | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) |
| Wadi Rum | [Berthold Werner](https://commons.wikimedia.org/wiki/File:Wadi_Rum_BW_6.JPG) | [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/) |
| Great Mosque of Djenné | [BluesyPete](https://commons.wikimedia.org/wiki/File:MaliDjenn%C3%A9Mosqu%C3%A9e.JPG) | [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/) |
| Sankore Mosque, Timbuktu | [upyernoz](https://commons.wikimedia.org/wiki/File:Sankore_Mosque_in_Timbuktu.jpg) | [CC BY 2.0](https://creativecommons.org/licenses/by/2.0/) |
| Tomb of Askia, Gao | [Taguelmoust](https://commons.wikimedia.org/wiki/File:Askia.jpg) | [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/) |
