<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Wunduwatu Naratif Media</title>
<style>
  :root {
    --primary-color: #578ef3;
    --secondary-color: #d9f0c1;
    --accent-color: #f2982f;
    --bg-color: #f7f9f4;
    --text-color: #2c3e22;
    --button-bg: #4c9a2a;
    --button-hover-bg: #367313;
  }

  * {
    box-sizing: border-box;
  }

  body {
    margin: 0;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background-color: var(--bg-color);
    color: var(--text-color);
  }

  header {
    background: var(--primary-color);
    color: white;
    padding: 1.5rem;
    text-align: center;
    font-size: 1.8rem;
    font-weight: 700;
    box-shadow: 0 3px 6px rgba(0,0,0,0.15);
  }

  .container {
    max-width: 1100px;
    margin: auto;
    padding: 1rem;
    display: flex;
    flex-wrap: wrap;
    gap: 1.5rem;
  }

  main {
    flex: 2 1 600px;
    background: white;
    padding: 1.5rem;
    border-radius: 8px;
    box-shadow: 0 2px 8px rgb(0 0 0 / 0.1);
    display: flex;
    flex-direction: column;
    min-height: 500px;
  }

  main h2 {
    margin-top: 0;
    color: var(--primary-color);
  }

  #interaction-area {
    flex: 1;
    display: flex;
    flex-direction: column;
  }

  #messages {
    flex: 1;
    overflow-y: auto;
    border: 1px solid var(--secondary-color);
    padding: 0.8rem;
    border-radius: 6px;
    background: var(--secondary-color);
    margin-bottom: 0.8rem;
  }

  .message {
    background: #eaf2d7;
    border-radius: 5px;
    margin-bottom: 0.4rem;
    padding: 0.4rem 0.8rem;
    box-shadow: 1px 1px 3px rgba(0,0,0,0.05);
  }

  #message-form {
    display: flex;
    gap: 0.5rem;
  }

  #message-input {
    flex: 1;
    padding: 0.5rem 0.8rem;
    font-size: 1rem;
    border: 1px solid var(--secondary-color);
    border-radius: 6px;
    outline: none;
  }

  #message-input:focus {
    border-color: var(--accent-color);
    box-shadow: 0 0 5px var(--accent-color);
  }

  #send-btn {
    background: var(--button-bg);
    border: none;
    color: white;
    font-weight: 600;
    padding: 0 1rem;
    border-radius: 6px;
    cursor: pointer;
    transition: background 0.3s ease;
  }

  #send-btn:hover {
    background: var(--button-hover-bg);
  }

  aside {
    flex: 1 1 320px;
    background: white;
    padding: 1.5rem;
    border-radius: 8px;
    box-shadow: 0 2px 8px rgb(0 0 0 / 0.1);
    display: flex;
    flex-direction: column;
  }

  aside h2 {
    color: var(--primary-color);
    margin-top: 0;
    margin-bottom: 1rem;
  }

  .news-item {
    margin-bottom: 1rem;
    padding-bottom: 0.8rem;
    border-bottom: 1px solid #ddd;
  }

  .news-item:last-child {
    border-bottom: none;
  }

  .news-title {
    font-weight: 700;
    font-size: 1.1rem;
    margin-bottom: 0.3rem;
  }

  .news-date {
    font-size: 0.8rem;
    color: #666;
    margin-bottom: 0.4rem;
  }

  footer {
    background: var(--primary-color);
    padding: 1rem 0;
    text-align: center;
    color: white;
    margin-top: 2rem;
  }

  .social-shortcuts {
    max-width: 1100px;
    margin: 1.5rem auto 0;
    display: flex;
    justify-content: center;
    gap: 1.2rem;
  }

  .social-btn {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 44px;
    height: 44px;
    border-radius: 50%;
    color: white;
    font-size: 1.3rem;
    cursor: pointer;
    transition: transform 0.3s ease;
    text-decoration: none;
  }

  .social-btn:hover {
    transform: scale(1.15);
  }

  .fb { background: #1877f2; }
  .ig { background: #e4405f; }
  .x { background: #1da1f2; }
  .yt { background: #ff0000; }
  .tt { background: #69c9d0; }

  /* Scrollbar for messages */
  #messages::-webkit-scrollbar {
    width: 8px;
  }

  #messages::-webkit-scrollbar-track {
    background: var(--secondary-color);
    border-radius: 6px;
  }

  #messages::-webkit-scrollbar-thumb {
    background-color: var(--accent-color);
    border-radius: 6px;
  }

  @media (max-width: 768px) {
    .container {
      flex-direction: column;
    }
    main, aside {
      flex: unset;
      width: 100%;
    }
  }
</style>
<!-- Icon CDN -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" />
</head>
<body>
  <header>
    <h1>Wunduwatu Naratif Media</h1>
    <div class="social-shortcuts" aria-label="Tautan media sosial desa">
    <a href="https://www.facebook.com/profile.php?id=61576909111806" target="_blank" rel="noopener noreferrer" class="social-btn fb" aria-label="Facebook Desa Harmoni"><i class="fab fa-facebook-f"></i></a>
    <a href="https://www.instagram.com/wunduwatunaratifmedia/" target="_blank" rel="noopener noreferrer" class="social-btn ig" aria-label="Instagram Desa Harmoni"><i class="fab fa-instagram"></i></a>
    <a href="https://x.com/wunduwatunmedia" target="_blank" rel="noopener noreferrer" class="social-btn x" aria-label="X / Twitter Desa Harmoni"><i class="fab fa-twitter"></i></a>
    <a href="https://www.youtube.com/@WunduwatuNaratifMedia" target="_blank" rel="noopener noreferrer" class="social-btn yt" aria-label="YouTube Desa Harmoni"><i class="fab fa-youtube"></i></a>
    <a href="https://www.tiktok.com/@wunduwatunaratifmedia" target="_blank" rel="noopener noreferrer" class="social-btn tt" aria-label="TikTok Desa Harmoni"><i class="fab fa-tiktok"></i></a>
  </div>
   </header>
  <div class="container" role="main">
    <main>
      <h2>Interaksi Masyarakat</h2>
      <div id="interaction-area" aria-live="polite" aria-label="Area interaksi masyarakat desa">
        <div id="messages" aria-live="polite" aria-relevant="additions" aria-atomic="false" role="log" tabindex="0">
          <!-- Messages will appear here -->
        </div>
        <form id="message-form" aria-label="Form kirim pesan komunitas">
          <input type="text" id="message-input" aria-label="Masukkan pesan" autocomplete="off" placeholder="Tulis pesan..." required />
          <button type="submit" id="send-btn" aria-label="Kirim pesan">Kirim</button>
        </form>
      </div>
    </main>
    <aside aria-label="Berita desa terbaru">
      <h2>Berita Desa</h2>
      <article class="news-item" tabindex="0">
        <div class="news-title">Program Penghijauan Desa Sukses</div>
        <div class="news-date">15 Mei 2024</div>
        <div class="news-content">Masyarakat desa antusias mengikuti program penghijauan yang dilaksanakan minggu lalu.</div>
      </article>
      <article class="news-item" tabindex="0">
        <div class="news-title">Pelatihan Kewirausahaan untuk Pemuda</div>
        <div class="news-date">10 Mei 2024</div>
        <div class="news-content">Pelatihan bertujuan membekali pemuda dengan keterampilan bisnis.</div>
      </article>
      <article class="news-item" tabindex="0">
        <div class="news-title">Pasar Rakyat Kembali Dibuka Setiap Sabtu</div>
        <div class="news-date">8 Mei 2024</div>
        <div class="news-content">Pasar rakyat menghadirkan produk lokal segar langsung dari petani.</div>
      </article>
    </aside>
  </div>



  <footer>
    &copy; 2025 Wunduwatu Naratif Media
  </footer>

<script>
  const form = document.getElementById('message-form');
  const input = document.getElementById('message-input');
  const messagesDiv = document.getElementById('messages');

  // Load messages from localStorage
  function loadMessages() {
    const messages = JSON.parse(localStorage.getItem('villageMessages') || '[]');
    messagesDiv.innerHTML = '';
    messages.forEach(msg => {
      const msgDiv = document.createElement('div');
      msgDiv.classList.add('message');
      msgDiv.textContent = msg;
      messagesDiv.appendChild(msgDiv);
    });
    messagesDiv.scrollTop = messagesDiv.scrollHeight;
  }

  // Save messages to localStorage
  function saveMessage(message) {
    const messages = JSON.parse(localStorage.getItem('villageMessages') || '[]');
    messages.push(message);
    localStorage.setItem('villageMessages', JSON.stringify(messages));
  }

  form.addEventListener('submit', e => {
    e.preventDefault();
    const message = input.value.trim();
    if(message.length > 0){
      saveMessage(message);
      loadMessages();
      input.value = '';
      input.focus();
    }
  });

  // Initial load
  loadMessages();
</script>
</body>
</html>

