# 🍳 Ricettario Personale

Un sito single-page per le tue ricette, ottimizzato per GitHub Pages.

## 🚀 Pubblicazione su GitHub Pages

1. Crea un nuovo repository su GitHub
2. Carica tutti i file di questa cartella
3. Vai in **Settings** → **Pages**
4. Seleziona **Deploy from a branch** → **main** → **/ (root)**
5. Il sito sarà disponibile su `https://USERNAME.github.io/REPO-NAME/`

---

## 📝 Come Aggiungere una Nuova Ricetta

### Passo 1: Apri `index.html`

### Passo 2: Trova il punto di inserimento

Cerca questo commento nel file:

```html
    </main>

    <!-- Footer -->
```

### Passo 3: Incolla il template

Copia il contenuto da `_templates/template-ricetta.html` e incollalo **prima** di `</main>`.

### Passo 4: Personalizza la ricetta

Modifica i seguenti campi nel template:
- `id="nome-ricetta"` - ID univoco per la navigazione
- Titolo e descrizione
- Ingredienti
- Passaggi di preparazione e cottura
- Consigli

### Passo 5: Aggiungi al menu di navigazione

Trova la sezione `<nav>` e aggiungi un nuovo link:

```html
<nav>
    <ul>
        <li><a href="#merluzzo">🐟 Merluzzo Gratin</a></li>
        <li><a href="#nome-ricetta">🍝 Nuova Ricetta</a></li>  <!-- Aggiungi qui -->
        <li><a href="#consigli">💡 Consigli</a></li>
    </ul>
</nav>
```

### Passo 6: Salva e pubblica

```bash
git add index.html
git commit -m "Aggiunta ricetta: Nome Ricetta"
git push
```

---

## 📁 Struttura File

```
ricettario/
├── index.html                    # Sito principale
├── README.md                     # Questo file
├── _config.yml                   # Configurazione GitHub Pages
├── _templates/
│   ├── template-ricetta.md       # Template markdown per le ricette
│   └── template-ricetta.html     # Template HTML da copiare nel sito
└── _manuali/
    └── *.pdf                     # Manuali elettrodomestici
```

---

## 🎨 Personalizzazione

### Colori

I colori sono definiti come variabili CSS all'inizio di `index.html`:

```css
:root {
    --color-cream: #faf7f2;           /* Sfondo principale */
    --color-terracotta: #c45c3e;      /* Colore accento primario */
    --color-terracotta-dark: #a04a30; /* Accento scuro */
    --color-sage: #7a9a7a;            /* Verde salvia */
    --color-olive: #6b7c5c;           /* Verde oliva */
    --color-charcoal: #2d2d2d;        /* Testo principale */
    --color-warm-gray: #5a5a5a;       /* Testo secondario */
    --color-light-sage: #e8f0e8;      /* Sfondo sezioni */
}
```

### Font

Il sito usa Google Fonts:
- **Cormorant Garamond** - Titoli (elegante, serif)
- **Nunito** - Testo (leggibile, sans-serif)

Per cambiarli, modifica il link nel `<head>` e le variabili:

```css
--font-serif: 'Cormorant Garamond', Georgia, serif;
--font-sans: 'Nunito', -apple-system, sans-serif;
```

---

## 🔧 Emoji Utili per le Ricette

| Categoria | Emoji |
|-----------|-------|
| Pesce | 🐟 🦐 🦑 🐙 |
| Carne | 🍖 🥩 🍗 🥓 |
| Pasta | 🍝 🍜 |
| Pizza | 🍕 |
| Verdure | 🥗 🥦 🥕 🍅 |
| Dolci | 🍰 🧁 🍪 🎂 |
| Pane | 🥖 🥐 🍞 |
| Colazione | 🥞 🧇 🥚 |
| Bevande | ☕ 🍵 🧃 |
| Generale | 🍳 👨‍🍳 🔥 ⏱️ |

---

## 📋 Checklist Nuova Ricetta

- [ ] Copiato template HTML
- [ ] Modificato ID univoco (`id="nome-ricetta"`)
- [ ] Inserito titolo e descrizione
- [ ] Elencati tutti gli ingredienti
- [ ] Scritti i passaggi di preparazione
- [ ] Scritti i passaggi di cottura
- [ ] Aggiunti consigli utili
- [ ] Aggiunto link nel menu `<nav>`
- [ ] Testato in locale (aprire index.html nel browser)
- [ ] Fatto commit e push su GitHub

---

## 💡 Tips

- **Test locale**: Apri `index.html` direttamente nel browser per vedere le modifiche
- **Immagini**: Per aggiungere foto, usa servizi come [Imgur](https://imgur.com) e inserisci il link
- **Backup**: GitHub tiene lo storico di tutte le versioni
- **Mobile**: Il sito è già responsive, testa sempre su mobile

---

Buona cucina! 🍽️

