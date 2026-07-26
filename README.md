# AI Marathi — AI tools शिका मराठीत

AI Marathi ही मराठी भाषेत AI tools शिकवणारी free, open tutorial website आहे. Students, beginners, creators आणि professionals यांना ChatGPT, Claude Code, Gemini, Cursor, image/video tools, voice tools आणि इतर practical AI applications step by step समजावून सांगणे हा या project चा उद्देश आहे.

Content मध्ये natural Marathi सोबत गरजेपुरते familiar English technical terms वापरले आहेत—म्हणून tutorials वाचायला सोपे आणि प्रत्यक्ष वापरायला practical राहतात.

## Website मध्ये काय आहे?

### ✍ लिहा

- Copywriting
- Creative writing
- Research
- Planning
- Translation
- College essays

### `</>` Code

- Website बनवा
- App बनवा
- Debug आणि fix करा
- Automation
- Data analysis

### 🎨 बघा

- AI images
- AI videos
- Lipsync
- Photo editing
- Presentations

### 🎧 ऐका

- Voice generation
- Music generation
- Voice cloning
- Podcast creation
- Transcription

### Tool-specific guides

Repository मध्ये Claude Code, ChatGPT, Claude, Gemini, GitHub Copilot, Cursor, Perplexity, Midjourney, Nano Banana, Suno, Udio, ElevenLabs, Kling, Gamma, Canva AI आणि Windsurf यांसाठी स्वतंत्र pages आहेत.

## मुख्य features

- पूर्णपणे static HTML/CSS/JavaScript website
- कोणताही build step किंवा backend नाही
- Mobile-first responsive design
- Marathi-friendly Devanagari typography
- Dark आणि light themes
- Theme preference `localStorage` मध्ये save होते
- Task-based navigation आणि tool-specific tutorials
- GitHub Pages सारख्या static hosting साठी योग्य structure

## Local preview

Pages मध्ये `/aimarathi/...` असे absolute paths आहेत. त्यामुळे repository च्या parent directory मधून local server सुरू करा:

```bash
git clone https://github.com/anuphw/aimarathi.git
cd aimarathi/..
python3 -m http.server 8000
```

नंतर browser मध्ये उघडा:

```text
http://localhost:8000/aimarathi/
```

हा approach production मधील `/aimarathi/` base path सारखाच local preview देतो.

## Project structure

```text
.
├── index.html              # Homepage
├── assets/
│   ├── css/style.css       # Shared responsive design and themes
│   └── logo.svg
├── claude-code/            # Multi-page Claude Code course
├── likha/                  # Writing tutorials
├── code/                   # Coding and automation tutorials
├── bagha/                  # Image, video, and presentation tutorials
├── aika/                   # Voice, music, podcast, and transcription tutorials
└── <tool-name>/            # Individual AI tool guides
```

प्रत्येक tutorial साधारणपणे स्वतःच्या directory मधील `index.html` म्हणून ठेवला आहे. त्यामुळे clean URLs आणि static hosting दोन्ही सोपे राहतात.

## नवीन tutorial कसा add करायचा?

1. योग्य category किंवा tool साठी नवीन directory तयार करा.
2. त्या directory मध्ये `index.html` add करा.
3. Shared styling साठी `/aimarathi/assets/css/style.css` वापरा.
4. Navigation किंवा संबंधित category page वर tutorial ची link add करा.
5. Desktop आणि mobile दोन्ही layouts मध्ये page तपासा.
6. Dark आणि light theme दोन्हीमध्ये text, code blocks आणि callouts readable आहेत याची खात्री करा.

## Design conventions

- Page language: `lang="mr"`
- Default theme: dark
- Marathi font: Noto Sans Devanagari
- English/UI font: Inter
- Content width: approximately `720px`
- Reusable visual blocks: cards, tips, warnings, exercises आणि code blocks
- Technical शब्दांचे forced translation टाळून clear Marathi + English वापरा

## Deployment

ही static site GitHub Pages, Netlify किंवा इतर कोणत्याही static host वर deploy करता येते. Existing links `/aimarathi/` base path assume करतात. वेगळ्या domain root वर deploy करताना asset आणि navigation paths update करावे लागू शकतात.

## Project philosophy

AI बद्दल भीती निर्माण करणे हा उद्देश नाही. मराठी भाषिक learners ना tools समजून घेता यावेत, स्वतः प्रयोग करता यावेत आणि real कामासाठी वापरता यावेत—हा focus आहे.

**मराठीत शिका. Free. Step by step.**

## License

सध्या repository मध्ये license add केलेला नाही. License उपलब्ध होईपर्यंत standard copyright terms लागू राहतात.
