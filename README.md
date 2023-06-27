# Html-calculator-<!DOCTYPE html>
<html>
<head>
  <title>Calculator</title>
  <style>
    .calculator {
      width: 200px;
      border: 1px solid #ccc;
      padding: 10px;
    }

    .calculator input[type="button"] {
      width: 48px;
      height: 48px;
    }

    .calculator input[type="text"] {
      width: 100%;
      margin-bottom: 10px;
    }
  </style>
  <script>
    function calculate() {
      var input = document.getElementById("input");
      var result = eval(input.value);
      input.value = result;
    }
  </script>
</head>
<body>
  <div class="calculator">
    <input type="text" id="input">
    <br>
    <input type="button" value="1" onclick="input.value += '1'">
    <input type="button" value="2" onclick="input.value += '2'">
    <input type="button" value="3" onclick="input.value += '3'">
    <input type="button" value="+" onclick="input.value += '+'">
    <br>
    <input type="button" value="4" onclick="input.value += '4'">
    <input type="button" value="5" onclick="input.value += '5'">
    <input type="button" value="6" onclick="input.value += '6'">
    <input type="button" value="-" onclick="input.value += '-'">
    <br>
    <input type="button" value="7" onclick="input.value += '7'">
    <input type="button" value="8" onclick="input.value += '8'">
    <input type="button" value="9" onclick="input.value += '9'">
    <input type="button" value="*" onclick="input.value += '*'">
    <br>
    <input type="button" value="0" onclick="input.value += '0'">
    <input type="button" value="." onclick="input.value += '.'">
    <input type="button" value="=" onclick="calculate()">
    <input type="button" value="/" onclick="input.value += '/'">
    <br>
    <input type="button" value="Clear" onclick="input.value = ''">
  </div>
</body>
</html>
