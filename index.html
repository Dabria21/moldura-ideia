<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Câmera com Moldura</title>
  <style>
    body {
      margin: 0;
      overflow: hidden;
      text-align: center;
      background-color: #000;
    }

    #container {
      position: relative;
      display: inline-block;
    }

    video, canvas {
      width: 100vw;
      height: 100vh;
      object-fit: cover;
    }

    #moldura {
      position: absolute;
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      pointer-events: none;
    }

    #botao {
      position: fixed;
      bottom: 20px;
      left: 50%;
      transform: translateX(-50%);
      padding: 10px 20px;
      font-size: 18px;
      z-index: 10;
    }
  </style>
</head>
<body>
  <div id="container">
    <video id="video" autoplay playsinline></video>
    <img id="moldura" src="moldura.png" alt="Moldura" />
  </div>
  <button id="botao">Tirar Foto</button>
  <canvas id="canvas" style="display: none;"></canvas>

  <script>
    const video = document.getElementById('video');
    const canvas = document.getElementById('canvas');
    const botao = document.getElementById('botao');
    const moldura = document.getElementById('moldura');

    // Ativar câmera
    navigator.mediaDevices.getUserMedia({ video: true }).then(stream => {
      video.srcObject = stream;
    });

    botao.addEventListener('click', () => {
      const context = canvas.getContext('2d');
      canvas.width = video.videoWidth;
      canvas.height = video.videoHeight;

      // Desenha a câmera
      context.drawImage(video, 0, 0, canvas.width, canvas.height);

      // Desenha a moldura por cima
      const img = new Image();
      img.src = moldura.src;
      img.onload = () => {
        context.drawImage(img, 0, 0, canvas.width, canvas.height);
        const link = document.createElement('a');
        link.download = 'foto-com-moldura.png';
        link.href = canvas.toDataURL('image/png');
        link.click();
      };
    });
  </script>
</body>
</html>
