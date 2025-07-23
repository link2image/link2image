## Hi there 



<!DOCTYPE html>
<html lang="bn">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>শর্ট লিঙ্ক জেনারেটর</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      padding: 30px;
      background: #f5f5f5;
    }
    h1 {
      color: #333;
    }
    input, button {
      padding: 10px;
      font-size: 16px;
      width: 80%;
      max-width: 400px;
      margin: 10px 0;
    }
    #output a {
      display: block;
      margin-top: 15px;
      color: green;
      font-weight: bold;
    }
  </style>

  <!-- 🔥 এখানে Adsterra বা PropellerAds স্ক্রিপ্ট বসাও -->
  <!-- উদাহরণ Adsterra Popunder Script -->
  <!--
  <script type='text/javascript' src='https://www.youradsterrascript.com/script.js'></script>
  -->
</head>
<body>
  <h1>🔗 শর্ট লিঙ্ক জেনারেটর</h1>
  <input type="text" id="longUrl" placeholder="তোমার URL লিখো">
  <br>
  <button onclick="shorten()">লিঙ্ক শর্ট করো</button>
  <p id="output"></p>

  <script>
    function shorten() {
      const longUrl = document.getElementById("longUrl").value.trim();
      if (!longUrl) {
        alert("দয়া করে একটি URL দিন");
        return;
      }
      const encoded = btoa(longUrl);
      const shortUrl = window.location.origin + window.location.pathname + "?go=" + encoded;
      document.getElementById("output").innerHTML = `<a href="${shortUrl}" target="_blank">${shortUrl}</a>`;
    }

    // Redirect if short URL is accessed
    window.onload = () => {
      const urlParam = new URLSearchParams(window.location.search).get("go");
      if (urlParam) {
        const decoded = atob(urlParam);
        // Redirect with delay (e.g., to show ad or loading)
        setTimeout(() => {
          window.location.href = decoded;
        }, 3000); // 3 second delay
      }
    };
  </script>
</body>
</html><!DOCTYPE html>
<html lang="bn">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>শর্ট লিঙ্ক জেনারেটর</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      padding: 30px;
      background: #f5f5f5;
    }
    h1 {
      color: #333;
    }
    input, button {
      padding: 10px;
      font-size: 16px;
      width: 80%;
      max-width: 400px;
      margin: 10px 0;
    }
    #output a {
      display: block;
      margin-top: 15px;
      color: green;
      font-weight: bold;
    }
  </style>

  <!-- 🔥 এখানে Adsterra বা PropellerAds স্ক্রিপ্ট বসাও -->
  <!-- উদাহরণ Adsterra Popunder Script -->
  <!--
  <script type='text/javascript' src='https://www.youradsterrascript.com/script.js'></script>
  -->
</head>
<body>
  <h1>🔗 শর্ট লিঙ্ক জেনারেটর</h1>
  <input type="text" id="longUrl" placeholder="তোমার URL লিখো">
  <br>
  <button onclick="shorten()">লিঙ্ক শর্ট করো</button>
  <p id="output"></p>

  <script>
    function shorten() {
      const longUrl = document.getElementById("longUrl").value.trim();
      if (!longUrl) {
        alert("দয়া করে একটি URL দিন");
        return;
      }
      const encoded = btoa(longUrl);
      const shortUrl = window.location.origin + window.location.pathname + "?go=" + encoded;
      document.getElementById("output").innerHTML = `<a href="${shortUrl}" target="_blank">${shortUrl}</a>`;
    }

    // Redirect if short URL is accessed
    window.onload = () => {
      const urlParam = new URLSearchParams(window.location.search).get("go");
      if (urlParam) {
        const decoded = atob(urlParam);
        // Redirect with delay (e.g., to show ad or loading)
        setTimeout(() => {
          window.location.href = decoded;
        }, 3000); // 3 second delay
      }
    };
  </script>
</body>
</html>
