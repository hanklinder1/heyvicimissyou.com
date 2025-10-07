<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Hey Vic, I Miss You</title>
  <meta name="description" content="A tiny love note on the web." />
  <link rel="icon" href="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'><text y='0.9em' font-size='90'>💜</text></svg>">
  <style>
    :root {
      --bg: #0f1225;
      --card: #161a34cc;
      --text: #f3f4f7;
      --muted: #a9acc5;
      --accent: #9b87f5;
      --accent-2: #ff7ab6;
    }
    * { box-sizing: border-box; }
    html, body { height: 100%; }
    body {
      margin: 0;
      font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, "Helvetica Neue", Arial, "Apple Color Emoji", "Segoe UI Emoji";
      color: var(--text);
      background: radial-gradient(1200px 800px at 80% -10%, #1e2246 0%, #0f1225 60%), #0f1225;
      display: grid;
      place-items: center;
      line-height: 1.4;
    }
    .wrap {
      max-width: 920px;
      width: min(92vw, 920px);
      padding: 28px;
      border-radius: 24px;
      background: linear-gradient(180deg, #ffffff12, #ffffff05);
      backdrop-filter: blur(8px);
      box-shadow: 0 10px 40px rgba(0,0,0,.35);
      border: 1px solid #ffffff18;
      position: relative;
      overflow: hidden;
    }
    h1 {
      font-size: clamp(28px, 4.8vw, 64px);
      margin: 0 0 10px;
      letter-spacing: .5px;
    }
    .type { position: relative; display: inline-block; }
    .cursor { position: absolute; right: -6px; width: 4px; height: 1em; background: var(--text); animation: blink 1s steps(1) infinite; }
    @keyframes blink { 50% { opacity: 0; } }

    .sub { color: var(--muted); margin: 0 0 20px; font-size: clamp(14px, 1.8vw, 18px); }

    .card {
      display: grid; gap: 18px;
      grid-template-columns: 1fr; align-items: start;
    }
    @media (min-width: 820px) {
      .card { grid-template-columns: 1.2fr 1fr; }
    }

    .photo {
      aspect-ratio: 4/3; width: 100%;
      border-radius: 18px; overflow: hidden; position: relative;
      background: #0b0e1f; border: 1px solid #ffffff20;
      display: grid; place-items: center;
    }
    .photo img { width: 100%; height: 100%; object-fit: cover; display: block; }

    .uploader { text-align: center; color: var(--muted); padding: 14px; }
    .btn {
      display: inline-flex; align-items: center; gap: 8px;
      background: linear-gradient(135deg, var(--accent), var(--accent-2));
      color: white; border: none; padding: 12px 16px; border-radius: 12px;
      font-weight: 600; cursor: pointer; transition: transform .06s ease;
    }
    .btn:active { transform: translateY(1px) scale(.99); }

    .tools { display: flex; flex-wrap: wrap; gap: 10px; align-items: center; }
    .chip { background: #ffffff14; color: var(--text); padding: 8px 10px; border-radius: 999px; font-size: 13px; border: 1px solid #ffffff18; }

    .notes { background: #111432; border: 1px solid #ffffff14; border-radius: 14px; padding: 14px; }
    .notes h3 { margin: 0 0 8px; font-size: 16px; color: #e6e7fb; }
    .notes textarea { width: 100%; min-height: 96px; padding: 10px; border-radius: 10px; border: 1px solid #ffffff25; background: #0a0d26; color: var(--text); resize: vertical; }

    .footer { margin-top: 12px; color: #9094b8; font-size: 12px; text-align: center; }

    /* Heart confetti */
    .heart { position: fixed; pointer-events: none; animation: floatUp 1.6s ease forwards; filter: drop-shadow(0 5px 4px rgba(0,0,0,.2)); }
    @keyframes floatUp {
      0% { transform: translateY(0) scale(.8) rotate(0deg); opacity: .95; }
      90% { opacity: .9; }
      100% { transform: translateY(-140px) scale(1.05) rotate(15deg); opacity: 0; }
    }

    .topbar { position: absolute; inset: 0 0 auto 0; height: 8px; background: linear-gradient(90deg, var(--accent), var(--accent-2)); opacity: .8; }
    .hidden { display: none !important; }
    .counter { font-size: 14px; color: var(--muted); }
    .toggle { background: #ffffff12; border: 1px solid #ffffff18; color: var(--text); padding: 8px 12px; border-radius: 999px; cursor: pointer; font-size: 13px; }
    .center { text-align: center; }
    a { color: #c5c8ff; }
  </style>
</head>
<body>
  <div class="wrap" id="app">
    <div class="topbar"></div>
    <header>
      <h1 class="type">Hey Vic, I miss you<span class="cursor" aria-hidden="true"></span></h1>
      <p class="sub" id="subtitle">Loading a tiny love note…</p>
    </header>

    <section class="card">
      <!-- Photo side -->
      <div>
        <div class="photo" id="photoBox" aria-live="polite">
          <img id="preview" alt="Hank & Vic" class="hidden" />
          <div id="placeholder" class="center">
            <p style="margin:0 0 8px">Add your photo here</p>
            <button class="btn" id="selectBtn" type="button">📷 Upload Photo</button>
            <input type="file" id="file" accept="image/*" class="hidden" />
            <p class="uploader">The image stays in your browser (LocalStorage). No servers. 💫</p>
          </div>
        </div>
        <div class="tools" style="margin-top:10px">
          <button class="toggle" id="heartBtn" type="button">Send hearts</button>
          <button class="toggle" id="clearBtn" type="button">Reset photo</button>
          <span class="chip counter" id="counter"></span>
        </div>
      </div>

      <!-- Right side -->
      <div>
        <div class="notes">
          <h3>One‑liner for today</h3>
          <textarea id="note" placeholder="e.g., “Counting the days till our next pizza date.”"></textarea>
          <div class="tools" style="margin-top:10px">
            <button class="btn" id="saveNote" type="button">💌 Save Note</button>
            <span class="chip" id="savedMsg" aria-live="polite"></span>
          </div>
        </div>
        <div class="notes" style="margin-top:10px">
          <h3>Mini playlist (optional)</h3>
          <p class="sub" style="margin:0 0 8px">Drop a link to a song and it’ll show up below.</p>
          <input id="song" placeholder="https://open.spotify.com/track/..." style="width:100%; padding:10px; border-radius:10px; border:1px solid #ffffff25; background:#0a0d26; color:var(--text)"/>
          <div id="embed" style="margin-top:10px"></div>
        </div>
        <p class="footer">Made with 💜 by Hank — <a href="mailto:hank@example.com">say hi</a></p>
      </div>
    </section>
  </div>

  <script>
    // ——— Utilities ———
    const $ = (s, d=document) => d.querySelector(s);
    const state = {
      since: localStorage.getItem('since') || new Date().toISOString(),
      compliments: [
        "You + me > any algorithm.",
        "If missing you were cardio, I’d be shredded.",
        "BRB, manifesting your hug.",
        "You’re my favorite notification.",
        "Distance: temporary. Us: persistent."
      ]
    };

    // ——— Typewriter subtitle that adapts by time of day ———
    function subtitleByTime() {
      const h = new Date().getHours();
      if (h < 6) return "Late‑night thoughts of you.";
      if (h < 12) return "Morning miss‑you mode.";
      if (h < 18) return "Afternoon heart online.";
      return "Evening vibes + you on my mind.";
    }

    function typeSubtitle(text, i=0) {
      const el = $('#subtitle');
      el.textContent = text.slice(0, i);
      if (i <= text.length) requestAnimationFrame(() => typeSubtitle(text, i+1));
    }

    // ——— Days counter since first visit ———
    function updateCounter() {
      const days = Math.floor((Date.now() - new Date(state.since)) / (1000*60*60*24));
      $('#counter').textContent = days === 0 ? 'Day 0 of missing you streak' : `${days} day${days!==1?'s':''} on the miss‑you streak`;
    }

    // ——— Image upload & persistence ———
    const fileInput = $('#file');
    const preview = $('#preview');
    const placeholder = $('#placeholder');

    function showImage(src) {
      preview.src = src;
      preview.classList.remove('hidden');
      placeholder.classList.add('hidden');
    }

    fileInput.addEventListener('change', (e) => {
      const file = e.target.files[0];
      if (!file) return;
      const reader = new FileReader();
      reader.onload = () => {
        const dataUrl = reader.result;
        localStorage.setItem('photo', dataUrl);
        showImage(dataUrl);
      };
      reader.readAsDataURL(file);
    });

    $('#selectBtn').addEventListener('click', () => fileInput.click());

    $('#clearBtn').addEventListener('click', () => {
      localStorage.removeItem('photo');
      preview.classList.add('hidden');
      placeholder.classList.remove('hidden');
    });

    // Restore saved photo on load
    const saved = localStorage.getItem('photo');
    if (saved) showImage(saved);

    // ——— Hearts animation ———
    function spawnHearts(x, y) {
      const colors = ['#ff7ab6', '#ffb3d6', '#ffd1e6', '#c7b8ff', '#9b87f5'];
      const n = 12;
      for (let i=0;i<n;i++) {
        const h = document.createElement('div');
        h.className = 'heart';
        h.textContent = '❤';
        h.style.left = (x + (Math.random()*60-30)) + 'px';
        h.style.top = (y + (Math.random()*20-10)) + 'px';
        h.style.fontSize = (18 + Math.random()*20) + 'px';
        h.style.color = colors[i % colors.length];
        h.style.transform = `translateY(0) rotate(${(Math.random()*40-20)}deg)`;
        document.body.appendChild(h);
        setTimeout(() => h.remove(), 1700);
      }
    }

    $('#heartBtn').addEventListener('click', (e) => {
      const rect = e.target.getBoundingClientRect();
      spawnHearts(rect.left + rect.width/2, rect.top);
    });

    // Click anywhere to toss a few hearts
    document.addEventListener('click', (e) => {
      if (e.target.closest('.btn, .toggle, input, textarea, a')) return; // avoid spam
      spawnHearts(e.clientX, e.clientY);
    }, { passive: true });

    // ——— Notes + playlist ———
    const noteEl = $('#note');
    const savedNote = localStorage.getItem('note');
    if (savedNote) noteEl.value = savedNote;

    $('#saveNote').addEventListener('click', () => {
      localStorage.setItem('note', noteEl.value.trim());
      const msg = $('#savedMsg');
      msg.textContent = 'Saved ✨';
      setTimeout(() => msg.textContent = '', 1200);
    });

    const songEl = $('#song');
    const embed = $('#embed');
    const savedSong = localStorage.getItem('song');
    if (savedSong) { songEl.value = savedSong; renderEmbed(savedSong); }

    songEl.addEventListener('change', () => {
      const url = songEl.value.trim();
      localStorage.setItem('song', url);
      renderEmbed(url);
    });

    function renderEmbed(url) {
      embed.innerHTML = '';
      try {
        if (url.includes('spotify.com/track')) {
          const id = (url.split('/track/')[1]||'').split('?')[0];
          if (id) embed.innerHTML = `<iframe style="border-radius:12px" src="https://open.spotify.com/embed/track/${id}" width="100%" height="152" frameborder="0" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"></iframe>`;
        } else if (url.includes('youtube.com') || url.includes('youtu.be')) {
          const id = url.match(/[?&]v=([^&]+)/)?.[1] || url.split('youtu.be/')[1];
          if (id) embed.innerHTML = `<iframe width="100%" height="200" src="https://www.youtube.com/embed/${id}" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>`;
        }
      } catch {}
    }

    // ——— Secret mode via URL (e.g., ?vic) shows a random compliment in the header ———
    const params = new URLSearchParams(location.search);
    function maybeCompliment() {
      if (!params.has('vic')) return;
      const pick = state.compliments[Math.floor(Math.random()*state.compliments.length)];
      $('#subtitle').textContent = pick;
    }

    // ——— init ———
    typeSubtitle(subtitleByTime());
    updateCounter();
    maybeCompliment();
    // Save first-visit timestamp
    localStorage.setItem('since', state.since);
  </script>
</body>
</html>
