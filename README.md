[airaykinz.html](https://github.com/user-attachments/files/28175934/airaykinz.html)<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1">
<title>AirAykinz</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;800;900&display=swap');
*{margin:0;padding:0;box-sizing:border-box}
body{font-family:'Inter',system-ui,sans-serif;background:#f0f0eb;min-height:100vh;color:#1a2744}

/* ─── HEADER ─── */
.hdr{background:#1a2744;padding:14px 24px;display:flex;align-items:center;justify-content:space-between;border-bottom:4px solid #E85D04}
.logo{display:flex;align-items:center;gap:8px}
.logo-ico{font-size:20px;color:#E85D04}
.logo-txt{font-size:22px;font-weight:900;color:#fff;letter-spacing:-0.02em}
.hdr-tag{font-size:10px;color:rgba(255,255,255,.45);font-weight:700;text-transform:uppercase;letter-spacing:.1em}

/* ─── GENERATOR ─── */
.gen{max-width:820px;margin:0 auto;padding:24px 16px 60px}
.fc{background:#fff;border-radius:14px;padding:22px 24px;margin-bottom:16px;border:1px solid #ebebeb}
.fc-title{font-size:10px;font-weight:900;text-transform:uppercase;letter-spacing:.12em;color:#E85D04;margin-bottom:16px}
.fg{display:grid;gap:11px}
.c2{grid-template-columns:1fr 1fr}
.c3{grid-template-columns:1fr 1fr 1fr}
.c4{grid-template-columns:1fr 1fr 1fr 1fr}
.field{display:flex;flex-direction:column;gap:4px}
.field label{font-size:10px;font-weight:800;text-transform:uppercase;letter-spacing:.08em;color:#c0c0c0}
.field input,.field select{font-size:14px;font-weight:700;padding:9px 11px;border:1.5px solid #eee;border-radius:9px;background:#fafafa;color:#1a2744;font-family:'Inter',sans-serif;transition:border-color .12s}
.field input:focus,.field select:focus{outline:none;border-color:#E85D04;background:#fff}
.field input.iata{text-transform:uppercase;font-size:17px;font-weight:900}
.pax-block{border:1.5px solid #f0f0f0;border-radius:10px;padding:14px 16px;margin-bottom:10px}
.pax-num{font-size:10px;font-weight:900;color:#E85D04;text-transform:uppercase;letter-spacing:.1em;margin-bottom:10px;display:flex;justify-content:space-between;align-items:center}
.rm-btn{background:none;border:none;color:#ddd;cursor:pointer;font-size:20px;line-height:1;font-family:sans-serif}
.rm-btn:hover{color:#E85D04}
.add-btn{display:inline-flex;align-items:center;gap:5px;padding:8px 14px;border:1.5px dashed #e0e0e0;border-radius:8px;background:none;color:#bbb;font-size:12px;font-weight:700;cursor:pointer;font-family:'Inter',sans-serif;margin-top:4px;transition:all .12s}
.add-btn:hover{border-color:#E85D04;color:#E85D04}
.gen-btn{width:100%;padding:15px;background:#1a2744;color:#fff;border:none;border-radius:12px;font-size:14px;font-weight:900;text-transform:uppercase;letter-spacing:.1em;cursor:pointer;font-family:'Inter',sans-serif;margin-top:4px;transition:background .15s}
.gen-btn:hover{background:#E85D04}
.gen-btn:active{opacity:.9}

/* hosting tip */
.tip{background:#fff8f0;border:1.5px solid #E85D04;border-radius:12px;padding:14px 18px;margin-bottom:20px;font-size:13px;color:#555;line-height:1.7}
.tip strong{color:#E85D04}
.tip a{color:#E85D04;font-weight:700}

/* ─── BOARDING PASS ─── */
.bp-section{margin-top:28px}
.bp-lbl{font-size:10px;font-weight:900;text-transform:uppercase;letter-spacing:.12em;color:#aaa;margin-bottom:14px}
.bp{background:#fff;border-radius:14px;display:grid;grid-template-columns:1fr 160px;overflow:hidden;border:1px solid #e8e8e8;box-shadow:0 2px 14px rgba(0,0,0,.06);margin-bottom:8px}
.bp-main{}
.bp-bar{height:5px;background:#E85D04}
.bp-body{padding:20px 24px}
.bp-head{display:flex;align-items:flex-start;justify-content:space-between;margin-bottom:16px}
.bp-logo{display:flex;align-items:center;gap:7px}
.bp-logo-i{font-size:17px;color:#E85D04}
.bp-logo-t{font-size:20px;font-weight:900;color:#1a2744;letter-spacing:-0.02em}
.bp-head-r{font-size:8px;font-weight:700;color:#bbb;text-align:right;letter-spacing:.1em;text-transform:uppercase;line-height:1.6}
.bp-pax-l{font-size:8px;font-weight:800;color:#bbb;text-transform:uppercase;letter-spacing:.1em;margin-bottom:2px}
.bp-pax-n{font-size:19px;font-weight:900;color:#1a2744;letter-spacing:-.01em;margin-bottom:12px}
.bp-meta{display:grid;grid-template-columns:1fr 1fr;gap:3px 20px;margin-bottom:12px}
.bp-ml{font-size:8px;font-weight:700;color:#bbb;text-transform:uppercase;letter-spacing:.08em}
.bp-mv{font-size:12px;font-weight:800;color:#1a2744}
.route{display:flex;align-items:center;gap:8px;margin-bottom:12px}
.ap{flex:1}.ap.r{text-align:right}
.ap-l{font-size:8px;font-weight:700;color:#bbb;text-transform:uppercase;letter-spacing:.08em;margin-bottom:1px}
.ap-c{font-size:24px;font-weight:900;color:#1a2744;letter-spacing:-.02em;line-height:1}
.ap-n{font-size:9px;color:#aaa;margin-top:1px}
.ap-ci{font-size:9px;font-weight:700;color:#1a2744;margin-top:1px}
.pl{font-size:17px;color:#1a2744;flex-shrink:0;padding:0 4px}
.info-row{display:grid;grid-template-columns:auto 1fr 1fr 1fr 1fr;border:1.5px solid #1a2744;border-radius:8px;overflow:hidden;margin-bottom:10px}
.ic{padding:8px 11px;border-right:1px solid #e4e4e4}.ic:last-child{border-right:none}
.ic-l{font-size:7px;font-weight:800;text-transform:uppercase;letter-spacing:.08em;color:#bbb;margin-bottom:3px}
.ic-v{font-size:14px;font-weight:900;color:#1a2744;line-height:1}
.ic-s{font-size:7px;color:#bbb;margin-top:1px}
.ic.gate{background:#1a2744;padding:8px 13px}
.ic.gate .ic-l{color:rgba(255,255,255,.5)}
.ic.gate .ic-v{color:#fff;font-size:16px}
.seat-v{color:#E85D04!important}
.bp-foot{font-size:7px;font-weight:800;color:#E85D04;text-transform:uppercase;letter-spacing:.06em;border-top:1px solid #f4f4f4;padding:8px 24px}

/* STUB */
.stub{border-left:2px dashed #e4e4e4;display:flex;flex-direction:column}
.stub-bar{height:5px;background:#E85D04}
.stub-body{padding:12px 11px;flex:1;display:flex;flex-direction:column;gap:7px}
.stub-logo{display:flex;align-items:center;gap:4px;margin-bottom:2px}
.stub-logo-i{font-size:12px;color:#E85D04}
.stub-logo-t{font-size:12px;font-weight:900;color:#1a2744;letter-spacing:-.01em}
.si .sl{font-size:7px;font-weight:800;text-transform:uppercase;letter-spacing:.1em;color:#bbb}
.si .sv{font-size:11px;font-weight:800;color:#1a2744}
.si .sv.o{color:#E85D04}
.si-row{display:grid;grid-template-columns:1fr 1fr;gap:6px}
.stub-qr{padding:10px 11px;border-top:1px solid #f4f4f4;display:flex;flex-direction:column;align-items:center;gap:5px}
.stub-qr canvas{border-radius:5px;display:block}
.stub-hint{font-size:7px;font-weight:700;color:#bbb;text-transform:uppercase;letter-spacing:.08em;text-align:center}

/* URL box */
.url-box{background:#fff;border-radius:10px;padding:11px 14px;border:1px solid #ebebeb;margin-bottom:20px;display:flex;align-items:center;gap:10px;flex-wrap:wrap}
.url-box code{font-family:ui-monospace,monospace;font-size:10px;color:#1a2744;word-break:break-all;flex:1;min-width:0}
.cp-btn{flex-shrink:0;padding:6px 11px;border-radius:7px;border:1.5px solid #eee;background:#fafafa;color:#999;font-size:11px;font-weight:700;cursor:pointer;font-family:'Inter',sans-serif;white-space:nowrap}
.cp-btn:hover{border-color:#E85D04;color:#E85D04}

/* ─── VALIDATOR ─── */
.val-wrap{max-width:440px;margin:0 auto;padding:20px 16px 48px}
.val-card{background:#fff;border-radius:18px;overflow:hidden;box-shadow:0 4px 28px rgba(0,0,0,.1);margin-bottom:14px}
.val-banner{padding:32px 24px 24px;text-align:center}
.v-ico{font-size:56px;margin-bottom:12px}
.v-ttl{font-size:24px;font-weight:900;color:#fff;margin-bottom:5px;letter-spacing:-.01em}
.v-sub{font-size:14px;color:rgba(255,255,255,.78);font-weight:500}
.v-ok .val-banner{background:#1a2744}
.v-err .val-banner{background:#b92b2b}
.v-wait .val-banner{background:#888}
.val-body{padding:18px 22px}
.v-route{display:flex;justify-content:space-between;align-items:center;padding:14px 0;border-bottom:1px solid #f0f0f0;margin-bottom:4px}
.v-ap{font-size:32px;font-weight:900;color:#1a2744}
.v-ap-l{font-size:9px;color:#aaa;text-transform:uppercase;letter-spacing:.08em;font-weight:700;margin-bottom:2px}
.v-row{display:flex;justify-content:space-between;align-items:center;padding:10px 0;border-bottom:1px solid #f5f5f5;font-size:14px}
.v-row:last-child{border-bottom:none}
.v-lbl{color:#aaa;font-weight:600;font-size:12px;text-transform:uppercase;letter-spacing:.05em}
.v-val{font-weight:800;color:#1a2744}
.v-val.big{color:#E85D04;font-size:18px}
.v-notice{font-size:12px;color:#aaa;text-align:center;padding:12px 16px;line-height:1.7;background:#fff;border-radius:12px;border:1px solid #ebebeb}
.v-scan{background:#f8f8f5;border-radius:11px;padding:13px 16px;margin-bottom:12px;font-size:13px;color:#666;line-height:1.6}
.v-scan b{color:#1a2744}

@media(max-width:600px){
  .bp{grid-template-columns:1fr}.stub{border-left:none;border-top:2px dashed #e4e4e4}
  .c3,.c4{grid-template-columns:1fr 1fr}
  .info-row{grid-template-columns:auto 1fr 1fr 1fr}
}
</style>
</head>
<body>

<div class="hdr">
  <div class="logo"><span class="logo-ico">✈</span><span class="logo-txt">AirAykinz</span></div>
  <span class="hdr-tag" id="hdr-tag">Générateur</span>
</div>

<!-- ═══════════════ GENERATOR VIEW ═══════════════ -->
<div class="gen" id="view-gen">

  <div class="tip">
    <strong>📡 Pour scanner depuis un iPhone :</strong> mets ce fichier en ligne sur 
    <a href="https://tiiny.host" target="_blank">tiiny.host</a> 
    (glisse-dépose → URL publique en 10 secondes, sans compte) puis utilise cette URL dans le champ ci-dessous.
    <br><br>
    <strong>URL de ce fichier en ligne :</strong>
    <input type="text" id="base-url" placeholder="https://xxxx.tiiny.site/airaykinz.html" 
      style="width:100%;margin-top:6px;font-size:13px;padding:8px 11px;border:1.5px solid #E85D04;border-radius:8px;font-family:'Inter',sans-serif;color:#1a2744;background:#fff">
    <span style="font-size:11px;color:#aaa">⬆ Colle ici l'URL que tiiny.host te donne, puis génère tes billets</span>
  </div>

  <div class="fc">
    <div class="fc-title">Informations du vol</div>
    <div class="fg c4" style="margin-bottom:11px">
      <div class="field"><label>N° de vol</label><input id="flight" value="AYK180"></div>
      <div class="field"><label>Date</label><input id="fdate" type="date" value="2026-06-21"></div>
      <div class="field"><label>Heure départ</label><input id="dep" type="time" value="18:00"></div>
      <div class="field"><label>Heure arrivée</label><input id="arr" type="time" value="20:00"></div>
    </div>
    <div class="fg c2" style="margin-bottom:11px">
      <div style="display:grid;grid-template-columns:85px 1fr;gap:9px;align-items:end">
        <div class="field"><label>IATA départ</label><input class="iata" id="fc" maxlength="4" value="LFQQ"></div>
        <div class="field"><label>Aéroport départ</label><input id="fn" value="Lille-Lesquin Airport"></div>
      </div>
      <div style="display:grid;grid-template-columns:85px 1fr;gap:9px;align-items:end">
        <div class="field"><label>IATA arrivée</label><input class="iata" id="tc" maxlength="4" value="LFQQ"></div>
        <div class="field"><label>Aéroport arrivée</label><input id="tn" value="Lille-Lesquin Airport"></div>
      </div>
    </div>
    <div class="fg c3">
      <div class="field"><label>Porte / Gate</label><input id="gate" value="CALM E"></div>
      <div class="field"><label>Classe</label>
        <select id="cabin"><option>ECONOMY</option><option>BUSINESS</option><option>FIRST</option></select>
      </div>
      <div class="field"><label>Ville</label><input id="fcity" value="Lille-Lesquin"></div>
    </div>
  </div>

  <div class="fc">
    <div class="fc-title">Passagers</div>
    <div id="pax-list"></div>
    <button class="add-btn" onclick="addPax()">+ Ajouter un passager</button>
  </div>

  <button class="gen-btn" onclick="generateAll()">✈ Générer les cartes d'embarquement</button>

  <div id="bp-out" style="display:none">
    <div class="bp-section">
      <div class="bp-lbl">Cartes d'embarquement</div>
      <div id="passes"></div>
    </div>
  </div>
</div>

<!-- ═══════════════ VALIDATOR VIEW ═══════════════ -->
<div class="val-wrap" id="view-val" style="display:none">
  <div class="val-card v-wait" id="vc">
    <div class="val-banner">
      <div class="v-ico" id="vi">⏳</div>
      <div class="v-ttl" id="vt">Vérification…</div>
      <div class="v-sub" id="vs">Analyse du billet en cours</div>
    </div>
    <div class="val-body" id="vb"></div>
  </div>
  <div class="v-scan" id="vscan" style="display:none">📱 Billet scanné le <b id="vtime"></b></div>
  <div class="v-notice" id="vn"></div>
</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/qrcodejs/1.0.0/qrcode.min.js"></script>
<script>
// ── ROUTING ──────────────────────────────────────────
var params = new URLSearchParams(location.search);
var isValidator = params.get('flight') || params.get('scan');

if (isValidator) {
  document.getElementById('view-gen').style.display = 'none';
  document.getElementById('view-val').style.display = 'block';
  document.getElementById('hdr-tag').textContent = 'Vérification billet';
  runValidator();
} else {
  initGenerator();
}

// ── GENERATOR ─────────────────────────────────────────
var pIdx = 0;

function initGenerator() {
  addPax('PIERRICK','','12A');
  addPax('JOSEPHINE','','12B');
}

function addPax(first, last, seat) {
  pIdx++;
  var i = pIdx;
  var d = document.createElement('div');
  d.className = 'pax-block'; d.id = 'pb-'+i;
  d.innerHTML = '<div class="pax-num">Passager ' + i
    + (i > 1 ? '<button class="rm-btn" onclick="document.getElementById(\'pb-'+i+'\').remove()">×</button>' : '')
    + '</div><div class="fg c3">'
    + '<div class="field"><label>Prénom</label><input id="pf-'+i+'" value="'+(first||'')+'" placeholder="PIERRICK"></div>'
    + '<div class="field"><label>Nom</label><input id="pl-'+i+'" value="'+(last||'')+'" placeholder="AYKIN"></div>'
    + '<div class="field"><label>Siège</label><input id="ps-'+i+'" value="'+(seat||'')+'" placeholder="12A"></div>'
    + '</div>';
  document.getElementById('pax-list').appendChild(d);
}

function getPax() {
  var list = [];
  document.querySelectorAll('.pax-block').forEach(function(b) {
    var i = b.id.replace('pb-','');
    var f = document.getElementById('pf-'+i), l = document.getElementById('pl-'+i), s = document.getElementById('ps-'+i);
    if (f && (f.value || (l && l.value))) list.push({first:f.value, last:l.value, seat:s.value, seq:list.length+1});
  });
  return list;
}

function fd(d) {
  if (!d) return '';
  var a = d.split('-'), m = ['JAN','FEB','MAR','APR','MAY','JUN','JUL','AUG','SEP','OCT','NOV','DEC'];
  return parseInt(a[2]) + ' ' + m[parseInt(a[1])-1] + ' ' + a[0];
}

function mkid(n) { return Math.random().toString(36).substring(2, 2+n).toUpperCase(); }

function buildUrl(pax, seq, ref) {
  var base = (document.getElementById('base-url').value || '').trim();
  if (!base) base = location.href.split('?')[0]; // same file
  // clean up
  if (!base.includes('airaykinz')) {
    base = base.replace(/\/?$/, '') + '/airaykinz.html';
  }
  var p = new URLSearchParams({
    flight: document.getElementById('flight').value,
    date: document.getElementById('fdate').value,
    time: document.getElementById('dep').value,
    from: document.getElementById('fc').value.toUpperCase(),
    to: document.getElementById('tc').value.toUpperCase(),
    fromCity: document.getElementById('fcity').value,
    seat: pax.seat,
    gate: document.getElementById('gate').value,
    passenger: (pax.first.toUpperCase() + ' ' + pax.last.toUpperCase()).trim(),
    cabin: document.getElementById('cabin').value,
    ref: ref,
    seq: String(seq).padStart(3,'0'),
    scan: '1'
  });
  return base + '?' + p.toString();
}

function generateAll() {
  var paxList = getPax();
  if (!paxList.length) { alert('Ajoutez au moins un passager.'); return; }
  var passes = document.getElementById('passes');
  passes.innerHTML = '';
  var ref = mkid(6);
  paxList.forEach(function(pax) {
    var div = document.createElement('div');
    passes.appendChild(div);
    renderPass(div, pax, buildUrl(pax, pax.seq, ref), ref);
  });
  document.getElementById('bp-out').style.display = 'block';
  setTimeout(function() { document.getElementById('bp-out').scrollIntoView({behavior:'smooth'}); }, 100);
}

function renderPass(container, pax, url, ref) {
  var flight = document.getElementById('flight').value;
  var fdate = document.getElementById('fdate').value;
  var dep = document.getElementById('dep').value;
  var arr = document.getElementById('arr').value;
  var fr = document.getElementById('fc').value.toUpperCase();
  var frn = document.getElementById('fn').value;
  var frc = document.getElementById('fcity').value;
  var to = document.getElementById('tc').value.toUpperCase();
  var ton = document.getElementById('tn').value;
  var gate = document.getElementById('gate').value;
  var cabin = document.getElementById('cabin').value;
  var pname = (pax.first.toUpperCase() + ' ' + pax.last.toUpperCase()).trim() || 'PASSAGER';
  var seq = String(pax.seq).padStart(3,'0');
  var qid = 'qr-' + seq + '-' + Date.now();

  container.innerHTML =
    '<div class="bp">'
    +'<div class="bp-main">'
    +'<div class="bp-bar"></div>'
    +'<div class="bp-body">'
    +'<div class="bp-head"><div class="bp-logo"><span class="bp-logo-i">✈</span><span class="bp-logo-t">AirAykinz</span></div><div class="bp-head-r">CARTE D\'EMBARQUEMENT<br>BOARDING PASS</div></div>'
    +'<div class="bp-pax-l">PASSAGER / PASSENGER</div><div class="bp-pax-n">'+pname+'</div>'
    +'<div class="bp-meta"><div><div class="bp-ml">VOL / FLIGHT</div><div class="bp-mv">'+flight+'</div></div><div><div class="bp-ml">DATE</div><div class="bp-mv">'+fd(fdate)+'</div></div></div>'
    +'<div class="route">'
    +'<div class="ap"><div class="ap-l">DÉPART / FROM</div><div class="ap-c">'+fr+'</div><div class="ap-ci">'+frc.toUpperCase()+'</div><div class="ap-n">'+frn+'</div></div>'
    +'<div class="pl">✈</div>'
    +'<div class="ap r"><div class="ap-l">ARRIVÉE / TO</div><div class="ap-c">'+to+'</div><div class="ap-ci">'+frc.toUpperCase()+'</div><div class="ap-n">'+ton+'</div></div>'
    +'</div>'
    +'<div class="info-row">'
    +'<div class="ic gate"><div class="ic-l">EMBARQUEMENT / GATE</div><div class="ic-v">'+gate+'</div></div>'
    +'<div class="ic"><div class="ic-l">DÉCOLLAGE / DEPARTURE</div><div class="ic-v">'+dep+'</div><div class="ic-s">heure locale</div></div>'
    +'<div class="ic"><div class="ic-l">ARRIVÉE / ARRIVAL</div><div class="ic-v">'+arr+'</div><div class="ic-s">heure locale</div></div>'
    +'<div class="ic"><div class="ic-l">CLASSE / CLASS</div><div class="ic-v" style="font-size:11px">'+cabin+'</div></div>'
    +'<div class="ic"><div class="ic-l">SIÈGE / SEAT</div><div class="ic-v seat-v">'+pax.seat+'</div></div>'
    +'</div></div>'
    +'<div class="bp-foot">FIN EMBARQUEMENT 30 MIN AVANT LE DÉCOLLAGE / BOARDING CLOSES 30 MIN BEFORE DEPARTURE</div>'
    +'</div>'
    // STUB
    +'<div class="stub">'
    +'<div class="stub-bar"></div>'
    +'<div class="stub-body">'
    +'<div class="stub-logo"><span class="stub-logo-i">✈</span><span class="stub-logo-t">AirAykinz</span></div>'
    +'<div class="si"><div class="sl">PASSAGER</div><div class="sv" style="font-size:10px">'+pname+'</div></div>'
    +'<div class="si-row"><div class="si"><div class="sl">VOL</div><div class="sv">'+flight+'</div></div><div class="si"><div class="sl">DATE</div><div class="sv" style="font-size:9px">'+fd(fdate)+'</div></div></div>'
    +'<div class="si"><div class="sl">DE</div><div class="sv" style="font-size:9px">'+frc.toUpperCase()+' ('+fr+')</div></div>'
    +'<div class="si"><div class="sl">À</div><div class="sv" style="font-size:9px">'+frc.toUpperCase()+' ('+to+')</div></div>'
    +'<div class="si-row"><div class="si"><div class="sl">DÉPART</div><div class="sv">'+dep+'</div></div><div class="si"><div class="sl">ARRIVÉE</div><div class="sv">'+arr+'</div></div></div>'
    +'<div class="si-row"><div class="si"><div class="sl">PORTE</div><div class="sv" style="font-size:9px">'+gate+'</div></div><div class="si"><div class="sl">SIÈGE</div><div class="sv o">'+pax.seat+'</div></div></div>'
    +'<div class="si-row"><div class="si"><div class="sl">SEQ.</div><div class="sv">'+seq+'</div></div><div class="si"><div class="sl">CLASSE</div><div class="sv" style="font-size:9px">'+cabin+'</div></div></div>'
    +'</div>'
    +'<div class="stub-qr"><div id="'+qid+'"></div><div class="stub-hint">Scanner pour valider</div></div>'
    +'</div></div>'
    +'<div class="url-box"><code id="u-'+seq+'">'+url+'</code>'
    +'<button class="cp-btn" onclick="cp(\'u-'+seq+'\',this)">Copier</button></div>';

  new QRCode(document.getElementById(qid), {
    text: url, width:108, height:108,
    colorDark:'#1a2744', colorLight:'#ffffff',
    correctLevel: QRCode.CorrectLevel.M
  });
}

function cp(id, btn) {
  navigator.clipboard.writeText(document.getElementById(id).textContent).then(function(){
    btn.textContent = '✓'; setTimeout(function(){ btn.textContent = 'Copier'; }, 2000);
  });
}

// ── VALIDATOR ─────────────────────────────────────────
function runValidator() {
  var f = params.get('flight'), d = params.get('date'), tm = params.get('time'),
      fr = params.get('from'), to = params.get('to'),
      st = params.get('seat'), gt = params.get('gate'),
      px = params.get('passenger'), cb = params.get('cabin'), rf = params.get('ref'),
      fc = params.get('fromCity');

  function fd2(x) {
    if (!x) return '—';
    var a = x.split('-'), m = ['JAN','FÉV','MAR','AVR','MAI','JUN','JUL','AOU','SEP','OCT','NOV','DÉC'];
    return parseInt(a[2]) + ' ' + m[parseInt(a[1])-1] + ' ' + a[0];
  }

  function chk() {
    if (!f || !d) return {ok:false, r:'QR code invalide.'};
    var n = new Date(), a = d.split('-'), h = (tm||'0:0').split(':');
    var dep = new Date(+a[0], a[1]-1, +a[2], +h[0], +h[1]);
    if (n > new Date(+dep + 3600000)) return {ok:false, r:'Ce vol a déjà décollé. Billet expiré.'};
    if (n > new Date(+dep - 1800000)) return {ok:false, r:"Embarquement terminé (clôture 30 min avant départ)."};
    return {ok:true};
  }

  setTimeout(function() {
    var r = chk();
    var vc = document.getElementById('vc');
    var vi = document.getElementById('vi'), vt = document.getElementById('vt'), vs = document.getElementById('vs');
    var vb = document.getElementById('vb'), vn = document.getElementById('vn');
    var vscan = document.getElementById('vscan');

    vc.className = 'val-card ' + (r.ok ? 'v-ok' : 'v-err');
    vi.textContent = r.ok ? '✓' : '✗';
    vt.textContent = r.ok ? 'Billet valide' : 'Billet non valide';
    vs.textContent = r.ok ? 'Embarquement autorisé' : r.r;
    vn.textContent = r.ok
      ? 'Billet authentifié par AirAykinz. Présentez cette page à l\'agent d\'embarquement.'
      : 'Ce billet n\'est plus valide. Contactez le service client AirAykinz.';

    vb.innerHTML =
      '<div class="v-route"><div><div class="v-ap-l">Départ</div><div class="v-ap">'+(fr||'—')+'</div><div style="font-size:10px;color:#aaa">'+(fc||'')+'</div></div>'
      +'<div style="font-size:22px;color:#1a2744">✈</div>'
      +'<div style="text-align:right"><div class="v-ap-l">Arrivée</div><div class="v-ap">'+(to||'—')+'</div></div></div>'
      +'<div class="v-row"><span class="v-lbl">Passager</span><span class="v-val" style="font-size:13px">'+(px||'—')+'</span></div>'
      +'<div class="v-row"><span class="v-lbl">Vol</span><span class="v-val">'+(f||'—')+'</span></div>'
      +'<div class="v-row"><span class="v-lbl">Date</span><span class="v-val">'+fd2(d)+'</span></div>'
      +'<div class="v-row"><span class="v-lbl">Départ</span><span class="v-val big">'+(tm||'—')+'</span></div>'
      +'<div class="v-row"><span class="v-lbl">Porte</span><span class="v-val">'+(gt||'—')+'</span></div>'
      +'<div class="v-row"><span class="v-lbl">Siège</span><span class="v-val big">'+(st||'—')+'</span></div>'
      +'<div class="v-row"><span class="v-lbl">Classe</span><span class="v-val">'+(cb||'—')+'</span></div>'
      +(rf ? '<div class="v-row"><span class="v-lbl">Réf.</span><span class="v-val" style="font-family:monospace;letter-spacing:.08em">'+(rf)+'</span></div>' : '');

    vscan.style.display = 'block';
    var n = new Date();
    document.getElementById('vtime').textContent = n.toLocaleDateString('fr-FR',{day:'2-digit',month:'long',year:'numeric',hour:'2-digit',minute:'2-digit'});
  }, 900);
}
</script>
</body>
</html>
