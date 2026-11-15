<!DOCTYPE html>
<html lang="en" data-theme="light">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Task 4 - Responsive Dashboard</title>
<link rel="stylesheet" href="style.css">
</head>
<body>
<header class="header">
  <div>
    <h1>Enterprise Dashboard</h1>
    <p>Task 4 - Responsive Design Tokens & Mobile-First CSS</p>
  </div>
  <button id="themeBtn" onclick="toggleTheme()">🌙 Dark Mode</button>
</header>

<main class="dashboard">
  <section class="card glass"><h3>👥 Total Users</h3><h2>12,480</h2><p>+12% this month</p></section>
  <section class="card glass"><h3>💰 Revenue</h3><h2>₹4,85,000</h2><p>+18% this month</p></section>
  <section class="card glass"><h3>📦 Orders</h3><h2>1,240</h2><p>+8% this week</p></section>
  <section class="card glass"><h3>⭐ Rating</h3><h2>4.8 / 5</h2><p>2,300 reviews</p></section>
  <section class="card wide glass"><h3>📊 Analytics</h3><p>Desktop lo idi pedda ga, mobile lo chinna ga kanipisthundi. Idi Responsive Grid.</p><div class="bar"><div class="fill" style="width:80%"></div></div><div class="bar"><div class="fill" style="width:60%"></div></div><div class="bar"><div class="fill" style="width:90%"></div></div></section>
  <section class="card glass"><h3>✅ Tasks</h3><p>Task 1 - Done</p><p>Task 2 - Done</p><p>Task 3 - Done</p></section>
</main>
<footer><p>Built with CSS Variables, Grid & Flexbox | 320px - 1440px Responsive</p></footer>

<script>
function toggleTheme(){
  const html = document.documentElement;
  const isDark = html.getAttribute('data-theme') === 'dark';
  html.setAttribute('data-theme', isDark ? 'light' : 'dark');
  document.getElementById('themeBtn').textContent = isDark ? '🌙 Dark Mode' : '☀️ Light Mode';
}
</script>
</body>
</html>
