<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-status-bar-style" content="default">
<meta name="apple-mobile-web-app-title" content="Spending">
<meta name="theme-color" content="#241C3C">
<link rel="apple-touch-icon" href="icon.png">
<link rel="manifest" href="manifest.json">
<title>Spending</title>
<script src="https://cdnjs.cloudflare.com/ajax/libs/pdf.js/3.11.174/pdf.min.js"></script>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600;700&family=Poppins:wght@400;500;600&display=swap" rel="stylesheet">
<style>
:root{
  --paper:#241C3C;        /* deep violet night */
  --paper-2:#332A52;      /* raised panel */
  --ink:#EDE7FA;          /* lavender white */
  --ink-soft:#A99BC9;     /* muted lavender */
  --rule:#453A6B;         /* violet rule */
  --green:#6FE3BE;        /* mint, under budget */
  --red:#FF6B8A;          /* rose, over budget */
  --ochre:#F5C26B;        /* amber, close to target */
  --blue:#8B6BF0;         /* violet, interactive */
  --shadow:0 4px 22px rgba(0,0,0,.28);
  color-scheme:dark;
  --radius:14px;
}
*{box-sizing:border-box}
body::before{content:"";position:fixed;inset:0;z-index:-1;pointer-events:none;
  background:radial-gradient(120% 65% at 50% -10%, #4B3A78 0%, #2E2450 38%, #241C3C 72%)}
body{margin:0;color:var(--ink);background:var(--paper);
  position:relative;min-height:100vh;
  font-family:"Poppins",-apple-system,BlinkMacSystemFont,sans-serif;
  font-feature-settings:"tnum" 1;line-height:1.55;-webkit-font-smoothing:antialiased}
.wrap{position:relative;z-index:1;max-width:840px;margin:0 auto;
  padding:calc(24px + env(safe-area-inset-top)) 16px calc(70px + env(safe-area-inset-bottom))}
header{padding-bottom:4px;margin-bottom:20px}
h1{text-shadow:0 2px 18px rgba(139,107,240,.35);font-family:"Playfair Display",Georgia,serif;font-size:clamp(27px,5.4vw,38px);
  font-weight:700;letter-spacing:-.01em;margin:0;color:var(--ink)}
.sub{color:var(--ink-soft);font-size:14px;margin:0}
h2{font-size:11px;font-weight:600;letter-spacing:.09em;text-transform:uppercase;
  color:var(--ink-soft);margin:26px 0 12px;padding-bottom:0;border-bottom:0;
  display:flex;justify-content:space-between;align-items:center;gap:10px}
textarea{width:100%;min-height:96px;font:inherit;font-size:16px;padding:13px;
  -webkit-appearance:none;appearance:none;-webkit-text-fill-color:var(--ink);
  caret-color:var(--blue);opacity:1;
  border:1px solid var(--rule);border-radius:var(--radius);background:rgba(255,255,255,.06);
  color:var(--ink);resize:vertical;box-shadow:var(--shadow)}
input[type=text],input[type=number]{font:inherit;font-size:16px;padding:8px 11px;
  -webkit-appearance:none;appearance:none;-webkit-text-fill-color:var(--ink);
  caret-color:var(--blue);opacity:1;border:1px solid var(--rule);
  border-radius:9px;background:rgba(255,255,255,.06);color:var(--ink)}
input[type=number]{width:96px;text-align:right}
textarea:focus,input:focus,select:focus{outline:2px solid var(--blue);outline-offset:1px}
.btnrow{display:flex;gap:9px;flex-wrap:wrap;margin-top:11px;align-items:center}
button{font:inherit;font-size:14px;font-weight:500;padding:10px 20px;border:1px solid var(--rule);
  border-radius:999px;background:rgba(255,255,255,.05);color:var(--ink);cursor:pointer;
  transition:background .13s,color .13s}
button.primary{background:var(--blue);color:#fff;border-color:var(--blue);font-weight:600;
  box-shadow:0 4px 16px rgba(139,107,240,.4)}
button:hover{background:var(--blue);color:#fff;border-color:var(--blue)}
button.ghost{color:var(--ink-soft);font-size:13px;padding:8px 15px}
button.link{border:0;background:none;color:var(--blue);font-size:12.5px;padding:3px 5px;
  font-weight:600;border-radius:7px}
button.link:hover{background:rgba(139,107,240,.18);color:var(--ink)}
button.x{border:0;background:none;color:var(--ink-soft);font-size:18px;line-height:1;
  padding:2px 8px;border-radius:7px}
button.x:hover{background:rgba(255,107,138,.18);color:var(--red)}
button.arm{border-color:var(--red);color:var(--red);background:rgba(255,107,138,.16);font-weight:600}
button.arm:hover{background:var(--red);color:#241C3C}
button.small{font-size:12.5px;padding:7px 14px}
select{font:inherit;font-size:13px;padding:7px 10px;border:1px solid var(--rule);
  border-radius:9px;background:#372E58;color:var(--ink)}
#month{font-size:14px;font-weight:600;border-color:var(--blue);color:var(--ink);padding:9px 12px}
.notice{margin:14px 0 0;padding:13px 15px;background:rgba(255,255,255,.07);border:1px solid var(--rule);
  border-left:4px solid var(--ochre);border-radius:var(--radius);font-size:13.5px;
  display:flex;align-items:center;gap:10px;flex-wrap:wrap;box-shadow:var(--shadow)}
.notice .msg{flex:1;min-width:180px}
.notice.bad{border-left-color:var(--red)}
.notice.good{border-left-color:var(--green)}
.monthbar{display:flex;align-items:center;gap:12px;margin:22px 0 0;padding:12px 15px;
  background:rgba(255,255,255,.07);border:1px solid var(--rule);border-radius:var(--radius);
  box-shadow:var(--shadow)}
.monthbar-label{font-size:10.5px;font-weight:600;letter-spacing:.09em;text-transform:uppercase;
  color:var(--ink-soft)}
.monthbar select{flex:0 1 auto}
.monthbar .link{margin-left:auto}
.summary{background:rgba(255,255,255,.07);border:1px solid var(--rule);border-radius:var(--radius);
  border-left:5px solid var(--blue);padding:17px 19px;margin:16px 0;box-shadow:var(--shadow)}
.big{font-family:"Playfair Display",Georgia,serif;font-size:clamp(18px,3.2vw,24px);
  font-weight:700;margin:0 0 5px;letter-spacing:-.01em;line-height:1.3}
.small{font-size:13px;color:var(--ink-soft);margin:0}
.over{color:var(--red)} .under{color:var(--green)}
#bars,#needsort,#compare,#settings,#backupbox{background:rgba(255,255,255,.055);border:1px solid var(--rule);
  border-radius:var(--radius);padding:6px 17px;box-shadow:var(--shadow)}
#settings.hidden,#needsort.hidden,#compare.hidden{display:none}
#backupbox{padding:15px 17px}
.bar{display:flex;align-items:center;gap:12px;padding:11px 0;border-bottom:1px solid var(--rule)}
.bar:last-of-type{border-bottom:0}
.bar-name{width:120px;flex-shrink:0;font-size:13.5px;font-weight:500}
.bar-track{flex:1;height:20px;position:relative;min-width:44px;display:flex;
  background:rgba(255,255,255,.09);border-radius:999px;overflow:hidden}
.seg{height:100%}
.seg.spent{background:var(--green)}
.seg.spent.warn{background:var(--ochre)}
.seg.spent.bust{background:var(--red)}
.seg.left{background:rgba(111,227,190,.26)}
.seg.left.warn{background:rgba(245,194,107,.26)}
.seg.overflow{background:var(--red);
  background-image:repeating-linear-gradient(45deg,rgba(36,28,60,.38) 0 3px,transparent 3px 6px)}
.seg.none{background:rgba(169,155,201,.5)}
.bar-target{position:absolute;top:-3px;bottom:-3px;width:2px;background:var(--ink);opacity:.85;z-index:2}
.bar-num{width:132px;flex-shrink:0;text-align:right;font-size:13px;white-space:nowrap;line-height:1.3}
.bar-num b{font-size:14.5px;display:block;font-weight:600}
.bar-num span{color:var(--ink-soft);font-size:11.5px}
.bar-num span.left{color:var(--green);font-weight:600}
.bar-num span.over{color:var(--red);font-weight:600}
.legend{display:flex;flex-wrap:wrap;gap:15px;font-size:11.5px;color:var(--ink-soft);
  margin:0;padding:11px 0 13px;border-top:1px solid var(--rule)}
.legend i{display:inline-block;width:15px;height:10px;margin-right:5px;vertical-align:middle;
  border-radius:3px;font-style:normal}
.setrow{display:flex;align-items:center;gap:10px;padding:9px 0;border-bottom:1px solid var(--rule)}
.setrow label{flex:1;font-size:13.5px;font-weight:500}
.setrow .note{font-size:11.5px;color:var(--ink-soft);font-weight:400}
.toggle input{width:19px;height:19px;accent-color:var(--blue);cursor:pointer;margin:0 6px 0 0}
.addrow{display:flex;gap:8px;margin:13px 0}.addrow input{flex:1}
.alloc{background:rgba(0,0,0,.22);border:1px solid var(--rule);border-radius:10px;
  padding:13px 15px;margin-bottom:15px;font-size:13.5px}
table{width:100%;border-collapse:collapse;font-size:13px}
th,td{padding:9px 5px;border-bottom:1px solid var(--rule);text-align:left;vertical-align:middle}
tbody tr:last-child td{border-bottom:0}
thead th{font-size:10.5px;color:var(--ink-soft);letter-spacing:.07em;text-transform:uppercase;
  font-weight:600}
td.amt,th.amt{text-align:right;white-space:nowrap}
td.amt{font-weight:500}
td.merch{font-size:12.5px;color:var(--ink-soft);max-width:170px;overflow:hidden;
  text-overflow:ellipsis;white-space:nowrap}
td.day{font-size:11.5px;color:var(--ink-soft);white-space:nowrap;width:52px}
tbody tr.tot td{border-top:1.5px solid var(--blue);font-weight:600}
select.cat{font-size:12.5px;padding:4px 7px;max-width:126px}
select.guessed{border-color:var(--ochre);border-width:1.5px}
input.amtin{width:84px;text-align:right;font-size:16px;padding:5px 6px;
  -webkit-text-fill-color:var(--ink);caret-color:var(--blue);
  border:1px solid transparent;border-radius:8px;background:transparent;color:var(--ink);
  font-weight:500;font-family:inherit}
input.amtin:hover{border-color:var(--rule);background:rgba(255,255,255,.07)}
input.amtin:focus{border-color:var(--blue);background:rgba(255,255,255,.1);outline:none}
input.amtin::-webkit-outer-spin-button,input.amtin::-webkit-inner-spin-button{
  -webkit-appearance:none;margin:0}
input.amtin{-moz-appearance:textfield}
td.kill{width:32px;padding-right:0}
.scroll{overflow-x:auto;-webkit-overflow-scrolling:touch}
.scroll table{min-width:100%}
.delta{font-size:11px;margin-left:5px}
.hint{font-size:12px;color:var(--ink-soft);margin:9px 0 0;line-height:1.5}
.empty{color:var(--ink-soft);font-size:14px;padding:22px 0;text-align:center}
.build{margin-top:34px;padding-top:14px;border-top:1px solid var(--rule);
  font-size:11px;color:var(--ink-soft);display:flex;justify-content:space-between;gap:10px}
.hidden{display:none}
@media(max-width:520px){
  #bars,#needsort,#compare,#settings{padding:4px 13px}
  .bar-name{width:80px;font-size:12.5px}.bar-num{width:92px;font-size:12px}
  input[type=number]{width:84px}
  input.amtin{width:76px}
  select.cat{max-width:104px}
}
</style>
</head>
<body>
<div class="wrap">

<header>
  <h1>Budget Tracker</h1>
</header>

<h2>Add a statement</h2>
<textarea id="input" placeholder="Paste transactions, or type your own. Cents are optional:
Jollibee 17
Chatime, 9.56
Groceries - $84"></textarea>
<div class="btnrow">
  <button class="primary" id="add">Sort these</button>
  <button class="ghost" id="pick">Upload PDF or CSV</button>
</div>
<input type="file" id="file" accept=".pdf,.csv,.txt,application/pdf,text/csv,text/plain" class="hidden">
<p class="hint">RBC app: More, then Statements, then Save to Files. Upload the PDF here. The month is read from the statement.</p>

<div id="notice" class="notice hidden"></div>

<div class="monthbar">
  <span class="monthbar-label">Showing</span>
  <select id="month" aria-label="Which month"></select>
  <button class="link" id="delMonth">Delete this month</button>
</div>

<div class="summary">
  <p class="big" id="headline">Nothing loaded yet.</p>
  <p class="small" id="subline">Upload a statement to see the breakdown.</p>
</div>

<h2>By category</h2>
<div id="bars"><p class="empty">No transactions yet.</p></div>

<h2 id="sortHead" class="hidden"><span>Needs sorting</span></h2>
<div id="needsort" class="hidden"></div>

<h2 id="cmpHead" class="hidden"><span>Month by month</span></h2>
<div id="compare" class="scroll hidden"></div>

<h2><span>Targets</span><button class="link" id="toggleSet">Edit</button></h2>
<div id="settings" class="hidden">
  <div class="setrow">
    <label>Monthly target <span class="note">everything, including rent</span></label>
    <input type="number" id="monthly" min="0" step="10">
  </div>
  <div class="setrow">
    <label>Fixed costs <span class="note">rent and transit, not on the card</span></label>
    <input type="number" id="fixed" min="0" step="10">
  </div>
  <div class="setrow">
    <label>Show cents <span class="note">off rounds everything to the dollar</span></label>
    <span class="toggle"><input type="checkbox" id="cents"></span>
  </div>
  <div id="catrows"></div>
  <div class="addrow">
    <input type="text" id="newcat" placeholder="New category name" maxlength="22">
    <button id="addcat">Add</button>
  </div>
  <div class="alloc" id="alloc"></div>
</div>
<div id="setsummary" class="hint" style="margin-top:0"></div>

<h2><span>Transactions</span></h2>
<p class="hint" style="margin-bottom:8px">Amber outline means it guessed. Change one and it remembers that merchant.</p>
<div id="txlist"><p class="empty">No transactions yet.</p></div>

<h2><span>Your data</span></h2>
<div class="btnrow" style="margin-top:0">
  <button class="ghost" id="backup">Back up to a file</button>
  <button class="ghost" id="restore">Restore from a file</button>
</div>
<input type="file" id="bfile" accept=".json,application/json" class="hidden">
<p class="hint">Everything lives on this phone only. Back up before you delete the home screen icon,
clear Safari data, or switch devices, because iOS removes stored data along with the app.</p>

<h2><span>Backup</span></h2>
<div id="backupbox">
  <div class="btnrow" style="margin-top:0">
    <button class="ghost" id="backup">Download backup</button>
    <button class="ghost" id="copybk">Copy to clipboard</button>
    <button class="ghost" id="restore">Restore from file</button>
  </div>
  <input type="file" id="bkfile" accept=".json,application/json" class="hidden">
  <p class="hint">Your data lives only on this device. Back it up before you delete the home screen
  icon, clear Safari data, or switch phones. If Download does nothing, use Copy and paste it
  somewhere safe like a note or an email to yourself.</p>
  <textarea id="bktext" class="hidden" readonly style="min-height:70px;font-size:11px"></textarea>
</div>

<div class="build">
  <span>Build 16 &middot; backup and restore</span>
  <span id="stat"></span>
</div>

</div>
<script>
const DEFAULT_TARGETS = {'Groceries':250,'Eating out':150,'Coffee & tea':0,'Delivery':0,
  'Shopping':100,'Entertainment':50,'Personal care':50,'Subscriptions':17,
  'Transport':0,'Travel':0,'Other':0};
const SEED = [
  [/CHATIME|HANLIN TEA|CHAYAN|MACU TEA|PARAGON TEA|STARBUCKS|BREWED COFFEE|NOIR FLY AWAY|MENTORA/i,'Coffee & tea'],
  [/DOORDASH|SKIPTHE|UBER ?EATS|UBER HOLDINGS|INSTACART/i,'Delivery'],
  [/SAFEWAY|T&T SUPERMARKET|D'ITALIA|FOUR RIVERS|SUPERSTORE|NO FRILLS|COSTCO|WHOLE FOODS|IGA|SAVE.?ON/i,'Groceries'],
  [/JOLLIBEE|JAPADOG|MCDONALD|KFC|FIVE GUYS|SUSHIYAMA|UNCLE FATIH|HOT POT|LUCKY SUSHI|FREEHOUSE|ZAPOTECA|MOMO FACTORY|CACTUS CLUB|A LA MODE|GREEN LEAF|JUICY JOES|HANDI GRILL|FALAFEL|FUEGO|LOCAL KITSILANO|RAIN OR SHINE|OSAKA|ITALIAN DELI|JUST ANOTHER|SWITCH|DANK MART|7 ELEVEN|PIZZA|SUSHI|RESTAURANT|CAFE|TST-|SQ \*/i,'Eating out'],
  [/YESASIA|ALIEXPRESS|ETSY|SHEIN/i,'Shopping'],
  [/SEPHORA|MICHAELS|OPUS ART|LEWKIN|TEMU|SPCA THRIFT|OAK FORT|SIMONS|LA VIE EN ROSE|INDIGO|DOLLARAMA|DOLLAR TREE|ZARA|AMAZON|WINNERS|UNIQLO/i,'Shopping'],
  [/CINEPLEX|FAMOUS PLAYER|APPROACH CLIMBING|PROGRESSION BOULDER|CAFE AU CLAY|BC LIQUOR|BREWING/i,'Entertainment'],
  [/SHOPPERS DRUG|BEAUTY SALON|PHARMASAVE|LONDON DRUGS|REXALL/i,'Personal care'],
  [/BELL MEDIA|NETFLIX|SPOTIFY|CRAVE|DISNEY|APPLE ?SERVICES|APPLE\.COM|ITUNES|GOOGLE ?\*/i,'Subscriptions'],
  [/BC TRANSIT|TRANSLINK|COMPASS|PETRO.?CANADA|CHEVRON|CHV\d|ESSO|SHELL|CANADIAN TIRE|TAXI|LYFT|EVO CAR|MODO/i,'Transport'],
  [/EXPEDIA|BCF ?-|BC FERR|SUPER 8|MOTEL|HOTEL|AIR ?CANADA|WESTJET|FLAIR/i,'Travel']
];
const MN = ['Jan','Feb','Mar','Apr','May','Jun','Jul','Aug','Sep','Oct','Nov','Dec'];
const MI = {JAN:0,FEB:1,MAR:2,APR:3,MAY:4,JUN:5,JUL:6,AUG:7,SEP:8,OCT:9,NOV:10,DEC:11};
const TXN = /^([A-Z]{3})\s+(\d{1,2})\s+[A-Z]{3}\s+\d{1,2}\s+(.+?)\s+(-?\$[\d,]+\.\d{2})/;
const SKIP = /PAYMENT|MERCI|THANK YOU|BALANCE|Minimum payment|Credit limit|Available credit|Total Account|Interest Rate/i;
// description, a separator, then the amount at the end. Cents optional.
// A store number like "SAFEWAY #4901" cannot match, because # is not a separator.
const TYPED = /^(.+?)[\s,\-\|\t]+\$?(\d[\d,]*(?:\.\d{1,2})?)\s*$/;
// ---- PayPal activity statements ----
// Only the Transaction History rows count. Summary tables have no date prefix, and the
// funding deposits are positive, so requiring a date and a negative gross skips both.
const PP   = /^(\d{2})\/(\d{2})\/(\d{4})\s+(.*?)-([\d,]+\.\d{2})\s+[\d,.]+\s+-[\d,]+\.\d{2}\s*$/;
const PDATE= /^\d{2}\/\d{2}\/\d{4}/;
const PJUNK= /^(Transaction History|Date Description|Merchant Account|Page \d|ID:|To report|To cancel|Activity |Balance |Description|Total|Payments |Deposits |Withdrawals|Fees|Beginning|Ending|CAD|USD)/i;
const PPRE = /^(PreApproved Payment Bill User Payment|PreApproved Payment Bill User|Express Checkout Payment|Payment Bill User Payment|Bank Deposit to PP Account|General Credit Card Deposit|General Card Deposit|Transfer Deposit|Mobile Payment|Web Accept Payment|Subscription Payment|Recurring Payment|Donation Payment|Payment)\s*/i;

function parsePayPal(lines){
  const out = [];
  lines.forEach((l, i) => {
    const m = PP.exec(l.trim());
    if (!m) return;
    const amt = parseFloat(m[5].replace(/,/g,''));
    if (!(amt > 0)) return;

    // the merchant sits on a line just above the date row, sometimes sharing it
    // with the boilerplate description
    let name = '';
    for (let j = i-1; j >= Math.max(0, i-3); j--){
      let c = (lines[j]||'').trim();
      if (!c || PDATE.test(c) || PJUNK.test(c) || c.includes('@')) continue;
      c = c.replace(PPRE,'').trim();
      if (c){ name = c; break; }
    }
    if (!name){                                  // fall back to the email domain below it
      for (let j = i+1; j < Math.min(lines.length, i+4); j++){
        const e = /@([\w-]+)\./.exec(lines[j]||'');
        if (e){ name = e[1].toUpperCase(); break; }
      }
    }
    if (!name) name = m[4].replace(PPRE,'').trim() || 'PayPal payment';

    const d = +m[1], mo = +m[2] - 1, y = +m[3];
    const g = guess(name);
    out.push({id:uid(), desc:name, amt, cat:g.cat, sure:g.sure,
              period: y + '-' + mo, day: String(d).padStart(2,'0') + ' ' + MN[mo].toUpperCase()});
  });
  return out;
}

const NOTATX = /STATEMENT FROM|ACCOUNT BALANCE|POINTS|Customer Service|Telephone Banking|Collect Outside|Rewards Website|Credit limit|Available credit|Annual interest|Payment due|Cash advances|Purchases &|Payments &|TRANSACTION POSTING|ACTIVITY DESCRIPTION|Royal Bank|P\.O\. BOX|PAYMENT CENTRE/i;
const STMT = /STATEMENT FROM\s+[A-Z]{3}\s+\d{1,2}\s+TO\s+([A-Z]{3})\s+\d{1,2},?\s+(\d{4})/i;

let tx = [], learned = {}, targets = {...DEFAULT_TARGETS}, fixed = 1097, monthly = 1714,
    view = 'ALL', cents = false;

const money = n => (n<0?'-':'') + '$' + Math.abs(n).toLocaleString('en-CA',
  cents ? {minimumFractionDigits:2, maximumFractionDigits:2}
        : {minimumFractionDigits:0, maximumFractionDigits:0});

const $ = id => document.getElementById(id);
const NOISE = /^(SQ|TST|DD|SP|POS|PURCHASE|WWW|PAYPAL|AMZN|MKTP)$/;
const PLACE = /^(VANCOUVER|RICHMOND|BURNABY|SURREY|VICTORIA|COQUITLAM|KELOWNA|TORONTO|CALGARY|EDMONTON|MONTREAL|OTTAWA|KITSILANO|ROBSON|WEST|EAST|NORTH|SOUTH|DOWNTOWN|BC|AB|ON|QC|MB|SK|NS|NB|NL|PE|YT|NT|NU|CA|USA|DE|COM|LTD|INC|STORE|CANADA)$/;
function key(s){
  const w = s.toUpperCase()
    .replace(/[^A-Z ]+/g,' ')          // drop digits, punctuation, store numbers
    .split(/\s+/)
    .filter(x => x.length > 1 && !NOISE.test(x));
  while (w.length > 1 && PLACE.test(w[w.length-1])) w.pop();   // trim trailing city/province
  return w.slice(0,2).join(' ') || s.toUpperCase().slice(0,18);
}
const cats = () => Object.keys(targets);
let seq = 0;
const uid = () => 't' + Date.now().toString(36) + (seq++).toString(36);
const clean = d => d.replace(/\d{6,}/g,'').replace(/["',]+/g,' ').replace(/\s+/g,' ').trim();
const label = p => { const [y,m] = p.split('-'); return MN[+m] + ' ' + y; };
const periods = () => [...new Set(tx.map(t=>t.period))].sort();
const thisPeriod = () => { const d=new Date(); return d.getFullYear()+'-'+d.getMonth(); };

function guess(desc){
  const k = key(desc);
  if (learned[k] && targets[learned[k]] !== undefined) return {cat:learned[k], sure:true};
  for (const [re,cat] of SEED) if (re.test(desc) && targets[cat] !== undefined) return {cat, sure:false};
  return {cat:'Other', sure:false};
}

function parse(text){
  const out = [];
  const lines0 = text.split('\n');

  // Work out what kind of document this is BEFORE parsing anything.
  // Statements are full of phone numbers, years and reference numbers that look
  // like amounts to the loose typed-line parser, so the two must never both run.
  if (/PayPal/i.test(text) && /Transaction History/i.test(text)){
    const pp = parsePayPal(lines0);
    if (pp.length) return pp;
  }
  const isStatement = /STATEMENT FROM/i.test(text) ||
                      lines0.filter(l => TXN.test(l.trim())).length >= 3;

  const sm = STMT.exec(text);
  const endM = sm ? MI[sm[1].toUpperCase()] : null;
  const endY = sm ? +sm[2] : null;
  const fb = view !== 'ALL' ? view : thisPeriod();

  text.split('\n').forEach(line => {
    line = line.trim(); if (!line) return;
    const m = TXN.exec(line);
    if (m){
      const amt = parseFloat(m[4].replace(/[$,]/g,''));
      const desc = clean(m[3]);
      if (!(amt > 0) || desc.length < 3 || SKIP.test(desc)) return;
      const mo = MI[m[1].toUpperCase()];
      let period = fb, day = m[1] + ' ' + m[2];
      if (endM !== null && mo !== undefined){
        // a statement can straddle a year end
        let y = endY; if (mo === 11 && endM === 0) y = endY - 1;
        period = y + '-' + mo;
      }
      const g = guess(desc);
      out.push({id:uid(), desc, amt, cat:g.cat, sure:g.sure, period, day});
      return;
    }
    if (isStatement) return;   // statement mode: nothing but dated rows

    // typed or CSV line: the amount is the last thing on the line.
    // "Jollibee 17", "Jollibee, 17.05", "Jollibee - $17" all work.
    const p = TYPED.exec(line.replace(/\d{4}-\d{2}-\d{2}|\d{1,2}\/\d{1,2}\/\d{2,4}/g,'').trim());
    if (!p) return;
    const amt = parseFloat(p[2].replace(/,/g,''));
    if (!(amt > 0)) return;
    // a bare 4-digit whole number after a phone number or on a boilerplate line is
    // almost never an amount
    if (!/\./.test(p[2]) && (/\(\d{3}\)|\d{3}-\d{4}|1-8\d\d/.test(line) || amt > 9999)) return;
    const desc = clean(p[1]);
    if (desc.length < 3 || SKIP.test(desc) || NOTATX.test(desc)) return;
    const g = guess(desc);
    out.push({id:uid(), desc, amt, cat:g.cat, sure:g.sure, period:fb, day:''});
  });
  return out;
}

function save(){
  try { localStorage.setItem('tracker', JSON.stringify({tx,learned,targets,fixed,monthly})); } catch(e){}
}
function load(){
  try {
    const raw = localStorage.getItem('tracker');
    if (raw){
      const d = JSON.parse(raw);
      tx = (d.tx||[]).map(t => ({...t, id: t.id || uid(), period: t.period || thisPeriod(), day: t.day || ''}));
      learned = d.learned||{};
      if (d.targets && Object.keys(d.targets).length) targets = d.targets;
      if (typeof d.fixed === 'number') fixed = d.fixed;
      if (typeof d.monthly === 'number') monthly = d.monthly;
      cents = !!d.cents;
    }
  } catch(e){}
  if (targets['Other'] === undefined) targets['Other'] = 0;
  const p = periods(); view = p.length ? p[p.length-1] : 'ALL';
  renderSettings(); render();
}

let armTimer = null, armed = null;
function arm(btn, key, label, action){
  if (armed === key){
    clearTimeout(armTimer); armed = null;
    btn.classList.remove('arm'); btn.textContent = btn.dataset.idle;
    action(); return;
  }
  if (armed) disarm();
  armed = key; btn.dataset.idle = btn.dataset.idle || btn.textContent;
  btn.textContent = label; btn.classList.add('arm');
  armTimer = setTimeout(() => disarm(btn), 5000);
}
function disarm(btn){
  clearTimeout(armTimer); armed = null;
  document.querySelectorAll('button.arm').forEach(b => {
    b.classList.remove('arm'); if (b.dataset.idle) b.textContent = b.dataset.idle;
  });
}
function say(msg, tone, actions){
  const n = $('notice');
  n.className = 'notice' + (tone ? ' ' + tone : '');
  n.innerHTML = '<span class="msg">' + msg + '</span>' +
    (actions||[]).map((a,i)=>`<button class="small" data-act="${i}">${a.label}</button>`).join('');
  (actions||[]).forEach((a,i) =>
    n.querySelector(`[data-act="${i}"]`).addEventListener('click', () => { hide(); a.run(); }));
  if (!actions) setTimeout(() => { if (n.textContent.includes(msg.replace(/<[^>]*>/g,''))) hide(); }, 6000);
}
function hide(){ $('notice').className = 'notice hidden'; $('notice').innerHTML = ''; }

function stamp(){
  const p = periods();
  $('stat').textContent = tx.length
    ? tx.length + ' transactions across ' + p.length + ' month' + (p.length===1?'':'s')
    : 'no data yet';
}

function renderMonths(){
  const p = periods();
  $('month').innerHTML = (p.length > 1 ? ['<option value="ALL">All months</option>'] : [])
    .concat(p.slice().reverse().map(x =>
      `<option value="${x}"${x===view?' selected':''}>${label(x)}</option>`)).join('')
    || '<option value="ALL">No data</option>';
  $('delMonth').classList.toggle('hidden', view === 'ALL' || !p.length);
  stamp();
}

function renderSettings(){
  $('monthly').value = monthly; $('fixed').value = fixed; $('cents').checked = cents;
  $('catrows').innerHTML = cats().map(c => `
    <div class="setrow"><label>${c}</label>
      <input type="number" min="0" step="5" value="${targets[c]}" data-cat="${c}">
      ${c==='Other'?'<span style="width:31px"></span>':`<button class="x" data-del="${c}">&times;</button>`}
    </div>`).join('');
  $('catrows').querySelectorAll('input').forEach(i => i.addEventListener('input', e => {
    targets[e.target.dataset.cat] = Math.max(0, +e.target.value || 0); save(); render(); updateAlloc();
  }));
  $('catrows').querySelectorAll('[data-del]').forEach(b => b.addEventListener('click', e => {
    const c = e.target.dataset.del, n = tx.filter(t=>t.cat===c).length;
    arm(e.target, 'delcat:'+c, '\u2713', () => {
      tx.forEach(t => { if (t.cat===c){ t.cat='Other'; t.sure=false; } });
      Object.keys(learned).forEach(k => { if (learned[k]===c) delete learned[k]; });
      delete targets[c]; save(); renderSettings(); render();
      say(n ? `Removed ${c}. Its ${n} transactions moved to Other.` : `Removed ${c}.`, 'good');
    });
  }));
  updateAlloc();
}

function updateAlloc(){
  const sum = cats().reduce((s,c)=>s+targets[c],0), allocated = sum + fixed, left = monthly - allocated;
  $('alloc').innerHTML = left === 0
    ? `<b>${money(allocated)}</b> allocated. Matches your monthly target exactly.`
    : left > 0
      ? `<b>${money(allocated)}</b> allocated of ${money(monthly)}. <span class="under">${money(left)} unassigned.</span>`
      : `<b>${money(allocated)}</b> allocated of ${money(monthly)}. <span class="over">${money(-left)} over your own target.</span>`;
  $('setsummary').textContent =
    `Monthly target ${money(monthly)}, of which ${money(fixed)} is rent and transit, leaving ${money(monthly-fixed)} for the card.`;
}

function totalsFor(period){
  const t = {}; cats().forEach(c => t[c] = 0);
  tx.forEach(x => {
    if (period !== 'ALL' && x.period !== period) return;
    if (t[x.cat] === undefined) x.cat = 'Other';
    t[x.cat] += x.amt;
  });
  return t;
}

function renderNeedSort(){
  // group everything sitting in Other by merchant, so one choice fixes all of them
  const g = {};
  tx.forEach(t => {
    if (t.cat !== 'Other') return;
    const k = key(t.desc);
    (g[k] = g[k] || {k, name:t.desc, n:0, amt:0}).n++;
    g[k].amt += t.amt;
  });
  const rows = Object.values(g).sort((a,b)=>b.amt-a.amt);
  const show = rows.length > 0;
  $('sortHead').classList.toggle('hidden', !show);
  $('needsort').classList.toggle('hidden', !show);
  if (!show) return;

  const opts = cats().map(c=>`<option${c==='Other'?' selected':''}>${c}</option>`).join('');
  $('needsort').innerHTML =
    `<p class="hint" style="margin:0 0 8px">${rows.length} merchant${rows.length===1?'':'s'} landed in Other. ` +
    `Set each one once and it applies to every transaction from that merchant, in every month.</p>` +
    '<table><tbody>' + rows.map(r => `<tr>
      <td class="merch" title="${r.name.replace(/"/g,'')}">${r.name}</td>
      <td style="width:44px;font-size:11.5px;color:var(--ink-soft)">${r.n>1?r.n+'\u00d7':''}</td>
      <td class="amt" style="width:66px">${money(r.amt)}</td>
      <td style="width:140px"><select class="cat guessed" data-k="${r.k.replace(/"/g,'')}">${opts}</select></td>
    </tr>`).join('') + '</tbody></table>';

  $('needsort').querySelectorAll('select').forEach(s => s.addEventListener('change', e => {
    const k = e.target.dataset.k, c = e.target.value;
    if (c === 'Other') return;
    learned[k] = c;
    tx.forEach(t => { if (key(t.desc) === k){ t.cat = c; t.sure = true; } });
    save(); render();
  }));
}

function renderCompare(){
  const p = periods();
  const show = p.length >= 2;
  $('cmpHead').classList.toggle('hidden', !show);
  $('compare').classList.toggle('hidden', !show);
  if (!show) return;

  const per = {}; p.forEach(x => per[x] = totalsFor(x));
  const list = cats().filter(c => p.some(x => per[x][c] > 0));
  const head = '<tr><th>Category</th>' + p.map(x=>`<th class="amt">${label(x)}</th>`).join('') +
               '<th class="amt">Avg</th></tr>';
  const rows = list.map(c => {
    const vals = p.map(x => per[x][c]);
    const avg = vals.reduce((a,b)=>a+b,0)/vals.length;
    return '<tr><td>' + c + '</td>' + vals.map((v,i) => {
      let d = '';
      if (i === vals.length-1 && vals.length > 1){
        const prev = vals[i-1], ch = v - prev;
        if (Math.abs(ch) >= 5) d = `<span class="delta ${ch>0?'over':'under'}">${ch>0?'\u25B2':'\u25BC'}${money(Math.abs(ch))}</span>`;
      }
      return `<td class="amt">${money(v)}${d}</td>`;
    }).join('') + `<td class="amt">${money(avg)}</td></tr>`;
  }).join('');
  const tot = p.map(x => Object.values(per[x]).reduce((a,b)=>a+b,0));
  const totRow = '<tr class="tot"><td>Card total</td>' +
    tot.map(v=>`<td class="amt">${money(v)}</td>`).join('') +
    `<td class="amt">${money(tot.reduce((a,b)=>a+b,0)/tot.length)}</td></tr>`;
  $('compare').innerHTML = `<table><thead>${head}</thead><tbody>${rows}${totRow}</tbody></table>
    <p class="hint">Arrows compare the newest month with the one before it.</p>`;
}

function render(){
  armed = null;
  renderMonths();
  const list = cats(), totals = totalsFor(view);
  const inView = tx.filter(t => view === 'ALL' || t.period === view);
  const nMonths = view === 'ALL' ? Math.max(1, periods().length) : 1;
  const cardTotal = inView.reduce((s,t)=>s+t.amt,0);
  const cardTarget = monthly - fixed;

  if (!tx.length){
    $('headline').textContent = 'Nothing loaded yet.';
    $('subline').textContent = 'Upload a statement to see the breakdown.';
  } else if (view === 'ALL'){
    const avg = cardTotal/nMonths + fixed, diff = avg - monthly;
    $('headline').innerHTML = money(avg) + ' a month on average, <span class="'+(diff>0?'over':'under')+'">' +
      money(Math.abs(diff)) + (diff>0?' over':' under') + '</span> your ' + money(monthly) + ' target.';
    $('subline').textContent = nMonths + ' months, ' + money(cardTotal) + ' on the card in total.';
  } else {
    const all = cardTotal + fixed, diff = all - monthly;
    $('headline').innerHTML = money(all) + ' in ' + label(view) + ', <span class="'+(diff>0?'over':'under')+'">' +
      money(Math.abs(diff)) + (diff>0?' over':' under') + '</span> your ' + money(monthly) + ' target.';
    $('subline').textContent = money(cardTotal) + ' on the card plus ' + money(fixed) +
      ' fixed. Card target is ' + money(cardTarget) + '.';
  }

  const scale = view === 'ALL' ? nMonths : 1;
  const shown = list.filter(c => totals[c] > 0 || targets[c] > 0);
  // categories with no target share one scale; each targeted bar is scaled to its own
  // target so the marker always sits at 75% and overspend is visible past it
  const freeMax = Math.max(50, ...shown.filter(c => !targets[c]).map(c => (totals[c]||0)/scale));

  $('bars').innerHTML = shown.length ? shown.map(c => {
    const v = (totals[c]||0)/scale, t = targets[c];

    if (!t){        // no target set: one neutral bar, scaled against the other untargeted ones
      const w = freeMax > 0 ? Math.min(100, v/freeMax*100) : 0;
      return `<div class="bar"><span class="bar-name">${c}</span>
        <span class="bar-track"><span class="seg none" style="width:${w.toFixed(1)}%"></span></span>
        <span class="bar-num"><b>${money(v)}</b><span>no target</span></span></div>`;
    }

    // the track spans whichever is bigger, the target or what you spent
    const barMax = Math.max(t, v);
    const ratio  = v / t;
    const tone   = ratio > 1 ? 'bust' : ratio >= 0.85 ? 'warn' : '';
    let segs, tail;

    if (v <= t){                                   // spent, then what is left
      segs = `<span class="seg spent ${tone}" style="width:${(v/barMax*100).toFixed(1)}%"></span>` +
             `<span class="seg left ${tone}" style="width:${((t-v)/barMax*100).toFixed(1)}%"></span>`;
      tail = `<span class="left">${money(t-v)} left</span>`;
    } else {                                       // up to target, then the overspend, hatched
      segs = `<span class="seg spent bust" style="width:${(t/barMax*100).toFixed(1)}%"></span>` +
             `<span class="seg overflow" style="width:${((v-t)/barMax*100).toFixed(1)}%"></span>`;
      tail = `<span class="over">${money(v-t)} over</span>`;
    }

    return `<div class="bar"><span class="bar-name">${c}</span>
      <span class="bar-track">${segs}
        <span class="bar-target" style="left:${(t/barMax*100).toFixed(1)}%"></span></span>
      <span class="bar-num"><b>${money(v)}</b>${tail}</span></div>`;
  }).join('') +
  `<div class="legend">
     <span><i style="background:#6FE3BE"></i>Spent</span>
     <span><i style="background:rgba(111,227,190,.26)"></i>Left</span>
     <span><i style="background:#F5C26B"></i>Close to target</span>
     <span><i style="background:#FF6B8A"></i>Over</span>
     <span><i style="background:rgba(169,155,201,.5)"></i>No target set</span>
   </div>`
  : '<p class="empty">Add a target or some transactions.</p>';

  renderNeedSort();
  renderCompare();

  if (!inView.length){ $('txlist').innerHTML = '<p class="empty">Nothing in this month.</p>'; return; }
  const sorted = tx.map((t,i)=>({...t,i})).filter(t => view==='ALL' || t.period===view)
                   .sort((a,b)=>b.amt-a.amt);
  $('txlist').innerHTML = '<div class="scroll"><table><thead><tr><th>Date</th><th>Merchant</th><th>Category</th><th class="amt">Amount</th><th></th></tr></thead><tbody>' +
    sorted.map(t => `<tr>
      <td class="day">${t.day||''}</td>
      <td class="merch" title="${t.desc.replace(/"/g,'')}">${t.desc}</td>
      <td><select class="cat ${t.sure?'':'guessed'}" data-id="${t.id}">${
        list.map(c=>`<option${c===t.cat?' selected':''}>${c}</option>`).join('')}</select></td>
      <td class="amt"><input class="amtin" type="number" inputmode="decimal" min="0" step="0.01"
           value="${t.amt.toFixed(2)}" data-id="${t.id}" aria-label="Amount"></td>
      <td class="kill"><button class="x" data-kill="${t.id}" title="Delete">&times;</button></td>
    </tr>`).join('') + '</tbody></table></div>' +
    '<p class="hint">Tap an amount to correct it. Tap \u00d7 twice to delete one transaction.</p>';

  $('txlist').querySelectorAll('select').forEach(s => s.addEventListener('change', e => {
    const t = tx.find(x => x.id === e.target.dataset.id); if (!t) return;
    const k = key(t.desc);
    learned[k] = e.target.value;
    tx.forEach(o => { if (key(o.desc)===k){ o.cat = e.target.value; o.sure = true; } });
    save(); render();
  }));

  $('txlist').querySelectorAll('input.amtin').forEach(inp => {
    inp.addEventListener('change', e => {
      const t = tx.find(x => x.id === e.target.dataset.id); if (!t) return;
      const v = parseFloat(e.target.value);
      if (!(v > 0)){ e.target.value = t.amt.toFixed(2); say('An amount has to be more than zero.','bad'); return; }
      const was = t.amt; t.amt = Math.round(v*100)/100;
      save(); render();
      if (Math.abs(was - t.amt) >= 0.01)
        say(`${t.desc} changed from ${money(was)} to ${money(t.amt)}.`, 'good');
    });
    inp.addEventListener('focus', e => e.target.select());
  });

  $('txlist').querySelectorAll('[data-kill]').forEach(b => b.addEventListener('click', e => {
    const t = tx.find(x => x.id === e.target.dataset.kill); if (!t) return;
    arm(e.target, 'kill:'+t.id, '\u2713', () => {
      const gone = t.desc, amt = t.amt;
      tx = tx.filter(x => x.id !== t.id);
      const p = periods(); if (view !== 'ALL' && !p.includes(view)) view = p.length ? p[p.length-1] : 'ALL';
      save(); render();
      say(`Deleted ${gone}, ${money(amt)}.`, 'good');
    });
  }));
}

function commit(rows, src){
  tx = tx.concat(rows);
  const p = [...new Set(rows.map(r=>r.period))].sort();
  view = p[p.length-1]; save(); render();
  say('Added ' + rows.length + ' transactions' +
      (p.length===1 ? ' to ' + label(p[0]) : ' across ' + p.length + ' months') +
      (src ? ' from ' + src : '') + '.', 'good');
}

function ingest(text, src){
  const rows = parse(text);
  if (!rows.length){ say('No transactions found in that file.', 'bad'); return; }
  // guard against loading the same statement twice
  const sig = t => t.period+'|'+t.day+'|'+t.desc+'|'+t.amt;
  const have = new Set(tx.map(sig));
  const dupes = rows.filter(r => have.has(sig(r))).length;
  if (dupes > rows.length*0.6){
    say(`${dupes} of these ${rows.length} are already loaded. Looks like a statement you have added before.`,
        null, [{label:'Add anyway', run:()=>commit(rows, src)}, {label:'Cancel', run:hide}]);
    return;
  }
  commit(rows, src);
}

async function pdfToText(file){
  pdfjsLib.GlobalWorkerOptions.workerSrc =
    'https://cdnjs.cloudflare.com/ajax/libs/pdf.js/3.11.174/pdf.worker.min.js';
  const pdf = await pdfjsLib.getDocument({data: await file.arrayBuffer()}).promise;
  const lines = [];
  for (let p = 1; p <= pdf.numPages; p++){
    const tc = await (await pdf.getPage(p)).getTextContent();
    const rows = {};
    tc.items.forEach(it => {
      if (!it.str.trim()) return;
      const k = Math.round(it.transform[5]/3)*3;
      (rows[k] = rows[k] || []).push({x: it.transform[4], s: it.str});
    });
    Object.keys(rows).map(Number).sort((a,b)=>b-a).forEach(k =>
      lines.push(rows[k].sort((a,b)=>a.x-b.x).map(o=>o.s).join(' ').replace(/\s+/g,' ')));
  }
  return lines.join('\n');
}

$('add').addEventListener('click', () => { ingest($('input').value); $('input').value=''; });
$('pick').addEventListener('click', () => $('file').click());
$('file').addEventListener('change', async e => {
  const f = e.target.files[0]; if (!f) return; e.target.value = '';
  if (/\.pdf$/i.test(f.name) || f.type === 'application/pdf'){
    say('Reading ' + f.name + '\u2026');
    try { ingest(await pdfToText(f), f.name); }
    catch(err){ say('Could not read that PDF. Scans and photos will not work, only real statements.', 'bad'); }
    return;
  }
  const r = new FileReader();
  r.onload = () => ingest(r.result, f.name);
  r.onerror = () => say('Could not read that file.', 'bad');
  r.readAsText(f);
});
$('backup').addEventListener('click', () => {
  const blob = new Blob([JSON.stringify({v:1, saved:new Date().toISOString(),
                                         tx, learned, targets, fixed, monthly, cents}, null, 1)],
                        {type:'application/json'});
  const d = new Date(), pad = n => String(n).padStart(2,'0');
  const name = `budget-backup-${d.getFullYear()}-${pad(d.getMonth()+1)}-${pad(d.getDate())}.json`;
  const url = URL.createObjectURL(blob);
  const a = document.createElement('a');
  a.href = url; a.download = name; a.rel = 'noopener';
  document.body.appendChild(a); a.click(); a.remove();
  setTimeout(() => URL.revokeObjectURL(url), 4000);
  say(`Saved ${name} with ${tx.length} transactions. Keep it somewhere off this phone.`, 'good');
});

$('restore').addEventListener('click', () => $('bfile').click());
$('bfile').addEventListener('change', e => {
  const f = e.target.files[0]; if (!f) return; e.target.value = '';
  const r = new FileReader();
  r.onload = () => {
    let d;
    try { d = JSON.parse(r.result); } catch(err){ say('That is not a backup file.', 'bad'); return; }
    if (!d || !Array.isArray(d.tx)){ say('That file has no transactions in it.', 'bad'); return; }
    say(`This backup holds ${d.tx.length} transactions. Restoring replaces everything on this phone.`,
        null, [
      {label:'Replace everything', run:() => {
        tx = d.tx.map(t => ({...t, id: t.id || uid(), period: t.period || thisPeriod(), day: t.day || ''}));
        learned = d.learned || {};
        if (d.targets && Object.keys(d.targets).length) targets = d.targets;
        if (targets['Other'] === undefined) targets['Other'] = 0;
        if (typeof d.fixed === 'number') fixed = d.fixed;
        if (typeof d.monthly === 'number') monthly = d.monthly;
        cents = !!d.cents;
        const p = periods(); view = p.length ? p[p.length-1] : 'ALL';
        save(); renderSettings(); render();
        say(`Restored ${tx.length} transactions.`, 'good');
      }},
      {label:'Cancel', run:hide}]);
  };
  r.onerror = () => say('Could not read that file.', 'bad');
  r.readAsText(f);
});

$('month').addEventListener('change', e => { view = e.target.value; render(); });
$('delMonth').addEventListener('click', e => {
  if (view === 'ALL') return;
  const gone = label(view), n = tx.filter(t=>t.period===view).length;
  arm(e.target, 'delmonth', `Delete ${n}? Tap again`, () => {
    tx = tx.filter(t => t.period !== view);
    const p = periods(); view = p.length ? p[p.length-1] : 'ALL';
    save(); render();
    say(`Deleted ${n} transactions from ${gone}.`, 'good');
  });
});
$('toggleSet').addEventListener('click', () => {
  const open = $('settings').classList.toggle('hidden');
  $('toggleSet').textContent = open ? 'Edit' : 'Done';
  $('setsummary').classList.toggle('hidden', !open);
});
function snapshot(){
  return JSON.stringify({tx, learned, targets, fixed, monthly, cents, saved:new Date().toISOString()});
}
$('backup').addEventListener('click', () => {
  try {
    const a = document.createElement('a');
    a.href = URL.createObjectURL(new Blob([snapshot()], {type:'application/json'}));
    a.download = 'budget-backup-' + new Date().toISOString().slice(0,10) + '.json';
    document.body.appendChild(a); a.click(); a.remove();
    setTimeout(() => URL.revokeObjectURL(a.href), 2000);
    say('Backup saved. Check your Files app under Downloads.', 'good');
  } catch(e){ say('Download did not work here. Use Copy to clipboard instead.', 'bad'); }
});
$('copybk').addEventListener('click', async () => {
  const s = snapshot();
  try { await navigator.clipboard.writeText(s); say('Copied. Paste it into a note or email it to yourself.', 'good'); }
  catch(e){
    const t = $('bktext'); t.classList.remove('hidden'); t.value = s; t.focus(); t.select();
    say('Copy it from the box below and keep it somewhere safe.', null);
  }
});
$('restore').addEventListener('click', e => {
  arm(e.target, 'restore', 'Replaces everything. Tap again', () => $('bkfile').click());
});
$('bkfile').addEventListener('change', ev => {
  const f = ev.target.files[0]; if (!f) return; ev.target.value = '';
  const r = new FileReader();
  r.onload = () => {
    try {
      const d = JSON.parse(r.result);
      if (!Array.isArray(d.tx)) throw 0;
      tx = d.tx.map(t => ({...t, id: t.id || uid(), period: t.period || thisPeriod(), day: t.day || ''}));
      learned = d.learned || {};
      if (d.targets && Object.keys(d.targets).length) targets = d.targets;
      if (targets['Other'] === undefined) targets['Other'] = 0;
      if (typeof d.fixed === 'number') fixed = d.fixed;
      if (typeof d.monthly === 'number') monthly = d.monthly;
      cents = !!d.cents;
      const p = periods(); view = p.length ? p[p.length-1] : 'ALL';
      save(); renderSettings(); render();
      say('Restored ' + tx.length + ' transactions across ' + p.length + ' month' + (p.length===1?'':'s') + '.', 'good');
    } catch(err){ say('That is not a backup file from this app.', 'bad'); }
  };
  r.onerror = () => say('Could not read that file.', 'bad');
  r.readAsText(f);
});
$('cents').addEventListener('change', e => { cents = e.target.checked; save(); render(); updateAlloc(); });
$('monthly').addEventListener('input', e => { monthly = Math.max(0,+e.target.value||0); save(); render(); updateAlloc(); });
$('fixed').addEventListener('input', e => { fixed = Math.max(0,+e.target.value||0); save(); render(); updateAlloc(); });
$('addcat').addEventListener('click', () => {
  const name = $('newcat').value.trim(); if (!name) return;
  if (targets[name] !== undefined){ say('That category already exists.', 'bad'); return; }
  const other = targets['Other']; delete targets['Other'];
  targets[name] = 0; targets['Other'] = other;
  $('newcat').value = ''; save(); renderSettings(); render();
});
$('newcat').addEventListener('keydown', e => { if (e.key === 'Enter') $('addcat').click(); });
load();
</script>
</body>
</html>
