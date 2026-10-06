# Happy-teachers-day-
Happy teachers day ma'am lj
confetti.style.backgroundColor
I'll add smooth, warm animations to this existing Teachers' Day greeting, matching the style of popular public GitHub tribute projects. This updated version includes fade-in effects, floating text, confetti, and subtle hover interactions:
<!DOCTYPE html>
<html>
<head>
  <title>Happy Teachers' Day</title>
  <style>
  {
 margin: 0;
 padding: 0;
 box-sizing: border-box;
 }
 body { 
 background: #fef3c7; 
 text-align: center; 
 font-family: 'Segoe UI', Arial, sans-serif; 
 padding-top: 120;
 min-height: 100;
 position: relative;
 overflow-x: hidden;
 }
 / Animated floating confetti background /
 .confetti {
 position: fixed;
 width: 10;
 height: 10;
 top: -10;
 animation: fall linear infinite;
 z-index: 1;
 }
 h1 { 
 color: #b45309; 
 font-size: 48;
 opacity: 0;
 transform: (30);
 animation: fadeInUp 1 ease forwards 0.5;
 margin-bottom: 30;
 position: relative;
 z-index: 2;
 }
 p { 
 font-size: 22; 
 color: #78350f; 
 max-width: 600; 
 margin: 20 auto;
 line-height: 1.6;
 opacity: 0;
 transform: (20);
 animation: fadeInUp 1 ease forwards 1.2;
 position: relative;
 z-index: 2;
 }
 / Floating subtle animation for the whole card /
 .greeting-card {
 animation: float 4 ease-in-out infinite;
 position: relative;
 z-index: 2;
 }
 / Animation keyframes /
  {
  {
 opacity: 1;
 transform: (0);
 }
 }
 @ {
 0, 100 { transform: (0); }
 50 { transform: (-10); }
 }
 @ {
  {
 transform: (105) (360);
 }
 }
 / Hover effect on the heading /
 h1:hover {
 transform: (1.05);
 transition: transform 0.3 ease;
 text-shadow: 2 2 8 (180, 83, 9, 0.2);
 }
  </style>
</head>
<body>
  <div class="greeting-card">
 <h1>Happy Teachers' Day! 🎉</h1>
 <p>Thank you for every lesson, every encouragement, and every moment you helped us grow.</p>
 <p style="margin-top: 40; font-style: italic; opacity: 0; animation: fadeInUp 1 ease forwards 1.8;">You make learning feel like an adventure, not just work 💛</p>
  </div>

  <!-- Auto generate confetti with JS -->
  <script>
  confettiColors = ['#b45309', '#f59e0b', '#ef4444', '#10b981', '#3b82f6'];
 confettiCount = 50;

 (l i = 0; i < confettiCount; i++) {
 document.createElement('div');
 confetti.classList.add('confetti');
 confetti.style.left = Math.random()  100 + 'vw';
 confetti.style.backgroundColor = confettiColors[Math.floor(Math.random()  confettiColors.length)];
 confetti.style.animationDuration = (Math.random()  3 + 2) + 's';
 confetti.style.animationDelay = Math.random()  5 + 's';
 confetti.style.width = (Math.random()  8 + 6) + 'px';
 confetti.style.height = 
