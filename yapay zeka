<!DOCTYPE html>
<html lang="tr">
<head>
<meta charset="UTF-8">
<title>Yapay Zeka Beyni Animasyonu</title>
<style>
body {
  margin: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background: #000;
  overflow: hidden;
}

.beyin {
  position: relative;
  width: 400px;
  height: 400px;
  border-radius: 50%;
  background: radial-gradient(circle at center, #111 0%, #000 80%);
  box-shadow: 0 0 60px #0ff inset;
}

.norons {
  position: absolute;
  width: 4px;
  height: 4px;
  background: #0ff;
  border-radius: 50%;
  animation: akis 3s linear infinite;
}

@keyframes akis {
  0% { transform: translate(0,0) scale(0.5); opacity: 1; }
  50% { transform: translate(calc(var(--x) * 1px), calc(var(--y) * 1px)) scale(1.5); opacity: 0.7; }
  100% { transform: translate(calc(var(--x) * 2px), calc(var(--y) * 2px)) scale(0.5); opacity: 0; }
}
</style>
</head>
<body>

<div class="beyin" id="beyin"></div>

<script>
// 200 tane "nöron" ekleyelim
const beyin = document.getElementById('beyin');
for(let i=0;i<200;i++){
  const noron = document.createElement('div');
  noron.classList.add('norons');
  // rastgele x ve y değerleri
  noron.style.setProperty('--x', Math.random()*400 - 200);
  noron.style.setProperty('--y', Math.random()*400 - 200);
  // rastgele animasyon gecikmesi
  noron.style.animationDelay = `${Math.random()*3}s`;
  beyin.appendChild(noron);
}
</script>

</body>
</html>
