<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sound Rest — расслабляющий тимбилдинг</title>

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
}

body{
font-family:Arial, sans-serif;
background:#f8f5f0;
color:#111;
line-height:1.5;
}

.container{
width:92%;
max-width:1200px;
margin:auto;
}

header{
position:fixed;
top:0;
left:0;
width:100%;
background:rgba(255,255,255,0.9);
backdrop-filter:blur(12px);
z-index:100;
border-bottom:1px solid rgba(0,0,0,0.05);
}

.nav{
height:80px;
display:flex;
justify-content:space-between;
align-items:center;
}

.logo{
font-size:28px;
font-weight:700;
}

.menu{
display:flex;
gap:30px;
}

.menu a{
text-decoration:none;
color:#333;
font-size:15px;
}

.hero{
padding-top:140px;
padding-bottom:100px;
background:
radial-gradient(circle at top right,#dde8ef,transparent 30%),
radial-gradient(circle at left,#eadcc8,transparent 35%);
}

.hero-grid{
display:grid;
grid-template-columns:1fr 1fr;
gap:60px;
align-items:center;
}

.hero h1{
font-size:72px;
line-height:0.95;
margin-bottom:30px;
}

.hero p{
font-size:24px;
color:#444;
margin-bottom:35px;
}

.buttons{
display:flex;
gap:20px;
flex-wrap:wrap;
}

.btn{
padding:18px 34px;
border-radius:999px;
text-decoration:none;
font-weight:bold;
display:inline-block;
transition:0.2s;
}

.btn-dark{
background:#111;
color:white;
}

.btn-light{
border:1px solid #999;
color:#111;
}

.btn:hover{
transform:translateY(-2px);
}

.circle{
width:500px;
height:500px;
border-radius:50%;
background:
linear-gradient(145deg,#d7c0a1,#8f6748 50%,#566f5a);
margin:auto;
position:relative;
overflow:hidden;
box-shadow:0 30px 90px rgba(0,0,0,0.18);
}

.circle:before{
content:'';
position:absolute;
width:250px;
height:250px;
border-radius:50%;
border:22px solid rgba(255,255,255,0.6);
top:50%;
left:50%;
transform:translate(-50%,-50%);
}

section{
padding:110px 0;
}

.center{
text-align:center;
max-width:850px;
margin:auto;
margin-bottom:60px;
}

h2{
font-size:64px;
line-height:1;
margin-bottom:25px;
}

.subtitle{
font-size:24px;
color:#555;
}

.cards{
display:grid;
grid-template-columns:repeat(3,1fr);
gap:25px;
}

.card{
background:white;
padding:35px;
border-radius:32px;
box-shadow:0 20px 60px rgba(0,0,0,0.06);
}

.number{
width:55px;
height:55px;
border-radius:50%;
background:#111;
color:white;
display:flex;
align-items:center;
justify-content:center;
font-weight:bold;
margin-bottom:25px;
}

.card h3{
font-size:28px;
margin-bottom:15px;
}

.card p{
color:#666;
font-size:18px;
}

.soft{
background:white;
}

.split{
display:grid;
grid-template-columns:1fr 1fr;
gap:70px;
align-items:center;
}

.round{
width:450px;
height:450px;
border-radius:50%;
background:
linear-gradient(145deg,#cba57f,#566f5a);
margin:auto;
box-shadow:0 25px 80px rgba(0,0,0,0.15);
}

.text p{
font-size:22px;
margin-bottom:20px;
color:#444;
}

.quote{
padding:35px;
background:#fff7ed;
border-left:4px solid #8f6748;
border-radius:0 30px 30px 0;
font-size:26px;
margin-top:30px;
}

.program{
display:grid;
gap:20px;
max-width:950px;
margin:auto;
}

.step{
background:white;
padding:30px;
border-radius:28px;
display:grid;
grid-template-columns:150px 1fr;
gap:25px;
}

.time{
font-weight:bold;
color:#8f6748;
}

.step h3{
font-size:30px;
margin-bottom:10px;
}

.step p{
color:#666;
font-size:18px;
}

.dark{
background:#101010;
color:white;
}

.dark .subtitle{
color:rgba(255,255,255,0.7);
}

.grid2{
display:grid;
grid-template-columns:1fr 1fr;
gap:22px;
}

.dark-card{
background:rgba(255,255,255,0.06);
padding:35px;
border-radius:30px;
}

.dark-card h3{
font-size:28px;
margin-bottom:15px;
}

.dark-card p{
color:rgba(255,255,255,0.72);
font-size:18px;
}

.instruments{
display:grid;
grid-template-columns:repeat(5,1fr);
gap:16px;
}

.instrument{
background:white;
padding:28px;
border-radius:30px;
text-align:center;
}

.icon{
width:90px;
height:90px;
border-radius:50%;
margin:auto;
margin-bottom:20px;
background:
linear-gradient(145deg,#e8c18e,#5d4635);
}

.instrument h3{
font-size:22px;
margin-bottom:10px;
}

.instrument p{
font-size:15px;
color:#666;
}

.results{
display:grid;
gap:16px;
max-width:900px;
margin:auto;
}

.result{
background:white;
padding:24px;
border-radius:24px;
font-size:20px;
display:flex;
gap:18px;
align-items:flex-start;
}

.check{
width:40px;
height:40px;
border-radius:50%;
background:#566f5a;
color:white;
display:flex;
align-items:center;
justify-content:center;
font-weight:bold;
}

.contacts{
background:
linear-gradient(180deg,#fff,#f7f4ef);
}

.contact-box{
background:#111;
color:white;
padding:70px;
border-radius:42px;
text-align:center;
max-width:1000px;
margin:auto;
}

.contact-box p{
font-size:22px;
color:rgba(255,255,255,0.7);
margin-bottom:35px;
}

.contact-buttons{
display:flex;
justify-content:center;
gap:20px;
flex-wrap:wrap;
margin-bottom:30px;
}

.contact-buttons .btn-dark{
background:white;
color:#111;
}

.contact-buttons .btn-light{
color:white;
border:1px solid rgba(255,255,255,0.3);
}

footer{
padding:35px;
text-align:center;
font-size:14px;
color:#666;
}

@media(max-width:900px){

.hero-grid,
.split,
.cards,
.grid2,
.instruments{
grid-template-columns:1fr;
}

.hero h1{
font-size:48px;
}

h2{
font-size:42px;
}

.circle,
.round{
width:320px;
height:320px;
}

.step{
grid-template-columns:1fr;
}

.contact-box{
padding:40px 25px;
}

}

</style>
</head>

<body>

<header>
<div class="container nav">
<div class="logo">Sound Rest</div>

<div class="menu">
<a href="#">О формате</a>
<a href="#">Программа</a>
<a href="#">Музыка</a>
<a href="#">Контакты</a>
</div>
</div>
</header>

<section class="hero">

<div class="container hero-grid">

<div>

<h1>
Команда устала.<br>
Мы привезём<br>
ей глубокий выдох.
</h1>

<p>
Крепкая йога, понятная наука о стрессе и час шавасаны под живую этническую музыку.
</p>

<div class="buttons">
<a href="#" class="btn btn-dark">Обсудить выезд</a>
<a href="#" class="btn btn-light">Как это проходит</a>
</div>

</div>

<div class="circle"></div>

</div>
</section>

<section>

<div class="container">

<div class="center">

<h2>
Телесный отдых,<br>
который реально чувствуется
</h2>

<div class="subtitle">
Не просто йога. Это целый опыт расслабления через движение, дыхание и живой звук.
</div>

</div>

<div class="cards">

<div class="card">
<div class="number">1</div>
<h3>Крепкая практика</h3>
<p>
Мягкая, но ощутимая нагрузка для спины, шеи, плеч и таза.
</p>
</div>

<div class="card">
<div class="number">2</div>
<h3>Научное объяснение</h3>
<p>
Понятно рассказываем, как стресс живёт в теле и почему появляются зажимы.
</p>
</div>

<div class="card">
<div class="number">3</div>
<h3>Живая музыка</h3>
<p>
Шавасана под ханги, чаши, бубны, звонницу и хрустальную арфу.
</p>
</div>

</div>

</div>
</section>

<section class="soft">

<div class="container split">

<div class="round"></div>

<div class="text">

<h2>
Не разогнать,<br>
а восстановить
</h2>

<p>
Обычные тимбилдинги требуют ещё больше энергии.
</p>

<p>
Наш формат наоборот помогает команде сбросить напряжение и по-настоящему отдохнуть.
</p>

<div class="quote">
«Люди приходят уставшими, а уходят с ощущением — я наконец выдохнул.»
</div>

</div>

</div>

</section>

<section>

<div class="container">

<div class="center">

<h2>Как проходит выезд</h2>

<div class="subtitle">
От камерной встречи до большого корпоративного ретрита.
</div>

</div>

<div class="program">

<div class="step">
<div class="time">10–15 мин</div>
<div>
<h3>Мягкий вход</h3>
<p>
Объясняем формат и снимаем тревогу.
</p>
</div>
</div>

<div class="step">
<div class="time">45–60 мин</div>
<div>
<h3>Йога и мобилизация</h3>
<p>
Дыхание, движение и работа с телом.
</p>
</div>
</div>

<div class="step">
<div class="time">15 мин</div>
<div>
<h3>Мини-лекция</h3>
<p>
Как стресс влияет на нервную систему и мышцы.
</p>
</div>
</div>

<div class="step">
<div class="time">60 мин</div>
<div>
<h3>Шавасана и музыка</h3>
<p>
Участники лежат и отдыхают под живые инструменты.
</p>
</div>
</div>

</div>

</div>

</section>

<section class="dark">

<div class="container">

<div class="center">

<h2>
Почему это работает
</h2>

<div class="subtitle">
Без мистики — через внимание, ритм и нервную систему.
</div>

</div>

<div class="grid2">

<div class="dark-card">
<h3>После движения легче расслабиться</h3>
<p>
Тело уже включилось в ощущения и перестаёт жить только в голове.
</p>
</div>

<div class="dark-card">
<h3>Ритм успокаивает мозг</h3>
<p>
Повторяющиеся звуки снижают внутренний шум.
</p>
</div>

<div class="dark-card">
<h3>Обертоны создают объём</h3>
<p>
Чаши и ханги создают ощущение глубокого пространства.
</p>
</div>

<div class="dark-card">
<h3>Команда отдыхает вместе</h3>
<p>
Без соревнования и давления — только общий спокойный опыт.
</p>
</div>

</div>

</div>

</section>

<section>

<div class="container">

<div class="center">

<h2>Инструменты</h2>

<div class="subtitle">
Живой акустический сет для глубокого расслабления.
</div>

</div>

<div class="instruments">

<div class="instrument">
<div class="icon"></div>
<h3>Ханги</h3>
<p>Тёплый медитативный ритм</p>
</div>

<div class="instrument">
<div class="icon"></div>
<h3>Чаши</h3>
<p>Длинные обертоны</p>
</div>

<div class="instrument">
<div class="icon"></div>
<h3>Бубны</h3>
<p>Глубокий пульс</p>
</div>

<div class="instrument">
<div class="icon"></div>
<h3>Арфа</h3>
<p>Воздушное звучание</p>
</div>

<div class="instrument">
<div class="icon"></div>
<h3>Звонница</h3>
<p>Чистые переливы</p>
</div>

</div>

</div>

</section>

<section class="contacts">

<div class="container">

<div class="contact-box">

<h2>
Хотите такой формат для своей команды?
</h2>

<p>
Обсудим площадку, количество участников и формат выезда.
</p>

<div class="contact-buttons">

<a href="#" class="btn btn-dark">
Telegram
</a>

<a href="#" class="btn btn-light">
Email
</a>

</div>

<div>
Москва • выезды по России
</div>

</div>

</div>

</section>

<footer>
Sound Rest • выездные практики расслабления
</footer>

</body>
</html>