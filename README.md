# hello-world
Sample Repository 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">	
    <title>Future Value Application</title>
    <script>
    		var again = "y";
		var futureValue;
	do{
		// get user entries
		var investment = prompt("Enter investment amount as xxxxx.xx", 10000);
		investment = parseFloat(investment);
		var rate = prompt("Enter interest rate as xx.x", 7.5);
		rate = parseFloat(rate);
		var years = prompt("Enter number of years", 10);
		years = parseInt(years);
		
		// calulate future value
		futureValue = investment;
		for (var i = 1; i <= years; i++ ) {
			futureValue = futureValue + (futureValue * rate / 100);
		}
		futureValue = parseInt(futureValue);
	}while(again == "y")	
    </script>
</head>
<body>
    <main>
    	<script>
			document.write("Investment amount = " + investment);
			document.write(" Interest rate = " + rate);
			document.write(" Years = " + years);
			document.write(" Future Value is " + futureValue + "<br><br>");
			futureValue = investment;
			for (var i = 1; i <= years; i++ ) {
			x = futureValue * rate / 100
			futureValue = futureValue + (futureValue * rate / 100);
			document.write("year = " + i + " " + "Interest = " + x + " " + " " + "value = " + parseInt(futureValue) + "<br>");
		}
        </script>
        <br><br>Thanks for using the Future Value application.
    </main>
</body>
</html>
