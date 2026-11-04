<!doctype html>
<html lang="ar" dir="rtl">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1,maximum-scale=1,user-scalable=no">
<meta name="theme-color" content="#09090d">
<title>ROX AI Studio</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Alexandria:wght@400;500;600;700;800&display=swap" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/@supabase/supabase-js@2"></script>
<style>
:root{--bg:#09090d;--panel:#12121a;--panel2:#191925;--line:#29283a;--purple:#9565ff;--pink:#d45cff;--text:#f7f5ff;--muted:#aaa6bd;--good:#67dfb0}
*{box-sizing:border-box}body{margin:0;background:radial-gradient(ellipse at 80% -10%,#32204f 0,transparent 35%),var(--bg);color:var(--text);font-family:Alexandria,system-ui,sans-serif;min-height:100vh}button,input,textarea{font:inherit}button{cursor:pointer;border:0}.hidden{display:none!important}.wrap{max-width:1100px;margin:auto;padding:18px 16px 100px}.top{display:flex;align-items:center;justify-content:space-between;gap:12px;margin-bottom:22px}.brand{display:flex;align-items:center;gap:10px;font-weight:800;font-size:20px;letter-spacing:.3px}.logo{width:42px;height:42px;border-radius:15px;background:linear-gradient(145deg,#bd83ff,#6332d5);display:grid;place-items:center;box-shadow:0 8px 30px #8b54ff55;font-size:20px}.pill{border:1px solid var(--line);background:#ffffff09;color:var(--muted);padding:9px 12px;border-radius:30px;font-size:12px}.hero{padding:25px;border:1px solid #51406d;border-radius:25px;background:linear-gradient(130deg,#251a38,#14121e 65%,#21172c);position:relative;overflow:hidden}.hero:after{content:"✦";position:absolute;font-size:150px;left:20px;top:-40px;color:#ffffff09}.eyebrow{color:#c8aaff;font-size:12px}.hero h1{font-size:clamp(25px,5vw,40px);margin:12px 0}.hero p{color:#c1bad1;line-height:1.9;max-width:650px;font-size:13px}.primary{background:linear-gradient(100deg,#9c68ff,#7041dd);color:white;border-radius:13px;padding:13px 18px;font-weight:700;box-shadow:0 8px 25px #7846df44}.secondary{background:#ffffff0b;color:white;border:1px solid var(--line);border-radius:13px;padding:12px 15px}.grid{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:12px;margin-top:17px}.tile,.card{background:linear-gradient(145deg,#171722,#101018);border:1px solid var(--line);border-radius:19px;padding:17px;text-align:right;color:var(--text);min-width:0}.tile{min-height:122px;transition:.2s}.tile:active{transform:scale(.98)}.tile .ico{font-size:23px}.tile b{display:block;margin:10px 0 5px;font-size:14px}.tile small{color:var(--muted);font-size:11px;line-height:1.7}.section{margin-top:25px}.sectionhead{display:flex;justify-content:space-between;align-items:center;margin-bottom:12px}.sectionhead h2{font-size:17px;margin:0}.muted{color:var(--muted);font-size:12px;line-height:1.9}.auth{max-width:470px;margin:8vh auto;padding:25px;background:#12121a;border:1px solid var(--line);border-radius:24px;box-shadow:0 25px 80px #0008}.auth h2{margin:5px 0 8px;font-size:23px}.field{width:100%;padding:14px 13px;margin-top:10px;background:#0b0b11;border:1px solid #302d42;border-radius:12px;color:white;outline:none}.field:focus{border-color:var(--purple)}.wide{width:100%;margin-top:12px}.google{background:#fff;color:#20202a;border-radius:12px;padding:13px;width:100%;font-weight:700;margin-top:12px}.or{display:flex;align-items:center;gap:10px;color:#77738a;font-size:11px;margin:15px 0}.or:before,.or:after{content:"";height:1px;background:var(--line);flex:1}.switch{color:#c6a8ff;background:none;margin-top:15px;width:100%;font-size:12px}.choice{display:flex;gap:9px;margin:12px 0}.choice button{flex:1}.stats{display:grid;grid-template-columns:repeat(3,1fr);gap:9px}.stat{background:#ffffff08;border:1px solid var(--line);padding:13px;border-radius:15px}.stat strong{display:block;font-size:20px}.stat small{font-size:10px;color:var(--muted)}.refbox{background:#0c0b13;border:1px dashed #7053a9;border-radius:14px;padding:14px;word-break:break-all;font-size:12px;color:#d7c6ff}.bottom{position:fixed;bottom:0;left:0;right:0;background:#0c0b12ed;backdrop-filter:blur(18px);border-top:1px solid var(--line);display:flex;justify-content:space-around;padding:9px 4px calc(9px + env(safe-area-inset-bottom));z-index:5}.nav{background:none;color:#89859a;font-size:10px;display:grid;gap:4px;justify-items:center;min-width:55px}.nav span{font-size:19px}.nav.active{color:#c5a6ff}.notice{padding:12px;border-radius:12px;background:#2b2140;color:#d9caff;font-size:11px;line-height:1.8;margin-top:12px}.toast{position:fixed;top:15px;left:15px;right:15px;z-index:10;background:#252034;border:1px solid #66508b;padding:13px;border-radius:13px;text-align:center;font-size:12px;display:none}.area{width:100%;min-height:115px;resize:vertical}.toolrow{display:flex;gap:9px;flex-wrap:wrap}.toolrow>*{flex:1}.profileline{display:flex;align-items:center;gap:12px}.avatar{width:48px;height:48px;border-radius:16px;background:linear-gradient(140deg,#a16bff,#43208d);display:grid;place-items:center;font-size:21px}
@media(min-width:700px){.grid{grid-template-columns:repeat(4,minmax(0,1fr))}.wrap{padding-top:28px}.hero{padding:38px}.auth{margin-top:10vh}}
</style>
</head>
<body>
<div id="toast" class="toast"></div>
<div id="authView" class="wrap">
 <div class="top"><div class="brand"><div class="logo">✦</div> ROX AI <span class="pill">STUDIO</span></div><span class="pill">منصة الإبداع الذكي</span></div>
 <div class="auth">
  <div class="eyebrow">WELCOME TO ROX AI</div><h2 id="authTitle">أنشئ حسابك وابدأ الإبداع</h2><p class="muted">مساحة واحدة لأدوات الذكاء الاصطناعي وصناعة المحتوى.</p>
  <div id="inviteStep" class="card" style="padding:14px;margin-top:15px">
   <b style="font-size:13px">هل وصلت إلى ROX AI عن طريق صديق؟</b>
   <div class="choice"><button class="secondary" onclick="inviteChoice(true)">نعم، لدي كود دعوة</button><button class="secondary" onclick="inviteChoice(false)">لا</button></div>
   <input id="inviteCode" class="field hidden" placeholder="اكتب كود الدعوة">
  </div>
  <input id="fullName" class="field" placeholder="الاسم" autocomplete="name">
  <input id="email" class="field" type="email" placeholder="البريد الإلكتروني" autocomplete="email">
  <input id="password" class="field" type="password" placeholder="كلمة المرور (6 أحرف على الأقل)" autocomplete="new-password">
  <button class="primary wide" id="emailBtn" onclick="emailAuth()">إنشاء حساب بالبريد</button>
  <div class="or">أو</div>
  <button class="google" onclick="googleLogin()">🌐 المتابعة باستخدام Google</button>
  <button class="switch" onclick="toggleMode()" id="switchBtn">لديك حساب؟ تسجيل الدخول</button>
  <div class="notice">تسجيل Google يحتاج تفعيل مزوّد Google وإعداد رابط الرجوع في Supabase قبل استخدامه.</div>
  <p class="muted" style="text-align:center;margin-top:15px">بالمتابعة أنت توافق على شروط الاستخدام وسياسة الخصوصية.</p>
 </div>
</div>
<div id="appView" class="hidden">
 <main class="wrap">
  <div class="top"><div class="brand"><div class="logo">✦</div> ROX AI <span class="pill">STUDIO</span></div><button class="pill" onclick="logout()">تسجيل الخروج ↗</button></div>
  <section class="hero"><div class="eyebrow">YOUR CREATIVE AI SPACE</div><h1>أطلق خيالك مع <span style="color:#c7a3ff">ROX AI</span></h1><p>منصة إبداعية تجمع أدوات الذكاء الاصطناعي وصناعة المحتوى في مكان واحد. اختر أداتك وابدأ بتحويل أفكارك إلى أعمال.</p><button class="primary" onclick="openSection('assistant')">ابدأ مع ROX AI ✦</button></section>
  <section class="section"><div class="sectionhead"><h2>نظرة عامة</h2><span class="muted" id="userGreeting">مرحبًا بك</span></div><div class="stats"><div class="stat"><strong id="points">—</strong><small>رصيد النقاط</small></div><div class="stat"><strong>0</strong><small>أعمال محفوظة</small></div><div class="stat"><strong>Free</strong><small>الباقة الحالية</small></div></div></section>
  <section class="section"><div class="sectionhead"><h2>استكشف الأدوات</h2><span class="muted">مساحة الإبداع</span></div><div class="grid">
   <button class="tile" onclick="openSection('assistant')"><span class="ico">✦</span><b>مساعد ROX AI</b><small>اسأل، خطط، واكتب أفكارك</small></button>
   <button class="tile" onclick="openSection('images')"><span class="ico">▧</span><b>توليد الصور</b><small>حوّل وصفك إلى صورة</small></button>
   <button class="tile" onclick="openSection('video')"><span class="ico">▶</span><b>إنشاء الفيديو</b><small>أفكار ومشاهد فيديو</small></button>
   <button class="tile" onclick="openSection('writing')"><span class="ico">✎</span><b>صناعة المحتوى</b><small>منشورات وسيناريوهات</small></button>
   <button class="tile" onclick="openSection('design')"><span class="ico">◇</span><b>أفكار التصميم</b><small>هوية وألوان وتصميمات</small></button>
   <button class="tile" onclick="openSection('gallery')"><span class="ico">▦</span><b>معرض أعمالي</b><small>مساحة أعمالك المحفوظة</small></button>
   <button class="tile" onclick="openSection('history')"><span class="ico">◷</span><b>سجل النشاط</b><small>عملياتك السابقة</small></button>
   <button class="tile" onclick="openSection('referrals')"><span class="ico">♧</span><b>الإحالات والنقاط</b><small>ادعُ أصدقاءك واجمع النقاط</small></button>
   <button class="tile" onclick="openSection('plans')"><span class="ico">♛</span><b>الباقات</b><small>قارن مزايا الخطط</small></button>
   <button class="tile" onclick="openSection('profile')"><span class="ico">◎</span><b>حسابي</b><small>بيانات الحساب والإعدادات</small></button>
  </div></section>
  <section id="detail" class="section card"><div class="sectionhead"><h2 id="detailTitle">ابدأ رحلتك</h2><span class="pill">ROX AI</span></div><div id="detailBody" class="muted">اختر إحدى الأدوات من الأقسام لعرض تفاصيلها.</div></section>
 </main>
 <nav class="bottom"><button class="nav active" onclick="navTo('home',this)"><span>⌂</span>الرئيسية</button><button class="nav" onclick="openSection('assistant',this)"><span>✦</span>المساعد</button><button class="nav" onclick="openSection('gallery',this)"><span>▦</span>أعمالي</button><button class="nav" onclick="openSection('referrals',this)"><span>♧</span>الإحالات</button><button class="nav" onclick="openSection('profile',this)"><span>◎</span>حسابي</button></nav>
</div>
<script>
const SUPABASE_URL='https://jjtntfltnewliiptpolv.supabase.co';
const SUPABASE_KEY='sb_publishable_y_ZxbvQhhGW8GpW89KccWw_ptAcmOgp';
const db=window.supabase.createClient(SUPABASE_URL,SUPABASE_KEY);
let mode='signup', inviteAnswer=null, currentUser=null;
const $=id=>document.getElementById(id);
function toast(t){$('toast').textContent=t;$('toast').style.display='block';setTimeout(()=>$('toast').style.display='none',3600)}
function inviteChoice(v){inviteAnswer=v;$('inviteCode').classList.toggle('hidden',!v);if(!v)$('inviteCode').value=''}
function toggleMode(){mode=mode==='signup'?'login':'signup';$('authTitle').textContent=mode==='signup'?'أنشئ حسابك وابدأ الإبداع':'مرحبًا بعودتك';$('emailBtn').textContent=mode==='signup'?'إنشاء حساب بالبريد':'تسجيل الدخول';$('switchBtn').textContent=mode==='signup'?'لديك حساب؟ تسجيل الدخول':'ليس لديك حساب؟ إنشاء حساب';$('fullName').classList.toggle('hidden',mode==='login');$('inviteStep').classList.toggle('hidden',mode==='login')}
async function emailAuth(){
 const email=$('email').value.trim(),password=$('password').value,name=$('fullName').value.trim();
 if(!email||!password){toast('اكتب البريد الإلكتروني وكلمة المرور أولًا');return}
 if(mode==='signup'){
  if(!name){toast('اكتب اسمك أولًا');return}
  if(inviteAnswer===null){toast('اختر هل وصلت عن طريق صديق أم لا');return}
  if(inviteAnswer && !$('inviteCode').value.trim()){toast('اكتب كود الدعوة');return}
  const {data,error}=await db.auth.signUp({email,password,options:{data:{full_name:name,referral_code_entered:inviteAnswer?$('inviteCode').value.trim():null,joined_via_referral:!!inviteAnswer},emailRedirectTo:location.origin+location.pathname}});
  if(error){toast(error.message);return}
  toast('تم إنشاء الحساب. افحص بريدك لتأكيده. بعد التأكيد ارجع إلى الموقع وسجّل الدخول.'); 
 }else{
  const {data,error}=await db.auth.signInWithPassword({email,password});
  if(error){toast(error.message);return} await showApp(data.user);
 }
}
async function googleLogin(){
 const {error}=await db.auth.signInWithOAuth({provider:'google',options:{redirectTo:location.origin+location.pathname,queryParams:{access_type:'offline',prompt:'consent'}}});
 if(error)toast(error.message);
}
async function showApp(user){
 currentUser=user;$('authView').classList.add('hidden');$('appView').classList.remove('hidden');
 $('userGreeting').textContent='مرحبًا، '+(user.user_metadata?.full_name||user.email||'بك');
 $('points').textContent='0';
 const code='ROX'+user.id.replace(/-/g,'').slice(0,7).toUpperCase();
 $('detailTitle').textContent='مرحبًا بك في ROX AI';$('detailBody').textContent='حسابك جاهز. اختر أداة من الأقسام للبدء.';
}
async function logout(){await db.auth.signOut();currentUser=null;$('appView').classList.add('hidden');$('authView').classList.remove('hidden')}
function navTo(where,el){document.querySelectorAll('.nav').forEach(x=>x.classList.remove('active'));if(el)el.classList.add('active');if(where==='home'){$('detailTitle').textContent='ابدأ رحلتك';$('detailBody').textContent='اختر إحدى الأدوات من الأقسام لعرض تفاصيلها.'}}
function openSection(key,el){
 if(el){document.querySelectorAll('.nav').forEach(x=>x.classList.remove('active'));el.classList.add('active')}
 const titles={assistant:'مساعد ROX AI',images:'توليد الصور',video:'إنشاء الفيديوهات',writing:'صناعة المحتوى',design:'أفكار التصميم',gallery:'معرض أعمالي',history:'سجل النشاط',referrals:'الإحالات وجمع النقاط',plans:'الباقات والاشتراكات',profile:'حسابي والإعدادات'};
 $('detailTitle').textContent=titles[key]||'ROX AI';
 const referral=key==='referrals';
 if(referral){
  const code='ROX'+currentUser.id.replace(/-/g,'').slice(0,7).toUpperCase();
  const link=location.origin+location.pathname+'?ref='+code;
  $('detailBody').innerHTML=`<p>شارك رابطك مع أصدقائك. بعد اكتمال التسجيل والتحقق من الحساب، يمكن احتساب المكافآت من خلال نظام الإحالات الآمن.</p><div class="refbox" id="refLink">${link}</div><div class="toolrow" style="margin-top:10px"><button class="primary" onclick="copyRef()">نسخ رابط الدعوة</button><button class="secondary" onclick="copyCode('${code}')">نسخ الكود ${code}</button></div><div class="notice">مكافأة مقترحة: 20 نقطة لصاحب الدعوة و10 نقاط للمستخدم الجديد. عرض الرابط هنا لا يعني أن النقاط تُضاف تلقائيًا بعد؛ يلزم تفعيل وظيفة آمنة في قاعدة البيانات لمنع التلاعب والتكرار.</div>`;
 }else if(key==='assistant'||key==='writing'||key==='images'||key==='video'||key==='design'){
  $('detailBody').innerHTML=`<p>هذه مساحة الأداة داخل ROX AI. واجهة القسم جاهزة للتصميم، لكن التوليد الفعلي يحتاج ربط خدمة ذكاء اصطناعي من خلال خادم آمن.</p><textarea class="field area" placeholder="اكتب فكرتك أو وصفك هنا..."></textarea><button class="primary wide" onclick="toast('سيتم تفعيل التوليد بعد ربط محرك الذكاء الاصطناعي')">ابدأ الإنشاء</button>`;
 }else if(key==='plans'){
  $('detailBody').innerHTML='<div class="grid"><div class="tile"><b>Free</b><small>تجربة أساسية ونقاط مجانية</small></div><div class="tile"><b>Pro</b><small>حدود أعلى وأدوات أكثر</small></div><div class="tile"><b>Ultra</b><small>تجربة موسعة للمبدعين</small></div></div><p class="muted">الاشتراكات والدفع غير مفعّلين بعد.</p>';
 }else if(key==='profile'){
  $('detailBody').innerHTML=`<div class="profileline"><div class="avatar">✦</div><div><b>${currentUser.email||'مستخدم ROX'}</b><div class="muted">حساب ROX AI</div></div></div><p class="muted">يمكنك تسجيل الخروج من الزر أعلى الصفحة.</p>`;
 }else{$('detailBody').textContent=key==='gallery'?'سيظهر هنا المحتوى الذي تنشئه وتحفظه بعد تفعيل محرك التوليد والتخزين.':'سيظهر هنا سجل نشاطك بعد ربط قاعدة البيانات.'}
 $('detail').scrollIntoView({behavior:'smooth',block:'start'});
}
function copyRef(){const t=$('refLink').textContent;navigator.clipboard?.writeText(t).then(()=>toast('تم نسخ رابط الدعوة')).catch(()=>toast(t))}
function copyCode(t){navigator.clipboard?.writeText(t).then(()=>toast('تم نسخ الكود')).catch(()=>toast(t))}
const params=new URLSearchParams(location.search);const incoming=params.get('ref');if(incoming){inviteAnswer=true;$('inviteCode').value=incoming;$('inviteCode').classList.remove('hidden')}
db.auth.getSession().then(({data})=>{if(data.session)showApp(data.session.user)});
db.auth.onAuthStateChange((_event,session)=>{if(session&&!currentUser)showApp(session.user)});
</script>
</body></html>
