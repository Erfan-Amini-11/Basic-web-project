<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <style>
      .box {
        height: 150px;
        width: 100px;
        margin: auto;
        background-color: chartreuse;
      }
      .key {
        height: 150px;
        width: 100px;
        margin: auto;
        background-color: skyblue;
      }
      .btn {
        width: 4rem;
        height: 3rem;
        margin: auto;
      }
    </style>
  </head>
  <body>
    <button class="btn">Click Me</button>
    <div class="box"></div>
    <script>
      const btn = document.querySelector('.btn');
      const box = document.querySelector('.box');

      btn.addEventListener('click', function () {
        if (box.classList.contains('box')) {
          box.classList.add('key');
        }
        if (box.classList.contains('key')) {
          box.classList.remove('key');
        }
      });
    </script>
  </body>
</html>
