<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Noto Sans', Helvetica, Arial, sans-serif;
      background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      padding: 20px;
    }

    .profile-card {
      background: rgba(255, 255, 255, 0.95);
      border-radius: 24px;
      padding: 40px;
      max-width: 500px;
      box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
      text-align: center;
      backdrop-filter: blur(10px);
      border: 1px solid rgba(255, 255, 255, 0.2);
    }

    .avatar-container {
      margin-bottom: 30px;
      position: relative;
      display: inline-block;
      padding: 8px;
      background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
      border-radius: 16px;
      box-shadow: 0 8px 25px rgba(102, 126, 234, 0.4);
    }

    .avatar {
      border-radius: 12px;
      width: 300px;
      height: 150px;
      object-fit: cover;
      display: block;
      background: white;
    }

    .links-container {
      display: flex;
      flex-wrap: wrap;
      gap: 12px;
      justify-content: center;
      margin-top: 25px;
    }

    .social-link {
      text-decoration: none;
      color: white;
      background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
      padding: 12px 24px;
      border-radius: 12px;
      font-weight: 600;
      font-size: 14px;
      transition: all 0.3s ease;
      box-shadow: 0 4px 15px rgba(102, 126, 234, 0.4);
      position: relative;
      overflow: hidden;
      display: inline-flex;
      align-items: center;
      gap: 8px;
    }

    .social-link i {
      font-size: 16px;
    }

    .social-link::before {
      content: '';
      position: absolute;
      top: 0;
      left: -100%;
      width: 100%;
      height: 100%;
      background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.3), transparent);
      transition: left 0.5s ease;
    }

    .social-link:hover::before {
      left: 100%;
    }

    .social-link:hover {
      transform: translateY(-3px);
      box-shadow: 0 6px 20px rgba(102, 126, 234, 0.6);
    }

    .social-link:active {
      transform: translateY(-1px);
    }

    .divider {
      height: 2px;
      background: linear-gradient(90deg, transparent, #667eea, transparent);
      margin: 25px 0;
      border-radius: 2px;
    }

    @media (max-width: 600px) {
      .profile-card {
        padding: 30px 20px;
      }

      .avatar {
        width: 250px;
        height: 125px;
      }

      .social-link {
        font-size: 13px;
        padding: 10px 18px;
      }
    }
  </style>
</head>
<body>
  <div class="profile-card">
    <div class="avatar-container">
      <img class="avatar" src="https://media.tenor.com/atsrEuZxjdMAAAAM/orange-juice-drinking.gif" alt="Profile Animation">
    </div>

    <div class="divider"></div>

    <div class="links-container">
      <a href="https://steamcommunity.com/id/Saveqn/" class="social-link">
        <i class="fab fa-steam"></i> Steam
      </a>
      <a href="https://discordapp.com/users/753276264961278002/" class="social-link">
        <i class="fab fa-discord"></i> Discord
      </a>
      <a href="https://t.me/saveqn" class="social-link">
        <i class="fab fa-telegram"></i> Telegram
      </a>
      <a href="https://www.tiktok.com/@saveqqn" class="social-link">
        <i class="fab fa-tiktok"></i> TikTok
      </a>
      <a href="https://github.com/Saveqn/cs2cfg" class="social-link">
        <i class="fas fa-cog"></i> CS2 Config
      </a>
    </div>
  </div>
</body>
</html>
