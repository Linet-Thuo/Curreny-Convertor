# Curreny-Convertor
Using HTML, CSS and JavaScript
![CC](https://user-images.githubusercontent.com/60045349/105733033-22b99500-5f42-11eb-9bdc-4c2e5a6ac60e.png)
<html>

<head>
	<title>CURRENCY CONVERTER</title>
</head>

<style>
body{
	background: url(img.jpeg) center;
}

h1{
	text-align: center:;
	font-size: 38px;
	padding: 20px lem;
	font-weight: bold;
	margin-left: 35%;
	margin-right: 35%;
	cursor: pointer;
	font-family: Times New Roman;
}

marquee{
	font-size: 20px;
	padding-top: 6px;
	margin: -23px;
	margin-left: 35%;
	margin-right: 35%;
	cursor: pointer;
}

fieldset{
	width: 45%;
	margin:  auto;
	border: 1px solid #000;
	text-align: left;
	font-size: 20px;
	font-family: lato, san-serif;
}
input[type=number],[id]{
	background: #fff;
	border: 1px solid #000;
	border-radius: 2px;
	border-width: 1px;
	color: #36454b;
	font-size: 15px;
	margin:  5px;
	padding: 12px;
	display: inline-block;
}

input[type=button]{
	width: 80px;
	height:43px;
	font-weight: bold;
}

input[type=reset]{
	width: 95px;
	height:43px;
	font-weight: bold;
}
</style>


<body>

<h1>Currency Converter</h1>

<h2><marquee>Welcome to the Online Currency Convertor!</marquee></h2>
<br><br>

<form name="converter">

<fieldset>

<label>KES Currency(Shillings):</label>
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp
&nbsp 
<input type="number" name="shillings" required>

<input type="button" value="Convert" onclick="currencyConverter(converter.shillings.value)"><br><br>

<label>Dollar(America):</label>
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp

<input id="dollar"><br><br>

<label>Euro(Europe):</label>
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp

<input id="euro"><br><br>

<label>Yuan(China):</label>
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp	
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp

<input id="yuan"><br><br>

<label>Won(Korea):</label>
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp	
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp

<input id="won"><br><br>

<label>Riyal(Saudia):</label>
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp	
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp

<input id="riyal"><br><br>

<input type="reset" value="Reset Form">

<p align="center">You can press Reset Button for resetting the form.</p>

</fieldset>

</form>
<script>
function currencyConverter(valNum){
if(converter.shillings.value <= 0)
window.alert("Enter A Value Greater Than 0");
else{

document.getElementById("dollar").value = (valNum/100.798).toFixed(2);
document.getElementById("euro").value = (valNum/111.799).toFixed(2);
document.getElementById("yuan").value = (valNum/14.6932).toFixed(2);
document.getElementById("won").value = (valNum/0.111975).toFixed(2);
document.getElementById("riyal").value = (valNum/26.8794).toFixed(2);
}
}
</script>

</body>
</html>
