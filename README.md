<!DOCTYPE html>
<html>
<head>
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<link rel="stylesheet" href="styles.css">
</head>
<body>

<h6> Jacob Hampton </h6>

<h1> 25th Anniversary Countdown! </h1>

<h2> Your 25th Anniversary is on September 9th, 2020 </h2>

<p> Love you </>

<div style="float: right;">
<img src="wed2.png" width="250" height="300" class="rotateimg90"></div>

<div style="text-align: left;">
<img src="wed1.png" width="250" height="300" class="rotateimg90"></div>

<div style="float: right;">
<img src="md3.jpg" width="300" height="200" class="rotateimg180"></div>

<div style="align: left;">
<img src="md2.jpg" width="300" height="200"></div>

<h3  id="demo"></p>


<script>
// Set the date we're counting down to
var countDownDate = new Date("Sep 9, 2020 12:00:00").getTime();

// Update the count down every 1 second
var x = setInterval(function() {

  // Get today's date and time
  var now = new Date().getTime();
    
  // Find the distance between now and the count down date
  var distance = countDownDate - now;
    
  // Time calculations for days, hours, minutes and seconds
  var days = Math.floor(distance / (1000 * 60 * 60 * 24));
  var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
  var seconds = Math.floor((distance % (1000 * 60)) / 1000);
    
  // Output the result in an element with id="demo"
  document.getElementById("demo").innerHTML = days + "d " + hours + "h "
  + minutes + "m " + seconds + "s ";
    
  // If the count down is over, write some text 
  if (distance < 0) {
    clearInterval(x);
    document.getElementById("demo").innerHTML = "EXPIRED";
  }
}, 1000);



</script>
</body>
</html>
