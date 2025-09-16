<!DOCTYPE html>
<html>
<head>
  <style>
    .btn {
      background: lightgreen;
      padding: 10px;
      margin: 5px;
      border: none;
    }
    .active {
      background: darkgreen;
      color: white;
    }
  </style>
</head>
<body>
  <button class="btn" onclick="setActive(this)">Button 1</button>
  <button class="btn" onclick="setActive(this)">Button 2</button>

  <script>
    function setActive(clicked) {
      var all = document.getElementsByClassName("btn");
      for (var i = 0; i < all.length; i++) {
        all[i].classList.remove("active");
      }
      clicked.classList.add("active");
    }
  </script>
</body>
</html>
