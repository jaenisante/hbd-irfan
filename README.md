# hbd-irfan
ILY
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Happy Birthday Irfan</title>
  <style>
    body {
      background-color: black;
      color: #ff69b4;
      font-family: monospace;
      white-space: pre;
      text-align: center;
      padding-top: 30px;
    }
    #heart {
      margin-top: 20px;
      font-size: 14px;
    }
  </style>
</head>
<body>
  <h2>HAPPY BIRTHDAY IRFAN</h2>
  <h3>I LOVE YOU ALWAYS</h3>
  <div id="heart"></div>

  <script>
    const heartLines = [
        "        ********       ********    ",
        "      ***********************      ",
        "    ***************************    ",
        "   *****************************   ",
        "  *******************************  ",
        " ********************************* ",
        " ********************************* ",
        " ********************************* ",
        " ********************************* ",
        "  *******************************  ",
        "  *******************************  ",
        "   *****************************   ",
        "    ***************************    ",
        "     *************************     ",
        "      ***********************      ",
        "       *********************       ",
        "         *****************         ",
        "           *************           ",
        "             *********             ",
        "               *****               ",
        "                ***                ",
        "                 *                 "
    ];

    const heartDiv = document.getElementById("heart");

    let index = 0;
    function drawHeart() {
      if (index <= heartLines.length) {
        heartDiv.innerText = heartLines.slice(0, index).join("\n");
        index++;
        setTimeout(drawHeart, 100);
      } else {
        setTimeout(() => {
          index = 0;
          drawHeart();
        }, 1000);
      }
    }

    drawHeart();
  </script>
</body>
</html>
