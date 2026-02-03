# valentine
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Important Question 😳</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(135deg, #ff758c, #ff7eb3);
      font-family: 'Arial', sans-serif;
    }

    button {
      padding: 20px 40px;
      font-size: 22px;
      border: none;
      border-radius: 12px;
      cursor: pointer;
      background: #fff;
      color: #ff4d6d;
      font-weight: bold;
      box-shadow: 0 10px 25px rgba(0,0,0,0.2);
      transition: transform 0.2s;
    }

    button:hover {
      transform: scale(1.05);
    }

    .popup {
      position: fixed;
      inset: 0;
      background: rgba(0,0,0,0.5);
      display: none;
      justify-content: center;
      align-items: center;
    }

    .card {
      background: white;
      padding: 30px;
      border-radius: 16px;
      text-align: center;
      width: 300px;
    }

    .card h2 {
      color: #ff4d6d;
    }

    .choices {
      margin-top: 20px;
      display: flex;
      justify-content: space-around;
    }

    .yes {
      background: #ff4d6d;
      color: white;
    }

    .no {
      background: #ddd;
      position: relative;
    }
  </style>
</head>
<body>

<button onclick="openPopup()">click me mommy</button>

<div class="popup" id="popup">
  <div class="card">
    <h2>Will you be my Valentine? 💖</h2>
    <p>(You legally can’t say no)</p>
    <div class="choices">
      <button class="yes" onclick="yes()">YES 😍</button>
      <button class="no" onmouseover="run(this)">NO 🙄</button>
    </div>
  </div>
</div>

<script>
  function openPopup() {
    document.getElementById('popup').style.display = 'flex';
  }

  function run(btn) {
    btn.style.position = "absolute";
    btn.style.top = Math.random() * 200 + "px";
    btn.style.left = Math.random() * 200 + "px";
  }

  function yes() {
    alert("YAYYYY 💕 See you on Valentine’s 😘");
  }
</script>

</body>
</html>
