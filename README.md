<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8" />
		<title></title>
	</head>
	<link href="css/mystyle.css" rel="stylesheet" type="text/css"/>
	<script type="text/javascript" src="js/myjs.js">
		
	</script>
	
	<body>
		<div class="container">
			<div class="card">
				<div class =“content”>
					<
          H1> 1 </ H1>
					<p>假如给我三天光明</p>
					<a href="#">Read more</a>
				</div>
			</div>
			<div class="card">
				<div class="content">
					<h1>2</h1>
					<p>假如给我三天光明</p>
					<a href="#">Read more</a>
				</div>
			</div>
			<div class="card">
				<div class="content">
					<h1>3</h1>
					<p>假如给我三天光明</p>
					<a href="#">Read more</a>
				</div>
			</div>
			<div class="card">
				<div class="content">
					<h1>4 </h1>
					<p>假如给我三天光明</p>
					<a href="#">Read more</a>
				</div>
			</div>
		</div>
	</body>
</html>
*
{
	margin: 0;
	padding: 0;
	box-sizing: border-box;
	font-family: "微软雅黑",sans-serif;
}
body
{
	display: flex;
	justify-content: center;
	align-items: center;
	min-height: 100vh;
	background: linear-gradient(0deg,#fff 50%,#2196f3);
}
.container
{
	max-width: 1000px;
	position: relative;
	display: flex;
	justify-content: center;
	flex-wrap: wrap;
	transition: 0.5s;
}
.container .card
{
	position: relative;
	width: 250px;
	height: 300px;
	background: #fff;
	display: flex;
	justify-content: center;
	align-items: center;
	transition: 0.5s;
}
.container:hover .card
{
	filter: blur(5px);
	transform: scale(.85);
}
.container .card:hover
{
	filter: blur(0px);
	transform: scale(1);
}
.container .card:before
{
	content: "";
	position: absolute;
	width: 100%;
	height: 100%;
	background: #fff;
	z-index: 1;
	transition: 0.5s;
}
.container .card:hover:before
{
	background: #000;
	transform: scaleY(1.15);
	box-shadow: 0 5px 15px rgba(0,0,0,.2);
}
.container .card .content
{
	text-align: center;
	z-index: 2;
	padding: 0 20px;
	transition: 0.5s;
}
.container .card:hover .content
{
	color: #fff;
}
.container .card .content h1
{
	font-size:3em ;
}
.container .card .content p
{
	font-size: 0.9em;
}
.container .card .content a
{
	display: inline-block;
	margin-top: 15px;
	padding: 5px 10px;
	background: #262626;
	color: #fff;
	text-decoration: none;
}
.container .card:hover .content a
{
	 background: #2196F3;
}
