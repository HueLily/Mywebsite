<!DOCTYPE html>
<html>
<body>

<h2>Set your password</h2>

<p>Please enter a number between 100 and 999 to set your password.</p>

<input id="numb">

<button type="button" onclick="myFunction()">Set</button>

<p id="mywebsite"></p>

<p>Please click here after you set your password.</p>

<input type="button" value="Next" onclick="newDoc()">

<script>
function myFunction(){
	let x = document.getElementById("numb").value;

	let text;
	if(isNaN(x) || x < 100 || x > 999){
		text ="Password is not valid. Please enter a number between 100 and 999.";
	} else{ 
		text ="You successfully set your password in the website.";
	}
	document.getElementById("mywebsite").innerHTML = text;
}

function newDoc(){
	window.location.assign("file:///Users/nguyenhue/Desktop/My%20first%20web3.html")
	
}
</script>

</head>
</html>
