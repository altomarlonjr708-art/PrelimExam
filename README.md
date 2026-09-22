# PrelimExam
<!DOCTYPE html>
<html>
<head>
  <title>Login</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background: #f2f2f2;
    }

    .login {
      background: white;
      padding: 30px;
      border-radius: 10px;
      width: 300px;
      box-shadow: 0 4px 12px #ccc;
    }

    input, button {
      width: 100%;
      padding: 10px;
      margin: 8px 0;
      box-sizing: border-box;
    }

    button {
      background: #007bff;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
  </style>
</head>

<body>
  <div class="login">
    <h2>Login</h2>

    <input type="text" id="username" placeholder="Username">
    <input type="password" id="password" placeholder="Password">

    <button onclick="login()">Log In</button>

    <p id="message"></p>
  </div>

  <script>
    function login() {
      const username = document.getElementById("username").value;
      const password = document.getElementById("password").value;

      if (username === "admin" && password === "1234") {
        document.getElementById("message").textContent = "Login successful!";
      } else {
        document.getElementById("message").textContent = "Invalid username or password.";
      }
    }
  </script>
</body>
</html>
