<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>❤️ For You</title>
<style>
  body {
    text-align: center;
    font-family: Arial;
    background: linear-gradient(135deg, #ff758c, #ff7eb3);
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    color: white;
  }
  .heart {
    font-size: 50px;
    margin-bottom: 20px;
    animation: beat 1s infinite;
  }
  @keyframes beat {
    0%, 100% { transform: scale(1); }
    50% { transform: scale(1.2); }
  }
  input {
    padding: 10px;
    width: 80%;
    border: none;
    border-radius: 10px;
    margin-top: 10px;
  }
  button {
    margin-top: 15px;
    padding: 10px 20px;
    border: none;
    border-radius: 20px;
    background: white;
    color: #ff4f7b;
    font-weight: bold;
    cursor: pointer;
  }
</style>
</head>
<body>

<div class="heart">❤️</div>
<h1>I Love You</h1>
<p>ادخل كلمة السر</p>
<input type="password" id="password" placeholder="كلمة السر">
<br>
<button onclick="check()">دخول</button>
<p id="msg"></p>

<script>
function check() {
  const pass = document.getElementById("password").value;
  if(pass === "1234") {
    window.location.href = "love.html"; // هذا الاسم يجب أن يكون بالضبط نفس الملف التالي
  } else {
    document.getElementById("msg").innerText = "كلمة السر غلط 💔";
  }
}
</script>

</body>
</html>
