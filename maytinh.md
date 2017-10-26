# aaaa
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>maytinh</title>
</head>
<body>
	<style>
	p.serif {
    font-family: "Times New Roman", Times, serif;
}
	h2 {
    	color: maroon;
    	text-align: center;
	}

    * {padding: 0px; margin: 0px;}

    .calculator {
      width: 300px;
      height: 440px;
      margin: 40px auto;
      background-color: #B0C4DE;
      border: 3px solid black;
      padding: 20px;
      border-radius: 25px;
    }
    .input {
      width: calc(100%);
      background-color: white;
      border: 1px solid black;
      padding: 5px 1px;
      font-size:30px;
      border-bottom:;
      border-top-left-radius: 5px;
      border-top-right-radius: 5px;
      margin-top : 20px;
    }
    .output {
      width: calc(100%);
      background-color: white;
      border: 1px solid black;
      padding: 5px 1px;
      font-size: 30px;
      border-top: none;
      text-align: right;
      border-bottom-right-radius: 5px;
      border-bottom-left-radius: 5px;
      margin-bottom: 65px;
    }
    .button button {
      width: 200%;
      margin-top: 8px;
      padding: 8px;
      font-size: 20px;
      border: 1px solid black;
      border-radius: 4px;
      color: white;
    }
    button.number {background-color: #4682B4;width:70px;height:40px; border-radius: 25px;}
    button.event {background-color: #FFA500;width:70px;height:40px; border-radius: 25px;}
    button.equal {background-color: #808080;width:70px;height:40px; border-radius: 25px;}
    button.dot {background-color: #708090; width:70px;height:40px; border-radius: 25px;}
    button.clear {background-color: #FF4500;width:70px;height:40px; border-radius: 25px;}
    button.zero { width: 144.5px;}
    button.equal {background-color: #708090; width: 220px;margin-top: 20px}
	button.number {margin-top: 10px}
	body {
    background: url(chibi.jpg);
    background-size: 450px 450px;
    background-repeat: no-repeat;
    margin-top: 100px;
}
	</style>
	<div class="contener">
		<h2>Máy Tính Cơ Bản</<h2>
		<div class="calculator">
    		<p><input type="text" class="input" value=""></p>
    		<p><input type="text" class="output" value=""></p>

			<div>
			<p>
				<button type = "submit" class = "number">1</button>
				<button type = "submit" class = "number">2</button>
				<button type = "submit" class = "number">3</button>
				<button type = "submit" class = "clear">C</button>
			</p>
			<p>
				<button type = "submit" class = "number">4</button>
				<button type = "submit" class = "number">5</button>
				<button type = "submit" class = "number">6</button>
				<button type = "submit" class = "plus event">+</button>
			</p>
			<p>
				<button type = "submit" class = "number">7</button>
				<button type = "submit" class = "number">8</button>
				<button type = "submit" class = "number">9</button>
				<button type = "submit" class = "nimus event">-</button>
			</p>
			<p>
				<button type = "submit" class = "number zero">0</button>
				<button type = "submit" class = "dot">.</button>
				<button type = "submit" class = "divide event">/</button>
				<button type = "submit" class = "equal">=</button>
				<button type = "submit" class = "multiply event">*</button>

			</p>		
			</div>	
		</div>
	</div>
	<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>

	<script>
      $(document).ready(function() {
        $('.input').attr('disabled', 'true');
        $('.output').attr('disabled', 'true');
        $('.multiply').attr('disabled', 'true');
        $('.divide').attr('disabled', 'true');
      });
      a = "";
      $('.number, .clear').click(function() {
        $('.multiply').removeAttr('disabled');
        $('.divide').removeAttr('disabled');
        $('.dot').removeAttr('disabled');
        $value = $(this).html();
        a += $value;
        $('.input').val(a);
      });

      $('.dot').click(function(){
        $value = $(this).html();
        a += $value;
        $('.input').val(a);
        $('.dot').attr('disabled', 'true');
        $('.multiply').attr('disabled', 'true');
        $('.divide').attr('disabled', 'true');
      });

      $('.plus, .nimus, .multiply, .divide').click(function() {
        $value = $(this).html();
        a += $value;
        $('.input').val(a);
        $('.multiply').attr('disabled', 'true');
        $('.divide').attr('disabled', 'true');
      });

      $('.equal').click(function(){
        $('.output').val(eval(a));
        a = "";
      });

      $('.clear').click(function() {
        $('.input').val('');
        $('.output').val('');
        $('.dot').removeAttr('disabled');
        $('.multiply, .divide').attr('disabled', 'true');
        a = "";
      });
    </script>  

</body>
</html>
