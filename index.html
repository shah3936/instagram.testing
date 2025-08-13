<!DOCTYPE html>
<html lang="hi">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>Instagram — Security Demo (Training)</title>
<style>
  :root{
    --insta-grad: linear-gradient(45deg,#feda75,#fa7e1e,#d62976,#962fbf,#4f5bd5);
    --card-bg: #fff;
    --muted:#8e8e8e;
    --blue:#0095f6;
  }
  *{box-sizing:border-box}
  body{
    margin:0;
    font-family:system-ui,-apple-system,Segoe UI,Roboto,Arial;
    background: #fafafa;
    display:flex;
    align-items:center;
    justify-content:center;
    min-height:100vh;
    padding:20px;
  }
  .wrap{
    width:100%;
    max-width:380px;
  }

  .phone {
    background:var(--card-bg);
    border:1px solid #dbdbdb;
    border-radius:12px;
    box-shadow:0 8px 20px rgba(0,0,0,0.06);
    padding:22px;
    text-align:center;
  }

  .brand {
    margin: 6px 0 14px;
    display:flex;
    align-items:center;
    justify-content:center;
    gap:10px;
  }
  .logo {
    width:44px;height:44px;border-radius:10px;
    background:var(--insta-grad);
    display:flex;align-items:center;justify-content:center;color:white;font-weight:700;
    box-shadow:0 4px 10px rgba(0,0,0,0.08);
    font-family: 'Segoe UI', Roboto, Arial;
  }
  .title { font-size:18px; font-weight:700; color:#262626; }

  form{margin-top:6px; text-align:left}
  label{display:block;font-size:12px;color:var(--muted);margin:8px 0 6px}
  input[type="text"], input[type="password"]{
    width:100%; padding:12px 12px; border-radius:8px; border:1px solid #dbdbdb;
    background:#fff; font-size:14px;
  }
  .btn{
    width:100%; padding:12px;border-radius:8px;border:none;margin-top:12px;
    background:var(--blue);color:#fff;font-weight:700;font-size:15px;cursor:pointer;
  }
  .small{font-size:13px;color:var(--muted);margin-top:10px;text-align:center}

  .note {
    margin-top:12px;padding:10px;border-radius:8px;background:#fff8e1;border:1px solid #ffecb3;color:#5a3711;font-size:13px;
  }

  /* Modal */
  .modal-backdrop{position:fixed;inset:0;display:none;align-items:center;justify-content:center;background:rgba(0,0,0,0.45);padding:20px}
  .modal{background:#fff;border-radius:12px;max-width:640px;padding:18px;box-shadow:0 12px 40px rgba(0,0,0,0.3)}
  .modal h3{margin:0 0 8px;color:#c62828}
  .tips{margin:8px 0 0;padding-left:18px}

  /* Attempts panel */
  .attempts{
    margin-top:12px;border-radius:8px;border:1px dashed #e0e0e0;padding:10px;background:#fbfbfb;font-size:13px;color:#333;
  }

  /* Responsive small */
  @media (max-width:420px){
    .wrap{padding:6px}
    .phone{padding:16px}
  }
</style>
</head>
<body>

<div class="wrap">
  <div class="phone" role="main" aria-labelledby="heading">
    <div class="brand">
      <div class="logo" aria-hidden="true">In</div>
      <div>
        <div id="heading" class="title">Instagram</div>
        <div style="font-size:12px;color:var(--muted)">Security Awareness Demo</div>
      </div>
    </div>

    <form id="demoForm" autocomplete="off" novalidate>
      <label for="user">Phone, username or email</label>
      <input id="user" name="user" type="text" placeholder="उदा: username@example.com" required />

      <label for="pass">Password</label>
      <input id="pass" name="pass" type="password" placeholder="Password" required />

      <button class="btn" type="submit">Log In</button>

      <div class="small" style="margin-top:8px">यह केवल प्रशिक्षण के लिए है — कोई भी डाटा कहीं भेजा नहीं जाएगा।</div>

      <div id="protocolWarning" class="note" style="display:none; margin-top:12px;">
        चेतावनी: यह पेज वेब पर होस्ट किया गया प्रतीत होता है। कृपया इस डेमो को सार्वजनिक सर्वर पर न रखें — केवल ऑफलाइन/लोकल ट्रेनिंग के लिए ही उपयोग करें।
      </div>

      <div id="attemptsPanel" class="attempts" style="display:none">
        <strong>ट्रेनिंग रिकॉर्ड (सत्र):</strong>
        <div id="attemptsList"></div>
      </div>
    </form>
  </div>
</div>

<!-- Modal (after submit) -->
<div class="modal-backdrop" id="modal" aria-hidden="true">
  <div class="modal" role="dialog" aria-labelledby="modTitle">
    <h3 id="modTitle">सावधान! यह प्रशिक्षण/डेमो पेज है</h3>
    <p>आपने अभी एक नकली-लॉगिन जैसा टेम्पलेट भरा — ध्यान रखें कि असली फिशिंग पेज दिखने में यही जैसा होते हैं। असली क्रेडेंशियल कभी भी किसी लिंक से भर कर ना दें।</p>
    <ul class="tips">
      <li>हमेशा URL और डोमेन की जाँच करें — <code>instagram.com</code> ही होना चाहिए।</li>
      <li>किसी भी ईमेल/मैसेज के लिंक से लॉगिन करने से बचें; ब्राउज़र में खुद वेबसाइट टाइप करें।</li>
      <li>मल्टिफैक्टर ऑथेंटिकेशन (MFA) ऑन रखें।</li>
      <li>पासवर्ड मैनेजर का उपयोग करें — यह नकली साइटें पहचानने में मदद करता है।</li>
    </ul>

    <p style="margin-top:10px;font-size:13px;color:#555">नीचे दिए गए बटनों में से चुनें:</p>
    <div style="display:flex;gap:10px;flex-wrap:wrap;margin-top:8px">
      <button id="closeBtn" style="flex:1;padding:10px;border-radius:8px;border:none;background:#0095f6;color:white;cursor:pointer">समझ गया</button>
      <button id="showInputBtn" style="flex:1;padding:10px;border-radius:8px;border:1px solid #ccc;background:#fff;cursor:pointer">मैंने क्या भरा था?</button>
    </div>
  </div>
</div>

<script>
/*
  Ethical demo behavior:
  - preventDefault() so nothing is sent.
  - Clear inputs after submit.
  - Show modal with tips.
  - Keep an in-memory (non-persistent) list of attempts for this session only.
  - If page is loaded over http/https, show protocol warning (do not host publicly).
*/

(function(){
  const form = document.getElementById('demoForm');
  const modal = document.getElementById('modal');
  const closeBtn = document.getElementById('closeBtn');
  const showInputBtn = document.getElementById('showInputBtn');
  const attemptsPanel = document.getElementById('attemptsPanel');
  const attemptsList = document.getElementById('attemptsList');
  const protocolWarning = document.getElementById('protocolWarning');

  // show warning if served over http(s)
  if (location.protocol === 'http:' || location.protocol === 'https:') {
    protocolWarning.style.display = 'block';
  }

  // in-memory attempts (not stored anywhere)
  const attempts = [];

  form.addEventListener('submit', function(e){
    e.preventDefault();

    const user = form.user.value || '(empty)';
    const passLen = form.pass.value ? form.pass.value.length : 0;

    // push safe summary only (no real credentials)
    attempts.push({
      time: new Date().toLocaleTimeString(),
      userShown: summarize(user),
      passLength: passLen
    });

    renderAttempts();

    // clear inputs immediately
    form.user.value = '';
    form.pass.value = '';

    // show modal (training tips)
    modal.style.display = 'flex';
    modal.setAttribute('aria-hidden','false');
  });

  function summarize(u){
    // show first 3 chars and mask rest to avoid storing actual username
    if (u === '(empty)') return u;
    const safe = u.slice(0,3);
    return safe + '…';
  }

  function renderAttempts(){
    attemptsPanel.style.display = 'block';
    attemptsList.innerHTML = '';
    attempts.slice().reverse().forEach((a, idx) => {
      const div = document.createElement('div');
      div.style.padding = '6px 0';
      div.style.borderBottom = '1px dashed #eee';
      div.innerHTML = `<strong>${a.time}</strong> — User: <code>${a.userShown}</code> • Password length: ${a.passLength}`;
      attemptsList.appendChild(div);
    });
  }

  closeBtn.addEventListener('click', function(){
    modal.style.display = 'none';
    modal.setAttribute('aria-hidden','true');
  });

  showInputBtn.addEventListener('click', function(){
    // show a small summary alert — safe (no real data shown)
    const last = attempts[attempts.length - 1];
    if (!last) {
      alert('कोई अभी तक सबमिट नहीं किया।');
      return;
    }
    alert('आपने भरा (सारांश):\\nTime: ' + last.time + '\\nUser prefix: ' + last.userShown + '\\nPassword length: ' + last.passLength);
  });

  // close modal on Esc
  document.addEventListener('keydown', function(e){
    if (e.key === 'Escape') {
      modal.style.display = 'none';
      modal.setAttribute('aria-hidden','true');
    }
  });

})();
</script>

</body>
</html>
