<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Santa Workshop</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;600;800&family=Playfair+Display:wght@400;700;900&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg: #050510; --surface: #0e0e1a; --card: #151525;
            --gold: #d4a843; --red: #e74c3c; --green: #2ecc71;
            --blue: #3498db; --purple: #8e44ad; --text: #e8e8f0;
            --text2: #9090a0; --border: #252540; --radius: 14px;
        }
        * { margin:0; padding:0; box-sizing:border-box; }
        body {
            font-family: 'Montserrat', sans-serif;
            background: var(--bg); color: var(--text);
            min-height: 100vh; overflow-x: hidden;
        }
        body::before {
            content: ''; position: fixed; inset: 0; z-index:0;
            background: radial-gradient(ellipse at 30% 40%, rgba(231,76,60,0.06) 0%, transparent 50%),
                        radial-gradient(ellipse at 70% 30%, rgba(212,168,67,0.05) 0%, transparent 50%);
            pointer-events: none;
        }

        /* Telegram Colors */
        .tg-theme { background: var(--tg-theme-bg-color, var(--bg)); color: var(--tg-theme-text-color, var(--text)); }

        .app { position:relative; z-index:1; max-width:500px; margin:0 auto; min-height:100vh; display:flex; flex-direction:column; }

        /* Header */
        .header {
            background: rgba(14,14,26,0.95); backdrop-filter: blur(20px);
            border-bottom: 1px solid var(--border); padding: 12px 16px;
            display: flex; align-items: center; justify-content: space-between;
            position: sticky; top: 0; z-index: 100;
        }
        .logo { display:flex; align-items:center; gap:8px; cursor:pointer; }
        .logo-icon {
            width: 36px; height: 36px;
            background: linear-gradient(135deg, var(--red), #c0392b);
            border-radius: 10px; display: flex; align-items: center;
            justify-content: center; font-weight: 800; color: #fff; font-size: 16px;
        }
        .logo-text { font-size: 15px; font-weight: 800; color: #fff; }

        /* Navigation */
        .nav-links { display:flex; gap:2px; }
        .nav-link {
            padding: 6px 10px; border-radius: 8px; color: var(--text2);
            text-decoration: none; font-size: 10px; font-weight: 600;
            transition: all 0.3s; border: none; background: none;
            font-family: 'Montserrat', sans-serif; cursor: pointer;
        }
        .nav-link.active { background: rgba(231,76,60,0.15); color: var(--red); }

        /* Content */
        .content { flex:1; padding: 12px; }
        .page { display: none; animation: fadeIn 0.3s ease; }
        .page.active { display: block; }
        @keyframes fadeIn { from { opacity:0; transform: translateY(8px); } to { opacity:1; transform: translateY(0); } }

        /* Cards */
        .card {
            background: var(--surface); border: 1px solid var(--border);
            border-radius: var(--radius); padding: 16px; margin-bottom: 8px;
        }
        .card-accent { border-left: 3px solid var(--red); }

        /* NY Counter */
        .ny-counter {
            text-align: center; padding: 16px;
            background: linear-gradient(135deg, rgba(212,168,67,0.1), rgba(231,76,60,0.1));
            border: 2px solid var(--gold); border-radius: var(--radius); margin-bottom: 10px;
        }
        .ny-days { font-size: 42px; font-weight: 900; color: var(--gold); }
        .ny-label { font-size: 9px; color: var(--text2); text-transform: uppercase; letter-spacing: 2px; }

        /* Stats */
        .stats { display: grid; grid-template-columns: 1fr 1fr 1fr 1fr; gap: 6px; margin-bottom: 10px; }
        .stat { background: var(--card); border: 1px solid var(--border); border-radius: var(--radius); padding: 12px; text-align: center; }
        .stat-val { font-size: 20px; font-weight: 800; }
        .stat-lbl { font-size: 7px; color: var(--text2); text-transform: uppercase; letter-spacing: 1px; }

        /* Forms */
        .input, textarea {
            width: 100%; padding: 10px 14px; background: #0a0a14;
            border: 1px solid var(--border); border-radius: 10px;
            color: #fff; font-family: 'Montserrat', sans-serif; font-size: 12px;
            margin-bottom: 6px; transition: all 0.3s;
        }
        .input:focus, textarea:focus { outline: none; border-color: var(--red); }
        textarea { resize: vertical; min-height: 60px; }

        /* Buttons */
        .btn {
            padding: 10px 16px; border: none; border-radius: 10px;
            font-family: 'Montserrat', sans-serif; font-weight: 700; font-size: 11px;
            cursor: pointer; transition: all 0.3s; display: inline-flex;
            align-items: center; gap: 6px; text-transform: uppercase;
            letter-spacing: 0.5px; text-decoration: none;
        }
        .btn:active { transform: scale(0.96); }
        .btn-red { background: var(--red); color: #fff; }
        .btn-outline { background: transparent; border: 1px solid var(--border); color: var(--text); }
        .btn-gold { background: linear-gradient(135deg, #8b6914, var(--gold)); color: #000; }
        .btn-sm { padding: 5px 10px; font-size: 9px; }
        .btn-xs { padding: 3px 6px; font-size: 7px; }
        .btn-block { width: 100%; justify-content: center; }

        /* Badges */
        .badge {
            padding: 2px 6px; border-radius: 4px; font-size: 7px;
            font-weight: 800; text-transform: uppercase; color: #fff;
        }
        .badge-dev { background: linear-gradient(135deg, #8e44ad, #3498db); }
        .badge-admin { background: var(--red); }
        .badge-mod { background: var(--blue); }
        .badge-user { background: var(--green); }

        /* Chat */
        .chat-box { max-height: 350px; overflow-y: auto; display: flex; flex-direction: column; gap: 6px; margin-bottom: 8px; }
        .chat-msg { display: flex; gap: 6px; padding: 6px; background: rgba(255,255,255,0.02); border-radius: 8px; }
        .chat-msg img { width: 24px; height: 24px; border-radius: 6px; object-fit: cover; }

        /* Music Player */
        .music-bar {
            position: fixed; bottom: 0; left: 0; right: 0;
            background: rgba(14,14,26,0.98); backdrop-filter: blur(20px);
            border-top: 1px solid var(--gold); padding: 8px 16px;
            display: flex; align-items: center; gap: 8px; z-index: 100;
        }
        .music-btn {
            width: 30px; height: 30px; border-radius: 50%; border: none;
            background: var(--red); color: #fff; font-size: 10px;
            cursor: pointer; display: flex; align-items: center; justify-content: center;
        }
        .music-info { flex:1; font-size: 9px; color: var(--text2); overflow: hidden; text-overflow: ellipsis; white-space: nowrap; }
        .volume-slider { width: 60px; accent-color: var(--red); }

        /* Golden Ingot */
        .golden {
            max-width: 100%; margin: 0 auto;
            background: linear-gradient(160deg, #1a1000, #3d2b00 15%, #8b6914 30%, #d4a843 45%, #f0d078 55%, #d4a843 65%, #8b6914 80%, #3d2b00 90%, #1a1000);
            border-radius: 16px; padding: 20px 16px 30px;
            border: 2px solid var(--gold);
            box-shadow: 0 0 20px rgba(212,168,67,0.3);
        }
        .golden h2 { font-family: 'Playfair Display', serif; font-size: 18px; text-align: center; color: #1a0f00; margin-bottom: 14px; }
        .rule { display: flex; gap: 8px; padding: 6px 0; border-bottom: 1px solid rgba(0,0,0,0.2); }
        .rule-n { font-family: 'Playfair Display', serif; font-size: 22px; font-weight: 900; color: rgba(0,0,0,0.3); min-width: 24px; }
        .rule-t { font-size: 11px; font-weight: 800; color: #1a0f00; text-transform: uppercase; }
        .rule-d { font-size: 9px; color: #3d2b00; }
        .sign { text-align: right; margin-top: 16px; padding-top: 12px; border-top: 1px solid rgba(0,0,0,0.2); font-family: 'Playfair Display', serif; font-size: 16px; font-weight: 900; color: #1a0f00; }

        /* Modal */
        .modal {
            position: fixed; inset: 0; background: rgba(0,0,0,0.9); z-index: 200;
            display: none; align-items: center; justify-content: center; padding: 16px;
        }
        .modal.active { display: flex; }
        .modal-card {
            background: var(--surface); border: 1px solid var(--border);
            border-radius: var(--radius); padding: 24px; width: 100%; max-width: 360px;
            text-align: center;
        }

        /* Toast */
        .toast {
            position: fixed; top: 16px; left: 50%; transform: translateX(-50%);
            padding: 10px 20px; border-radius: 10px; font-size: 11px; font-weight: 600;
            z-index: 300; animation: fadeIn 0.3s ease;
        }
        .toast.ok { background: #1a3a2a; border: 1px solid var(--green); color: var(--green); }
        .toast.err { background: #3a1a1a; border: 1px solid var(--red); color: var(--red); }

        /* Snow */
        canvas#snow { position: fixed; top: 0; left: 0; pointer-events: none; z-index: 0; }

        ::-webkit-scrollbar { width: 3px; } ::-webkit-scrollbar-thumb { background: var(--border); border-radius: 2px; }
    </style>
</head>
<body>

<canvas id="snow"></canvas>
<div class="app">
    <!-- Header -->
    <header class="header">
        <div class="logo" onclick="showPage('home')">
            <div class="logo-icon">S</div>
            <div class="logo-text">Santa Workshop</div>
        </div>
        <nav class="nav-links">
            <button class="nav-link active" onclick="showPage('home')">🏠</button>
            <button class="nav-link" onclick="showPage('chat')">💬</button>
            <button class="nav-link" onclick="showPage('forum')">📋</button>
            <button class="nav-link" onclick="showPage('rules')">📜</button>
            <button class="nav-link admin-only" onclick="showPage('admin')" style="color:var(--gold);">⚡</button>
        </nav>
        <div>
            <span id="user-btn"></span>
        </div>
    </header>

    <!-- Content -->
    <div class="content">
        <!-- Home -->
        <div class="page active" id="page-home">
            <div class="ny-counter"><div class="ny-days" id="ny-days">0</div><div class="ny-label">дней до Нового года</div></div>
            <div class="stats" id="stats"></div>
            <div class="card"><h3 style="font-weight:800;margin-bottom:8px;">📰 Новости</h3><div id="news-list"></div></div>
        </div>

        <!-- Chat -->
        <div class="page" id="page-chat">
            <div class="card" style="display:flex;flex-direction:column;height:380px;">
                <h3 style="font-weight:800;margin-bottom:8px;">💬 Чат</h3>
                <div class="chat-box" id="chat-box"></div>
                <form onsubmit="sendChat(event)" style="display:flex;gap:4px;">
                    <input type="text" id="chat-input" class="input" placeholder="Сообщение..." style="margin:0;flex:1;" maxlength="300" required>
                    <button type="submit" class="btn btn-red">→</button>
                </form>
            </div>
        </div>

        <!-- Forum -->
        <div class="page" id="page-forum">
            <h3 style="font-weight:800;margin-bottom:8px;">📋 Форум</h3>
            <form onsubmit="createTopic(event)" style="display:flex;gap:4px;margin-bottom:8px;">
                <input type="text" id="topic-input" class="input" placeholder="Название темы..." style="margin:0;flex:1;" required>
                <button type="submit" class="btn btn-red">+</button>
            </form>
            <div class="card" id="forum-list"></div>
        </div>

        <!-- Rules -->
        <div class="page" id="page-rules">
            <div class="golden">
                <h2>📜 Кодекс Мастерской</h2>
                <div class="rule"><div class="rule-n">I</div><div><div class="rule-t">Уважение</div><div class="rule-d">Каждый эльф заслуживает уважения.</div></div></div>
                <div class="rule"><div class="rule-n">II</div><div><div class="rule-t">Чистота</div><div class="rule-d">Спам и реклама запрещены.</div></div></div>
                <div class="rule"><div class="rule-n">III</div><div><div class="rule-t">Тайна</div><div class="rule-d">Всё остаётся в Мастерской.</div></div></div>
                <div class="rule"><div class="rule-n">IV</div><div><div class="rule-t">Власть</div><div class="rule-d">Слово Santa — закон.</div></div></div>
                <div class="rule"><div class="rule-n">V</div><div><div class="rule-t">Ответ</div><div class="rule-d">3 предупреждения = мут.</div></div></div>
                <div class="rule"><div class="rule-n">VI</div><div><div class="rule-t">Добро</div><div class="rule-d">Помогай новичкам.</div></div></div>
                <div class="sign">Santa Claus</div>
            </div>
        </div>

        <!-- Admin -->
        <div class="page" id="page-admin">
            <h3 style="font-weight:800;margin-bottom:8px;color:var(--gold);">⚡ Админ-панель</h3>
            <div class="card" style="margin-bottom:8px;">
                <h4 style="font-weight:800;margin-bottom:6px;">📰 Добавить новость</h4>
                <form onsubmit="addNews(event)">
                    <input type="text" id="news-title" class="input" placeholder="Заголовок" required>
                    <textarea id="news-text" class="input" placeholder="Текст..." required></textarea>
                    <button type="submit" class="btn btn-gold btn-sm btn-block">Опубликовать</button>
                </form>
            </div>
            <div class="card"><h4 style="font-weight:800;margin-bottom:6px;">👥 Пользователи</h4><div id="admin-users"></div></div>
        </div>

        <!-- Profile -->
        <div class="page" id="page-profile">
            <div class="card" style="text-align:center;">
                <img id="prof-avatar" src="" style="width:70px;height:70px;border-radius:50%;border:3px solid var(--red);margin-bottom:6px;">
                <span id="prof-badge"></span>
                <h3 id="prof-name" style="font-weight:800;margin-top:4px;"></h3>
                <p id="prof-status" style="color:var(--text2);font-size:10px;"></p>
                <p style="color:var(--gold);font-size:9px;">⭐ Уровень: <span id="prof-level">1</span></p>
            </div>
            <div class="card">
                <h4 style="font-weight:800;margin-bottom:8px;">⚙️ Редактор</h4>
                <form onsubmit="saveProfile(event)">
                    <input type="text" id="edit-name" class="input" placeholder="Имя" required>
                    <input type="text" id="edit-status" class="input" placeholder="Статус">
                    <input type="text" id="edit-avatar" class="input" placeholder="URL аватарки">
                    <label style="font-size:9px;color:var(--text2);">Цвет ника</label>
                    <input type="color" id="edit-color" value="#e8e8f0" style="width:100%;height:36px;border:none;border-radius:8px;cursor:pointer;margin-bottom:6px;">
                    <input type="password" id="edit-pass" class="input" placeholder="Новый пароль (пусто = не менять)">
                    <button type="submit" class="btn btn-red btn-block btn-sm">💾 Сохранить</button>
                </form>
                <button onclick="logout()" class="btn btn-outline btn-block btn-sm" style="color:var(--red);border-color:var(--red);margin-top:6px;">🚪 Выйти</button>
            </div>
        </div>
    </div>

    <!-- Music Bar -->
    <div class="music-bar" id="music-bar">
        <button class="music-btn" onclick="prevTrack()"><i class="fa-solid fa-backward"></i></button>
        <button class="music-btn" id="play-btn" onclick="togglePlay()"><i class="fa-solid fa-play"></i></button>
        <button class="music-btn" onclick="nextTrack()"><i class="fa-solid fa-forward"></i></button>
        <span class="music-info" id="music-info">🎄 White Christmas</span>
        <span style="font-size:8px;color:var(--text2);" id="track-num">1/3</span>
        <input type="range" class="volume-slider" id="vol-slider" min="0" max="100" value="25" oninput="setVolume(this.value)">
    </div>
</div>

<script>
// ===== TELEGRAM WEB APP =====
const tg = window.Telegram?.WebApp;
if (tg) {
    tg.ready();
    tg.expand();
    tg.setHeaderColor('#050510');
    tg.setBackgroundColor('#050510');
}

// ===== DATA =====
const DB = {
    get(k, def) { try { return JSON.parse(localStorage.getItem('sw_'+k)) || def; } catch(e) { return def; } },
    set(k, v) { localStorage.setItem('sw_'+k, JSON.stringify(v)); }
};

let session = DB.get('session', null);
let users = DB.get('users', [
    { id:1, username:'Santa', password:'admin', role:'dev', avatar:'https://i.pravatar.cc/150?u=santa', status:'🎅 Создатель', nick_color:'#e74c3c', banned:false, muted:false, rating:999, level:99 }
]);
let messages = DB.get('chat', []);
let topics = DB.get('topics', []);
let news = DB.get('news', [
    { title:'🎄 Добро пожаловать!', text:'Santa Workshop запущен! Общайтесь в чате, создавайте темы.', date:'15.05.2026' },
    { title:'📜 Правила', text:'Ознакомьтесь с Кодексом Мастерской.', date:'15.05.2026' },
]);

function save() {
    DB.set('users', users);
    DB.set('chat', messages);
    DB.set('topics', topics);
    DB.set('news', news);
    if (session) DB.set('session', session);
}

// ===== MUSIC =====
const TRACKS = [
    { name:'🎄 Bing Crosby - White Christmas', url:'https://files.freemusicarchive.org/storage-freemusicarchive-org/music/no_curator/Tours/Enthusiastic_Tourist/Tours_-_01_-_Enthusiastic_Tourist.mp3' },
    { name:'🎅 Brenda Lee - Rockin Around', url:'https://files.freemusicarchive.org/storage-freemusicarchive-org/music/no_curator/Tours/Enthusiastic_Tourist/Tours_-_02_-_Enthusiastic_Tourist.mp3' },
    { name:'🌟 Nat King Cole - Christmas Song', url:'https://files.freemusicarchive.org/storage-freemusicarchive-org/music/ccCommunity/Chad_Crouch/Arps/Chad_Crouch_-_01_-_Arps.mp3' },
];
let curTrack = 0, playing = false;
const audio = new Audio();
audio.volume = DB.get('volume', 0.25);
document.getElementById('vol-slider').value = audio.volume * 100;

function loadTrack(i) {
    curTrack = i;
    audio.src = TRACKS[i].url;
    document.getElementById('music-info').innerText = TRACKS[i].name;
    document.getElementById('track-num').innerText = `${i+1}/${TRACKS.length}`;
    audio.load();
}
function togglePlay() {
    if (playing) { audio.pause(); document.getElementById('play-btn').innerHTML = '<i class="fa-solid fa-play"></i>'; }
    else { audio.play().catch(()=>{}); document.getElementById('play-btn').innerHTML = '<i class="fa-solid fa-pause"></i>'; }
    playing = !playing;
}
function nextTrack() { curTrack = (curTrack+1)%TRACKS.length; loadTrack(curTrack); if(playing) audio.play().catch(()=>{}); }
function prevTrack() { curTrack = (curTrack-1+TRACKS.length)%TRACKS.length; loadTrack(curTrack); if(playing) audio.play().catch(()=>{}); }
function setVolume(v) { audio.volume = v/100; DB.set('volume', audio.volume); }
audio.addEventListener('ended', ()=>{ nextTrack(); if(playing) audio.play().catch(()=>{}); });
loadTrack(0);

// ===== NAVIGATION =====
function showPage(id) {
    document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
    document.getElementById('page-'+id).classList.add('active');
    document.querySelectorAll('.nav-link').forEach(b => b.classList.remove('active'));
    event?.target?.classList.add('active');
    if (id === 'home') renderHome();
    if (id === 'chat') renderChat();
    if (id === 'forum') renderForum();
    if (id === 'admin') renderAdmin();
    if (id === 'profile') renderProfile();
}

// ===== RENDER =====
function renderHome() {
    const now = new Date(), ny = new Date(now.getFullYear()+1,0,1);
    document.getElementById('ny-days').innerText = Math.ceil((ny-now)/86400000);
    document.getElementById('stats').innerHTML = `
        <div class="stat"><div class="stat-val" style="color:var(--green);">⚡</div><div class="stat-lbl">Онлайн</div></div>
        <div class="stat"><div class="stat-val" style="color:var(--blue);">${messages.length}</div><div class="stat-lbl">Чат</div></div>
        <div class="stat"><div class="stat-val" style="color:var(--gold);">${topics.length}</div><div class="stat-lbl">Темы</div></div>
        <div class="stat"><div class="stat-val" style="color:var(--purple);">${users.filter(u=>!u.banned).length}</div><div class="stat-lbl">Эльфы</div></div>`;
    document.getElementById('news-list').innerHTML = news.slice(-5).reverse().map(n =>
        `<div style="padding:6px 0;border-bottom:1px solid var(--border);"><b style="color:var(--red);">${esc(n.title)}</b><span style="font-size:7px;color:var(--text2);margin-left:6px;">${n.date}</span><p style="font-size:10px;color:var(--text2);margin-top:2px;">${esc(n.text)}</p></div>`
    ).join('') || '<p style="color:var(--text2);">Нет новостей.</p>';
    updateUserBtn();
}

function renderChat() {
    document.getElementById('chat-box').innerHTML = messages.slice(-30).map(m =>
        `<div class="chat-msg"><img src="${m.avatar}" onerror="this.src='https://i.pravatar.cc/150?u=x'"><div><div style="display:flex;align-items:center;gap:3px;"><span class="badge badge-${m.role}">${m.role}</span><span style="font-weight:700;font-size:9px;color:${m.nick_color||'#e8e8f0'};">${esc(m.username)}</span><span style="font-size:7px;color:var(--text2);">${m.time}</span></div><p style="font-size:10px;margin-top:1px;">${esc(m.text)}</p></div></div>`
    ).join('') || '<p style="text-align:center;color:var(--text2);padding:20px;">💬 Нет сообщений.</p>';
    document.getElementById('chat-box').scrollTop = document.getElementById('chat-box').scrollHeight;
}

function sendChat(e) {
    e.preventDefault();
    if (!session) return toast('Войдите в профиль!', 'err');
    const inp = document.getElementById('chat-input');
    if (!inp.value.trim()) return;
    messages.push({
        username: session.username, role: session.role,
        avatar: session.avatar, nick_color: session.nick_color,
        text: inp.value.trim().substring(0, 300),
        time: new Date().toLocaleTimeString('ru-RU', {hour:'2-digit',minute:'2-digit'})
    });
    if (messages.length > 100) messages = messages.slice(-100);
    save(); inp.value = ''; renderChat(); renderHome();
}

function renderForum() {
    document.getElementById('forum-list').innerHTML = topics.length === 0 ? '<p style="color:var(--text2);">Нет тем.</p>' :
        topics.slice().reverse().map(t => `<div style="padding:6px 0;border-bottom:1px solid var(--border);"><b>${esc(t.title)}</b><div style="font-size:8px;color:var(--text2);">${esc(t.author)} • ${t.date}</div></div>`).join('');
}

function createTopic(e) {
    e.preventDefault();
    if (!session) return toast('Войдите!', 'err');
    const inp = document.getElementById('topic-input');
    if (!inp.value.trim()) return;
    topics.push({ title: inp.value.trim(), author: session.username, date: new Date().toLocaleDateString('ru-RU') });
    save(); inp.value = ''; renderForum(); renderHome();
    toast('Тема создана!', 'ok');
}

// ===== AUTH =====
function showLogin() {
    const modal = document.createElement('div');
    modal.className = 'modal active';
    modal.innerHTML = `
        <div class="modal-card" style="border-top:3px solid var(--red);">
            <div style="font-size:40px;">🎅</div>
            <h2 style="font-weight:800;margin:4px 0;">Вход</h2>
            <input type="text" id="login-user" class="input" placeholder="Логин">
            <input type="password" id="login-pass" class="input" placeholder="Пароль">
            <button class="btn btn-red btn-block" onclick="doLogin()">Войти</button>
            <button class="btn btn-outline btn-block btn-sm" style="margin-top:6px;" onclick="showRegister()">Создать аккаунт</button>
            <p style="font-size:8px;color:var(--text2);margin-top:6px;">Santa / admin</p>
        </div>`;
    document.body.appendChild(modal);
    modal.onclick = function(e) { if (e.target === modal) modal.remove(); };
}

function showRegister() {
    document.querySelector('.modal')?.remove();
    const modal = document.createElement('div');
    modal.className = 'modal active';
    modal.innerHTML = `
        <div class="modal-card" style="border-top:3px solid var(--green);">
            <div style="font-size:40px;">✨</div>
            <h2 style="font-weight:800;margin:4px 0;">Регистрация</h2>
            <input type="text" id="reg-user" class="input" placeholder="Логин">
            <input type="password" id="reg-pass" class="input" placeholder="Пароль">
            <input type="text" id="reg-status" class="input" placeholder="Статус (необязательно)">
            <label style="font-size:9px;color:var(--text2);display:block;margin-bottom:4px;">Цвет ника</label>
            <input type="color" id="reg-color" value="#e8e8f0" style="width:100%;height:36px;border:none;border-radius:8px;cursor:pointer;margin-bottom:6px;">
            <button class="btn btn-gold btn-block" onclick="doRegister()">Создать</button>
            <button class="btn btn-outline btn-block btn-sm" style="margin-top:6px;" onclick="showLogin()">Назад ко входу</button>
        </div>`;
    document.body.appendChild(modal);
    modal.onclick = function(e) { if (e.target === modal) modal.remove(); };
}

function doLogin() {
    const u = document.getElementById('login-user').value.trim();
    const p = document.getElementById('login-pass').value;
    const user = users.find(x => x.username === u && x.password === p);
    if (!user) return toast('Неверный логин или пароль', 'err');
    if (user.banned) return toast('Вы забанены', 'err');
    session = user;
    save();
    document.querySelector('.modal')?.remove();
    updateUserBtn();
    renderHome();
    toast(`Добро пожаловать, ${u}!`, 'ok');
}

function doRegister() {
    const u = document.getElementById('reg-user').value.trim();
    const p = document.getElementById('reg-pass').value;
    const s = document.getElementById('reg-status').value.trim() || '👤 Новый эльф';
    const c = document.getElementById('reg-color').value;
    if (u.length < 3) return toast('Логин от 3 символов', 'err');
    if (p.length < 4) return toast('Пароль от 4 символов', 'err');
    if (users.find(x => x.username === u)) return toast('Логин занят', 'err');
    users.push({
        id: Date.now(), username: u, password: p, role: 'user',
        avatar: `https://i.pravatar.cc/150?u=${encodeURIComponent(u)}`,
        status: s, nick_color: c, banned: false, muted: false, rating: 0, level: 1
    });
    save();
    document.querySelector('.modal')?.remove();
    toast('Аккаунт создан! Войдите.', 'ok');
    showLogin();
}

function logout() {
    session = null;
    DB.set('session', null);
    updateUserBtn();
    renderHome();
    showPage('home');
    toast('Вы вышли', 'ok');
}

function updateUserBtn() {
    const btn = document.getElementById('user-btn');
    if (session) {
        btn.innerHTML = `<span onclick="showPage('profile')" style="cursor:pointer;display:flex;align-items:center;gap:6px;background:var(--card);border:1px solid var(--border);padding:4px 10px 4px 4px;border-radius:30px;"><img src="${session.avatar}" style="width:26px;height:26px;border-radius:50%;"><span style="font-size:10px;font-weight:700;color:${session.nick_color};">${session.username}</span></span>`;
        document.querySelectorAll('.admin-only').forEach(e => e.style.display = (session.role==='dev'||session.role==='admin')?'inline-flex':'none');
    } else {
        btn.innerHTML = '<button class="btn btn-red btn-sm" onclick="showLogin()">Войти</button>';
        document.querySelectorAll('.admin-only').forEach(e => e.style.display = 'none');
    }
}

// ===== PROFILE =====
function renderProfile() {
    if (!session) return showLogin();
    document.getElementById('prof-avatar').src = session.avatar;
    document.getElementById('prof-badge').innerHTML = `<span class="badge badge-${session.role}">${session.role}</span>`;
    document.getElementById('prof-name').innerText = session.username;
    document.getElementById('prof-name').style.color = session.nick_color;
    document.getElementById('prof-status').innerText = session.status;
    document.getElementById('prof-level').innerText = `${session.level} (${session.rating})`;
    document.getElementById('edit-name').value = session.username;
    document.getElementById('edit-status').value = session.status;
    document.getElementById('edit-avatar').value = session.avatar;
    document.getElementById('edit-color').value = session.nick_color;
}

function saveProfile(e) {
    e.preventDefault();
    if (!session) return;
    const name = document.getElementById('edit-name').value.trim();
    const status = document.getElementById('edit-status').value.trim();
    const avatar = document.getElementById('edit-avatar').value.trim();
    const color = document.getElementById('edit-color').value;
    const pass = document.getElementById('edit-pass').value;
    if (name.length < 3) return toast('Имя от 3 символов', 'err');
    session.username = name;
    session.status = status || session.status;
    session.avatar = avatar || session.avatar;
    session.nick_color = color;
    if (pass && pass.length >= 4) session.password = pass;
    const idx = users.findIndex(u => u.id === session.id);
    if (idx >= 0) users[idx] = session;
    save(); renderProfile(); updateUserBtn();
    toast('Профиль обновлён!', 'ok');
}

// ===== ADMIN =====
function renderAdmin() {
    if (!session || (session.role!=='dev'&&session.role!=='admin')) return showPage('home');
    document.getElementById('admin-users').innerHTML = users.map(u => `
        <div style="display:flex;align-items:center;justify-content:space-between;padding:4px;background:rgba(0,0,0,0.2);border-radius:6px;margin-bottom:2px;flex-wrap:wrap;gap:2px;">
            <div><span style="font-weight:700;font-size:10px;color:${u.nick_color};">${esc(u.username)}</span><span class="badge badge-${u.banned?'banned':u.role}" style="margin-left:3px;">${u.banned?'BAN':u.role}</span></div>
            ${u.id !== session.id ? `
                <div style="display:flex;gap:2px;">
                    <select onchange="adminAction('role',${u.id},this.value)" style="background:#0a0a14;border:1px solid var(--border);color:#fff;padding:1px 2px;font-size:7px;border-radius:4px;">
                        <option value="user" ${u.role==='user'?'selected':''}>U</option>
                        <option value="mod" ${u.role==='mod'?'selected':''}>M</option>
                        <option value="admin" ${u.role==='admin'?'selected':''}>A</option>
                    </select>
                    <button onclick="adminAction('mute',${u.id})" class="btn btn-xs btn-outline">${u.muted?'🔊':'🔇'}</button>
                    <button onclick="adminAction('ban',${u.id})" class="btn btn-xs btn-outline" style="color:${u.banned?'var(--green)':'var(--red)'};">${u.banned?'✅':'🚫'}</button>
                </div>
            ` : '<span style="font-size:7px;color:var(--gold);">Вы</span>'}
        </div>
    `).join('');
}

function adminAction(action, id, value) {
    const user = users.find(u => u.id === id);
    if (!user) return;
    if (action === 'role') user.role = value;
    if (action === 'ban') user.banned = !user.banned;
    if (action === 'mute') user.muted = !user.muted;
    save(); renderAdmin(); renderHome();
}

function addNews(e) {
    e.preventDefault();
    const t = document.getElementById('news-title').value.trim();
    const x = document.getElementById('news-text').value.trim();
    if (!t || !x) return;
    news.push({ title: t, text: x, date: new Date().toLocaleDateString('ru-RU') });
    save();
    document.getElementById('news-title').value = '';
    document.getElementById('news-text').value = '';
    renderHome();
    toast('Новость добавлена!', 'ok');
}

// ===== HELPERS =====
function toast(msg, type) {
    const old = document.querySelector('.toast');
    if (old) old.remove();
    const t = document.createElement('div');
    t.className = `toast ${type}`; t.innerText = msg;
    document.body.appendChild(t);
    setTimeout(() => t.remove(), 2500);
}
function esc(s) { const d = document.createElement('div'); d.appendChild(document.createTextNode(s)); return d.innerHTML; }

// ===== SNOW =====
(function(){
    const c = document.getElementById('snow'), x = c.getContext('2d');
    let w, h, p = [];
    function i() { w = c.width = innerWidth; h = c.height = innerHeight; p = Array.from({length:40}, ()=>({x:Math.random()*w, y:Math.random()*h, r:Math.random()*2+0.5, d:Math.random()*0.5+0.2})); }
    function d() { x.clearRect(0,0,w,h); p.forEach(pp => { x.fillStyle='rgba(255,255,255,0.4)'; x.beginPath(); x.arc(pp.x,pp.y,pp.r,0,Math.PI*2); x.fill(); pp.y+=pp.d; if(pp.y>h+10){pp.y=-10;pp.x=Math.random()*w;} }); requestAnimationFrame(d); }
    addEventListener('resize', i); i(); d();
})();

// ===== INIT =====
updateUserBtn();
renderHome();
</script>

</body>
</html>