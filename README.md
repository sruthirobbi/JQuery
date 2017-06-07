# JQuery
<!DOCTYPE html>
<html>
<head>
	<title>Sruthi Portfolio</title>
	<link rel="stylesheet" type="text/css" href="JS/PF_stylings.css"/>
	<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
	<script type="text/javaScript" src="../JS/Javascript.js"></script>
</head>
<body id="body">
	<div class="navigation">
		<nav id="logo">	
			<a href="#">Sruthi Robbi</a>
		</nav>
		<nav id="menu">
			<a href="#Experience">Experience</a>
			<a href="#">Education</a>
			<a href="#">Skills</a>
			<a href="#">Contact</a>
		</nav>
	</div>
	<div id="BGimage">
		<div id="myimage">
			<img id="image" src="Images/my-image.JPG" alt="my Image"/>
		</div>
		<div id="intro">
			<p id="profile-name">SRUTHI R</p>
			<p class="detail-headings">Front End Developer</p>
			<p class="detail-headings">Phone:</p>
			<p class="details"></p>
			<p class="detail-headings">Email:</p>
			<p class="details">sruthidhar.r@gmail.com</p>
			<p class="detail-headings">Address:</p>
			<p class="details">Maryland</p>
		</div>
		<div id="Experience">
			<div id="expyear"> 
				<p>Junior Analyst</p>
				<p>2013-2015</p>
			</div>
			<div id="expname">
				<p>Opinesoft Solutions Pvt Ltd</p>
				<p>Technologies Used: HTML5, CSS3, JavaScript, JQuery, Bootstrap</p>
			</div>
		</div>
	</div>
	<footer>
		<div>&copy By Sruthi Robbi</div>
	</footer>
	<script type="text/javaScript">
		$(document).ready(function(){
			$(body).mouseover(slideright);
			$(body).mouseover(fade);
			$("#Experience").click(displayexp);
		function slideright()
		{
			$("#image").animate({'marginLeft':'35%'},2000);
			$("#expyear").hide();
			$("#expname").hide();
			$("#intro").animate({'marginLeft':'-1%','margin-left':'10%'},2000);
		}

		function displayexp()
		{
			$("#expyear").show();
			$("#expname").show();
			$("#image").hide();
			$("#intro").hide();

		}

});

	</script>
</body>
</html>
