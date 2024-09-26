<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>AI Song Lyrics Generator</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f4f4f4;
      margin: 0;
      padding: 0;
    }

    .container {
      max-width: 800px;
      margin: 50px auto;
      background-color: #fff;
      padding: 20px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      border-radius: 8px;
    }

    h1 {
      text-align: center;
      color: #333;
    }

    .form-group {
      margin-bottom: 15px;
    }

    label {
      display: block;
      margin-bottom: 5px;
      color: #333;
    }

    input[type="text"] {
      width: 100%;
      padding: 10px;
      border-radius: 4px;
      border: 1px solid #ddd;
    }

    button {
      display: block;
      width: 100%;
      padding: 10px;
      background-color: #28a745;
      color: #fff;
      border: none;
      border-radius: 4px;
      cursor: pointer;
      font-size: 16px;
    }

    button:hover {
      background-color: #218838;
    }

    #output {
      margin-top: 20px;
      padding: 10px;
      background-color: #f1f1f1;
      border-radius: 4px;
      min-height: 100px;
    }
  </style>
</head>
<body>

<div class="container">
  <h1>AI Song Lyrics Generator</h1>

  <div class="form-group">
    <label for="theme">Enter Song Theme:</label>
    <input type="text" id="theme" placeholder="e.g., Love, Sadness, Anger">
  </div>

  <button id="generateBtn">Generate Song Lyrics</button>

  <div id="output">
    <p>Generated lyrics will appear here...</p>
  </div>
</div>

<script>
  document.getElementById('generateBtn').addEventListener('click', function() {
    const theme = document.getElementById('theme').value;

    // Mock AI lyric generation for the frontend
    // In a real-world app, you would call an API (e.g., OpenAI API) to generate the lyrics.
    let lyrics = "Here are some AI-generated lyrics based on the theme: " + theme + "\n";
    lyrics += "\nChorus:\nLife is tough, but we keep moving\nLove is rough, but we're still grooving\n";

    document.getElementById('output').innerText = lyrics;
  });
</script>

</body>
</html>
