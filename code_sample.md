<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Fizz Buzz</title>
<script>

function fizzbuzz() {
	var display = document.getElementById('display');
	var displayHTML = "";
	for (i = 1; i < 101; i++) {//make it 1-100
		 //FizzBuzz when divisible by 3 and 5
		 if(i % 3==0 && i % 5==0){
			displayHTML+= "<p>"+"FizzBuzz"+"</p>";
		 }

		  //Buzz when divisible by 5
		  else if(i%5 == 0){
			displayHTML += "<p>"+"Buzz"+"</p>"; 
		  }
		  //Fizz when divisible by 3
		  else if(i % 3==0){
			displayHTML += "<p>"+"Fizz"+"</p>";
		  }
		  
		  else{
			continue;
		  }
		  displayHTML += "<p>" + i + "</p>"
		//displayHTML += "<p>" + i + "</p>";how to write it
	}
	display.innerHTML = displayHTML
}

</script>

</head>

<body onload="fizzbuzz()">
<div id="display">

</div>
</body>

</html>
