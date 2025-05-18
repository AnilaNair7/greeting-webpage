<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Greeting</title>
  <style>
    body {
      background-color: #e0f7fa;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      flex-direction: column;
      font-family: Arial, sans-serif;
    }
    .message {
      font-size: 2rem;
      color: #00796b;
    }
  </style>
</head>
<body>

  <div class="message" id="greetingMessage"></div>

  <script>
    function getGreeting() {
      const hour = new Date().getHours();
      if (hour >= 6 && hour < 18) {
        return "Good Morning! ☀️";
      } else {
        return "Good Night! 🌙";
      }
    }

    document.getElementById("greetingMessage").innerText = getGreeting();
  </script>

</body>
</html>
