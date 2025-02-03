<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Will You Be My Valentine?</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      background-color: pink;
      padding-top: 100px;
    }

    h1 {
      font-size: 2em;
      color: red;
    }

    .btn-container {
      margin-top: 20px;
    }

    .btn {
      font-size: 20px;
      padding: 10px 20px;
      margin: 10px;
      cursor: pointer;
      border: none;
      border-radius: 10px;
    }

    .yes {
      background-color: green;
      color: white;
    }

    .no {
      background-color: red;
      color: white;
    }
  </style>
</head>

<body>

  <h1>Will you be my Valentine? 💖</h1>

  <div class="btn-container">
    <button class="btn yes" id="yesBtn">Yes</button>
    <button class="btn no" id="noBtn">No</button>
  </div>

  <script>
    let yesButton = document.getElementById("yesBtn");
    let noButton = document.getElementById("noBtn");
    let sizeMultiplier = 1; // Initial multiplier
    noButton.addEventListener("click", function() {
      if (sizeMultiplier < 4) { // Limit the growth to 4 times
        sizeMultiplier++;
        yesButton.style.fontSize = (20 * sizeMultiplier) + "px"; // Increase font size
        yesButton.style.padding = (10 * sizeMultiplier) + "px " + (20 * sizeMultiplier) + "px"; // Increase button padding
      } else {
        alert("Yes lang pwde boss! 😆💘");
      }
    });
    yesButton.addEventListener("click", function() {
      alert("Yay! 💖 tankina mo! 😊");
    });
  </script>

</body>

</html>
