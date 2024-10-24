<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>爱心表白</title>
<style>
  /* 爱心动画 */
  @keyframes heartbeat {
    0% { transform: scale(1); }
    25% { transform: scale(1.1); }
    50% { transform: scale(1); }
    75% { transform: scale(0.9); }
    100% { transform: scale(1); }
  }

  /* 爱心样式 */
  .heart {
    position: relative;
    width: 100px;
    height: 90px;
    margin: 50px auto;
    animation: heartbeat 1s infinite;
  }

  .heart::before,
  .heart::after {
    position: absolute;
    content: "";
    top: 40px;
    width: 52px;
    height: 80px;
    border-radius: 50px 50px 0 0;
    background: red;
  }

  .heart::before {
    left: 50px;
    transform: rotate(-45deg);
    transform-origin: 0 100%;
  }

  .heart::after {
    left: 0;
    transform: rotate(45deg);
    transform-origin: 100% 100%;
  }

  /* 表白文字样式 */
  .confession {
    text-align: center;
    font-size: 20px;
    font-weight: bold;
    color: #333;
    margin-top: 20px;
  }
</style>
</head>
<body>
  <div class="heart"></div>
  <div class="confession">
    亲爱的，我爱你！❤️
  </div>
</body>
</html>
