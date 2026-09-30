<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>Ali Book</title>
<style>
body{margin:0;font-family:Tahoma;background:#f4f7ff;color:#182033}
header{background:linear-gradient(135deg,#2563eb,#7c3aed);color:white;text-align:center;padding:45px 15px;border-radius:0 0 30px 30px}
h1{font-size:38px;margin:10px}
.search{display:block;width:85%;max-width:700px;margin:-25px auto 25px;padding:17px;border:0;border-radius:15px;box-shadow:0 5px 20px #0002;font-size:16px}
.grid{max-width:1000px;margin:auto;padding:15px;display:grid;grid-template-columns:repeat(auto-fit,minmax(210px,1fr));gap:18px}
.card{background:white;padding:25px;border-radius:20px;text-align:center;box-shadow:0 5px 20px #0001}
.icon{font-size:45px}
button{background:#2563eb;color:white;border:0;border-radius:10px;padding:12px 25px;font-size:15px}
footer{text-align:center;padding:30px;color:#777}
</style>
</head>
<body>

<header>
<div style="font-size:55px">📚</div>
<h1>Ali Book</h1>
<p>کتابخانه کتاب‌های درسی</p>
</header>

<input class="search" id="search" placeholder="🔎 جستجوی کتاب..." oninput="search()">

<div class="grid">

<div class="card"><div class="icon">📐</div><h2>ریاضی ششم</h2><button>مشاهده کتاب</button></div>

<div class="card"><div class="icon">🔬</div><h2>علوم تجربی ششم</h2><button>مشاهده کتاب</button></div>

<div class="card"><div class="icon">🌍</div><h2>مطالعات اجتماعی ششم</h2><button>مشاهده کتاب</button></div>

<div class="card"><div class="icon">📖</div><h2>قرآن ششم</h2><button>مشاهده کتاب</button></div>

<div class="card"><div class="icon">💡</div><h2>تفکر و پژوهش ششم</h2><button>مشاهده کتاب</button></div>

<div class="card"><div class="icon">📕</div><h2>فارسی ششم</h2><button>مشاهده کتاب</button></div>

<div class="card"><div class="icon">✏️</div><h2>نگارش فارسی ششم</h2><button>مشاهده کتاب</button></div>

<div class="card"><div class="icon">💻</div><h2>کار و فناوری ششم</h2><button>مشاهده کتاب</button></div>

<div class="card"><div class="icon">🌙</div><h2>هدیه‌های آسمان ششم</h2><button>مشاهده کتاب</button></div>

</div>

<footer>Ali Book 📚</footer>

<script>
function search(){
let x=document.getElementById("search").value.toLowerCase();
document.querySelectorAll(".card").forEach(c=>{
c.style.display=c.innerText.toLowerCase().includes(x)?"block":"none";
});
}
</script>

</body>
</html>
