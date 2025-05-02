<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1" />
  <title>Happy Birthday Alin!</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Pacifico&family=Quicksand:wght@400;700&display=swap');

    /* Reset */
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: 'Quicksand', sans-serif;
      background: linear-gradient(135deg, #fceabb, #f8b500);
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 1rem;
      overflow: hidden;
    }

    .container {
      background: rgba(255, 255, 255, 0.85);
      border-radius: 20px;
      box-shadow: 0 10px 25px rgba(0,0,0,0.15);
      max-width: 420px;
      padding: 2rem;
      text-align: center;
      position: relative;
    }

    h1 {
      font-family: 'Pacifico', cursive;
      font-size: 3rem;
      color: #e75480;
      margin-bottom: 1rem;
      user-select: none;
      text-shadow: 2px 2px 5px rgba(231, 84, 128, 0.6);
    }

    h2 {
      color: #f67280;
      font-weight: 700;
      margin-bottom: 1.5rem;
    }

    p {
      font-size: 1.2rem;
      color: #555;
      margin-bottom: 1.25rem;
      line-height: 1.5;
      user-select: text;
    }

    .hearts-container {
      position: absolute;
      top: -20px;
      right: -20px;
      width: 100px;
      height: 100px;
      pointer-events: none;
    }

    .heart {
      position: absolute;
      width: 20px;
      height: 18px;
      background-color: #e75480;
      transform: rotate(-45deg);
      animation: floatUp 6s linear infinite;
      opacity: 0.8;
      border-radius: 20px 20px 0 0;
    }
    .heart::before,
    .heart::after {
      content: "";
      position: absolute;
      width: 20px;
      height: 18px;
      background-color: #e75480;
      border-radius: 50%;
      top: 0;
      left: 0;
    }
    .heart::before {
      left: 10px;
    }
    .heart::after {
      top: -9px;
      left: 5px;
    }

    @keyframes floatUp {
      0% {
        transform: translateY(0) rotate(-45deg);
        opacity: 0.8;
      }
      50% {
        opacity: 1;
      }
      100% {
        transform: translateY(-120px) rotate(-45deg);
        opacity: 0;
      }
    }

    /* Decoration hearts randomly placed */
    .heart:nth-child(1) {
      left: 10px;
      animation-delay: 0s;
      animation-duration: 5s;
    }
    .heart:nth-child(2) {
      left: 50px;
      animation-delay: 1.5s;
      animation-duration: 6.5s;
      width: 25px;
      height: 23px;
    }
    .heart:nth-child(3) {
      left: 80px;
      animation-delay: 3s;
      animation-duration: 7s;
    }
    .heart:nth-child(4) {
      left: 30px;
      animation-delay: 2s;
      animation-duration: 5.5s;
      width: 15px;
      height: 13px;
    }
    .heart:nth-child(5) {
      left: 70px;
      animation-delay: 4s;
      animation-duration: 6s;
      width: 18px;
      height: 15px;
    }

    .flower {
      position: absolute;
      bottom: 10px;
      left: 10px;
      width: 60px;
      height: 60px;
      background: radial-gradient(circle at 30% 30%, #ff6f91, #ff9671);
      border-radius: 50%;
      box-shadow:
       20px 0 #f9f871,
       -20px 0 #f9f871,
       0 20px #f9f871,
       0 -20px #f9f871,
       14px 14px #f9f871,
       -14px 14px #f9f871,
       14px -14px #f9f871,
       -14px -14px #f9f871;
      animation: flowerRotate 10s linear infinite;
      opacity: 0.8;
      pointer-events: none;
    }
    @keyframes flowerRotate {
      from {
        transform: rotate(0deg);
      }
      to {
        transform: rotate(360deg);
      }
    }

    @media (max-width: 480px) {
      .container {
        max-width: 95vw;
        padding: 1.5rem 1rem;
      }
      h1 {
        font-size: 2.5rem;
      }
      p {
        font-size: 1rem;
      }
    }
  </style>
</head>
<body>
  <div class="container" role="main" aria-label="Birthday message to Alin">
    <h1>Happy Birthday, Alin! 🎉</h1>
    <h2>For my Best Friend</h2>
    <p>Dearest Alin,</p>
    <p>On your special day, I want you to know how much you mean to me. You bring so much joy, laughter, and light into my life. May your birthday be filled with all the sweetness, love, and happiness you deserve.</p>
    <p>Thank you for being such an amazing friend — my confidant, my cheerleader, and my joy. Here's to many more beautiful memories together!</p>
    <p>With all my love, <br><strong>Your Best Friend</strong></p>
    <div class="hearts-container" aria-hidden="true">
      <div class="heart"></div>
      <div class="heart"></div>
      <div class="heart"></div>
      <div class="heart"></div>
      <div class="heart"></div>
    </div>
    <div class="flower" aria-hidden="true"></div>
  </div>
</body>
</html>
