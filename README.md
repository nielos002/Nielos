Nielosip
<!DOCTYPE html><html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>NielOS 14</title>
  <style>
    body {
      margin: 0;
      background: url('https://images.unsplash.com/photo-1606788075761-5b8b721b9c13?auto=format&fit=crop&w=800&q=80') no-repeat center center fixed;
      background-size: cover;
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
      overflow: hidden;
    }
    .lockscreen {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      height: 100vh;
      color: white;
      text-shadow: 0 0 10px rgba(0,0,0,0.6);
    }
    .time {
      font-size: 64px;
      font-weight: 600;
    }
    .date {
      font-size: 18px;
      margin-bottom: 40px;
    }
    .unlock {
      font-size: 14px;
      opacity: 0.7;
    }
    .home {
      display: none;
      flex-direction: column;
      justify-content: space-between;
      align-items: center;
      padding: 20px 0;
      height: 100vh;
      background-color: rgba(255,255,255,0.1);
      backdrop-filter: blur(10px);
    }
    .icons {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 20px;
      padding: 20px;
    }
    .icon {
      display: flex;
      flex-direction: column;
      align-items: center;
      color: white;
      font-size: 12px;
      text-align: center;
    }
    .icon img {
      width: 60px;
      height: 60px;
      border-radius: 14px;
      margin-bottom: 5px;
    }
    .dock {
      display: flex;
      gap: 30px;
      background: rgba(255,255,255,0.2);
      padding: 10px 20px;
      border-radius: 30px;
    }
  </style>
</head>
<body>
  <div class="lockscreen" id="lockscreen">
    <div class="time" id="time"></div>
    <div class="date" id="date"></div>
    <div class="unlock">Deslize para desbloquear</div>
  </div>  <div class="home" id="home">
    <div class="icons">
      <div class="icon"><img src="https://img.icons8.com/ios-filled/100/ffffff/safari.png"/><div>Safari</div></div>
      <div class="icon"><img src="https://img.icons8.com/ios-filled/100/ffffff/youtube-play.png"/><div>YouTube</div></div>
