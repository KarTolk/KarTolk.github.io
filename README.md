<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Екатерина Андриянова | Portfolio</title>

<style>
:root{
    --bg:#f7f7f9;
    --card:#ffffff;
    --text:#1d1d1f;
    --accent:#6c63ff;
    --border:rgba(0,0,0,0.08);
    --shadow:0 15px 40px rgba(0,0,0,0.08);
}

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    font-family:-apple-system,BlinkMacSystemFont,"Segoe UI",sans-serif;
    background:var(--bg);
    color:var(--text);
    line-height:1.6;
}

section{
    padding:100px 8%;
}

.container{
    max-width:1400px;
    margin:0 auto;
}

h1{
    font-size:clamp(2.5rem,5vw,5rem);
    line-height:1;
    margin-bottom:20px;
}

h2{
    font-size:clamp(2rem,4vw,3rem);
    margin-bottom:40px;
}

h3{
    margin-bottom:10px;
}

p{
    color:#4b4b4b;
}

.nav{
    position:fixed;
    top:20px;
    left:50%;
    transform:translateX(-50%);
    z-index:1000;
    backdrop-filter:blur(15px);
    background:rgba(255,255,255,0.75);
    border:1px solid rgba(255,255,255,0.4);
    border-radius:100px;
    padding:12px 20px;
    box-shadow:var(--shadow);
}

.nav ul{
    display:flex;
    gap:20px;
    list-style:none;
}

.nav a{
    text-decoration:none;
    color:var(--text);
    font-weight:500;
    transition:.3s;
}

.nav a:hover{
    color:var(--accent);
}

.hero{
    min-height:100vh;
    display:flex;
    align-items:center;
}

.hero-grid{
    display:grid;
    grid-template-columns:1.3fr 1fr;
    gap:60px;
    align-items:center;
}

.info-card{
    background:var(--card);
    padding:35px;
    border-radius:28px;
    box-shadow:var(--shadow);
}

.meta{
    display:flex;
    flex-wrap:wrap;
    gap:15px;
    margin-bottom:25px;
    color:#666;
}

.photo-wrapper{
    display:flex;
    flex-direction:column;
    gap:15px;
}

.photo{
    width:100%;
    aspect-ratio:1/1;
    border-radius:30px;
    overflow:hidden;
    box-shadow:var(--shadow);
}

.photo img{
    width:100%;
    height:100%;
    object-fit:cover;
}

.image-note{
    background:white;
    border-radius:18px;
    padding:18px;
    border:1px dashed #bdbdbd;
}

.card{
    background:var(--card);
    border-radius:25px;
    padding:30px;
    box-shadow:var(--shadow);
    transition:.35s;
}

.card:hover{
    transform:translateY(-8px);
}

.experience-grid{
    display:grid;
    gap:25px;
}

.projects-track{
    display:flex;
    gap:25px;
    overflow-x:auto;
    scroll-snap-type:x mandatory;
    padding-bottom:20px;
}

.projects-track::-webkit-scrollbar{
    height:8px;
}

.projects-track::-webkit-scrollbar-thumb{
    background:var(--accent);
    border-radius:100px;
}

.project-card{
    min-width:350px;
    background:white;
    border-radius:24px;
    overflow:hidden;
    cursor:pointer;
    box-shadow:var(--shadow);
    transition:.4s;
    scroll-snap-align:start;
}

.project-card:hover{
    transform:translateY(-10px) scale(1.02);
}

.project-image{
    height:240px;
    overflow:hidden;
}

.project-image img{
    width:100%;
    height:100%;
    object-fit:cover;
    transition:.5s;
}

.project-card:hover img{
    transform:scale(1.08);
}

.project-content{
    padding:20px;
}

.case-description{
    margin-top:40px;
    background:white;
    padding:35px;
    border-radius:25px;
    box-shadow:var(--shadow);
    min-height:250px;
    opacity:0;
    transform:translateY(20px);
    transition:.4s;
}

.case-description.active{
    opacity:1;
    transform:translateY(0);
}

.case-title{
    color:var(--accent);
    margin-bottom:10px;
}

.contact-card{
    background:white;
    border-radius:30px;
    padding:40px;
    box-shadow:var(--shadow);
}

.fade{
    opacity:0;
    transform:translateY(40px);
    transition:1s;
}

.fade.show{
    opacity:1;
    transform:translateY(0);
}

footer{
    text-align:center;
    padding:40px;
    color:#666;
}

@media (max-width:900px){

.hero-grid{
    grid-template-columns:1fr;
}

.project-card{
    min-width:280px;
}

.nav{
    width:90%;
}

.nav ul{
    justify-content:center;
    flex-wrap:wrap;
}
}
</style>
</head>
<body>

<nav class="nav">
    <ul>
        <li><a href="#about">Обо мне</a></li>
        <li><a href="#experience">Опыт</a></li>
        <li><a href="#cases">Кейсы</a></li>
        <li><a href="#contacts">Контакты</a></li>
    </ul>
</nav>

<!-- ОБО МНЕ -->

<section id="about" class="hero">
    <div class="container hero-grid fade">

        <div class="info-card">

            <h1>Андриянова Екатерина</h1>

            <div class="meta">
                <span>Графический и продуктовый дизайнер</span>
                <span>•</span>
                <span>RUS / ENG (C1+)</span>
                <span>•</span>
                <span>Санкт-Петербург</span>
            </div>

            <div class="meta">
                <span>famm22@yandex.ru</span>
                <span>•</span>
                <span>@katt_an</span>
            </div>

            <h3>О себе</h3>

            <p>
                Я дизайнер с 1+ годом коммерческого опыта, фокусом на системное мышление и
                работу со сложными B2B-продуктами. Проектировала интерфейсы для вузов и
                инженерного ПО, а также создавала визуальные решения для игр. Умею
                выстраивать логику с нуля, проводить глубинные интервью и адаптировать
                интерфейс под реальные пользовательские сценарии.
            </p>

        </div>

        <div class="photo-wrapper">

            <div class="photo">

                <!-- ВСТАВЬТЕ ССЫЛКУ НА ВАШУ ФОТОГРАФИЮ -->
                <img src="https://via.placeholder.com/700x700"
                alt="Фото Екатерины">

            </div>

            <div class="image-note">
                <strong>Место для фотографии</strong><br><br>
                Замените ссылку внутри тега:
                <br><br>
                src="ВАША_ССЫЛКА_НА_ФОТО.jpg"
            </div>

        </div>

    </div>
</section>

<!-- ОПЫТ -->

<section id="experience">
    <div class="container fade">

        <h2>Опыт работы</h2>

        <div class="experience-grid">

            <div class="card">

                <h3>
                    [ЗАГОЛОВОК]
                </h3>

                <p>
                    <strong>[ПОДЗАГОЛОВОК]</strong>
                </p>

                <br>

                <p>
                    [ТЕКСТ ОПИСАНИЯ ОПЫТА РАБОТЫ]
                </p>

            </div>

            <div class="card">

                <h3>
                    [ЗАГОЛОВОК]
                </h3>

                <p>
                    <strong>[ПОДЗАГОЛОВОК]</strong>
                </p>

                <br>

                <p>
                    [ТЕКСТ ОПИСАНИЯ ОПЫТА РАБОТЫ]
                </p>

            </div>

        </div>

    </div>
</section>

<!-- КЕЙСЫ -->

<section id="cases">
    <div class="container fade">

        <h2>Кейсы</h2>

        <div class="projects-track">

            <div class="project-card"
                onclick="showCase(
                'ЗАГОЛОВОК КЕЙСА 1',
                'ПОДЗАГОЛОВОК КЕЙСА 1',
                'ТЕКСТ КЕЙСА 1'
                )">

                <div class="project-image">
                    <!-- ВСТАВЬТЕ ССЫЛКУ НА ИЗОБРАЖЕНИЕ -->
                    <img src="https://via.placeholder.com/800x500" alt="">
                </div>

                <div class="project-content">
                    <h3>Кейс 01</h3>
                    <p>Нажмите для просмотра описания</p>
                </div>

            </div>

            <div class="project-card"
                onclick="showCase(
                'ЗАГОЛОВОК КЕЙСА 2',
                'ПОДЗАГОЛОВОК КЕЙСА 2',
                'ТЕКСТ КЕЙСА 2'
                )">

                <div class="project-image">
                    <img src="https://via.placeholder.com/800x500" alt="">
                </div>

                <div class="project-content">
                    <h3>Кейс 02</h3>
                    <p>Нажмите для просмотра описания</p>
                </div>

            </div>

            <div class="project-card"
                onclick="showCase(
                'ЗАГОЛОВОК КЕЙСА 3',
                'ПОДЗАГОЛОВОК КЕЙСА 3',
                'ТЕКСТ КЕЙСА 3'
                )">

                <div class="project-image">
                    <img src="https://via.placeholder.com/800x500" alt="">
                </div>

                <div class="project-content">
                    <h3>Кейс 03</h3>
                    <p>Нажмите для просмотра описания</p>
                </div>

            </div>

            <div class="project-card"
                onclick="showCase(
                'ЗАГОЛОВОК КЕЙСА 4',
                'ПОДЗАГОЛОВОК КЕЙСА 4',
                'ТЕКСТ КЕЙСА 4'
                )">

                <div class="project-image">
                    <img src="https://via.placeholder.com/800x500" alt="">
                </div>

                <div class="project-content">
                    <h3>Кейс 04</h3>
                    <p>Нажмите для просмотра описания</p>
                </div>

            </div>

        </div>

        <div id="caseDescription" class="case-description">

            <h3 class="case-title">
                Выберите кейс
            </h3>

            <h4 id="caseSubtitle">
                Подзаголовок появится здесь
            </h4>

            <br>

            <p id="caseText">
                После нажатия на карточку кейса здесь появится подробное описание проекта.
            </p>

        </div>

    </div>
</section>

<!-- КОНТАКТЫ -->

<section id="contacts">
    <div class="container fade">

        <div class="contact-card">

            <h2>Контактная информация</h2>

            <p>
                [МЕСТО ДЛЯ ТЕКСТА]
            </p>

        </div>

    </div>
</section>

<footer>
    © 2025 Екатерина Андриянова
</footer>

<script>

function showCase(title, subtitle, text){

    const block = document.getElementById("caseDescription");

    block.querySelector(".case-title").textContent = title;
    document.getElementById("caseSubtitle").textContent = subtitle;
    document.getElementById("caseText").textContent = text;

    block.classList.add("active");
}

const observer = new IntersectionObserver(entries => {
    entries.forEach(entry => {
        if(entry.isIntersecting){
            entry.target.classList.add("show");
        }
    });
},{
    threshold:0.2
});

document.querySelectorAll(".fade").forEach(item=>{
    observer.observe(item);
});

</script>

</body>
</html>
