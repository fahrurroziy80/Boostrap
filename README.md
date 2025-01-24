<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>NOX</title>
  <style>
    body {
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background: #000; /* Latar belakang hitam */
  overflow: hidden; /* Agar elemen tidak keluar layar */
}

.aura-container {
  position: relative;
  z-index: 1;
}

.text {
  font-size: 3rem;
  color: #fff;
  text-align: center;
  z-index: 2;
  position: relative;
}

.aura-bg {
  position: absolute;
  top: 50%;
  left: 50%;
  width: 500px;
  height: 500px;
  background: radial-gradient(circle, rgba(0, 255, 255, 0.2), transparent 60%);
  filter: blur(50px); /* Efek kabur untuk asap */
  transform: translate(-50%, -50%);
  animation: moveAura 8s infinite alternate;
  opacity: 0.7;
}

@keyframes moveAura {
  0% {
    transform: translate(-50%, -50%) scale(1);
  }
  50% {
    transform: translate(-52%, -48%) scale(1.2);
  }
  100% {
    transform: translate(-50%, -50%) scale(1);
  }
}


div {
  display: flex;
  justify-content: center; /* Memusatkan secara horizontal */
  align-items: center;    /* Memusatkan secara vertikal */
  height: 200px;          /* Contoh tinggi elemen */
}

h1 {
  text-shadow: 0px 0px 10px red,
                0px 0px 20px red,
                0px 0px 30px red,
                0px 0px 40px red,
                0px 0px 60px red;
  font-size: 50px;
}
.circle-image {
  width: 200px;           /* Ukuran lebar gambar */
  height: 200px;          /* Ukuran tinggi gambar */
  border-radius: 50%;     /* Membuat gambar berbentuk lingkaran */
  object-fit: cover;      /* Menyesuaikan konten gambar agar proporsional */
  border: 2px solid #333; /* Opsional: tambahkan border */
  filter: drop-shadow(2px 2px 20px rgb(255, 17, 0));
  
  
}


  </style>
</head>
<body>
  <div class="aura-container">
    <h1 class="text">Fahrurrozy</h1>
    <div class="aura-bg"></div>
  </div>
  <div class="image-container">
    <img src="asset/lala.jpg" alt="Contoh Gambar" class="circle-image">
  </div>
</body>
</html>
