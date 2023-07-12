# light-on-and-off
how to make function of on and off with images
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <style>
    * {
        text-align: center;
        justify-content: center;
        box-sizing: border-box;
    }
    .img {
        margin-top: 130px;
    }
    .container {
        box-shadow: 0px 0px 5px 1px rgba(0,0,0,1);
        width: 23%;
        align-items: center;
        margin-top: 8%;
        margin-left: 35%;
    }
    .btn {
        margin-top: 4%;
        padding: 8px 8px 8px 8px;
        font-size: medium;
        color: white;
        border: 1.50px solid black;
        border-radius: 7px;
        background-color:olivedrab;
        font-weight: 550;
        cursor: pointer;
    }
  </style>
  <body>
    <script>
      function light(sw) {
        let pic;
        if (sw == 1) {
          pic = "on2.gif";
        } else {
          pic = "off.gif";
        }
        document.getElementById("image").src = pic;
    }
    </script>
    <div class="container">
    <img
     class="img"
      id="image"
      src="off.gif"
      width="95px"
      height="160px"
    /><br />
    <button class="btn" onclick="light(1)">Switch On</button>
    <button class="btn" onclick="light(2)">Switch Off</button>
</div>
  </body>
</html>

