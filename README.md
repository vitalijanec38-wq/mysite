<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Поездки в Варшаву</title>

<style>
body {
  margin: 0;
  font-family: Arial, sans-serif;
  color: white;
  background: linear-gradient(135deg,#0f2027,#203a43,#000);
}

/* главный экран */
.hero {
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

h1 {
  font-size: 40px;
  margin: 0;
}

p {
  opacity: 0.8;
}

/* кнопка */
.btn {
  margin-top: 20px;
  padding: 15px 30px;
  border-radius: 30px;
  background: linear-gradient(45deg,#2AABEE,#00c6ff);
  color: white;
  text-decoration: none;
  display: inline-block;
  transition: 0.3s;
}

.btn:hover {
  transform: scale(1.1);
}

/* секции */
.section {
  padding: 60px 20px;
  text-align: center;
}

/* карточки */
.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit,minmax(250px,1fr));
  gap: 20px;
  max-width: 900px;
  margin: auto;
}

.card {
  background: rgba(255,255,255,0.05);
  padding: 20px;
  border-radius: 20px;
  transition: 0.3s;
}

.card:hover {
  transform: translateY(-8px);
}
</style>
</head>

<body>

<div class="hero">
  <div>
    <h1>Поездки в Варшаву</h1>
    <p>Клайпеда → Варшава → обратно</p>
    <a href="#" class="btn">Написать в Telegram</a>
  </div>
</div>

<div class="section">
  <h2>Ближайшие поездки</h2>
  <div class="grid">
    <div class="card">Вторник — Клайпеда → Варшава</div>
    <div class="card">Пятница — Варшава → Клайпеда</div>
  </div>
</div>

<div class="section">
  <h2>Почему выбирают нас</h2>
  <div class="grid">
    <div class="card">⚡ Быстро</div>
    <div class="card">🚗 Комфорт</div>
    <div class="card">📄 Помощь</div>
  </div>
</div>

<div class="section">
  <h2>Контакты</h2>
  <p>📞 +370 619 10045</p>
</div>

</body>
</html>
