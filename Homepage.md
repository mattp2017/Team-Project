<!DOCTYPE html>

<html lang=en>

	<head>
		<meta charset=utf-8>
		*Feature Area code*
		<meta name="viewport" content="width-device-width, initial-scale=1">
		*Feature Area code*
		<title> </title>
	</head>
	<style>
		*{
			border:0;
			margin:0;
			padding:0;
			outline:0;
			box-sizing:border-box;
		}
		body{
			background:white;
			font-family:Verdana, sans-serif;
			font-size:17px;
			font-weight:bold;
		}
		.nav{
			background:#fff;
			min-height:59px;
			overflow:auto;
		}
		.nav .left{
			float:left;
			margin:lem;
		}
		ul{
			list-style:none;
		}
		.nav .left li{
			float:left;
		}
		a{
			display:block;
			padding:17px 20px;
			line-height:30px;
			color:#191919;
			text-decoration:none;
			font-size:17px;
		}
		.nav .left a:hover{
			background:#99ccff;
		}
		.mySlides{ 
        		display:none;
   		 }
		    img{
			vertical-align:middle;
		    }
		    .slideshow-contianer{
			max-width:1000px;
			position:relative;
			margin:auto;
		    }
		    .prev, .next{
			cursor: pointer;
			position:absolute;
			top:50%;
			width:auto;
			padding:16px;
			margin-top:-22px;
			color:white;
			font-weight:bold;
			font-size:18px;
			transition:0.6s ease;
			border-radius:0 3px 3px 0;
		    }
		    .next{
			right:0;
			border-radius:3px 0 0 3px;
		    }
		    .prev:hover, .next:hover{
			background-color:rgba(0,0,0,0.8);
		    }
		    .text{
			color:#f2f2f2;
			font-size:15px;
			padding:8px 12px;
			position:absolute;
			bottom:8px;
			width:100%;
			text-align:center;
		    }
		    .dot{
			cursor:pointer;
			height:15px;
			width:15px;
			margin:0 2px;
			background-color:gray;
			border-radius:50%;
			display:inline-block;
			transition:background-color 0.6s ease;
		    }
		    .active, .dot:hover{
			background-color: hsla(29, 87%, 45%, 0.637);
		    }
	</style>
	<body>
			<nav class="nav">
				<div class="nav-mobile">
				<ul class="left">
					<li><a href="#"><img src="tS_compass_cmyk_500px.pdf" alt="TruckSeekers" height="100" width="100"></a></li>
					<li><a href="#">Trucks for Sale</a></li>
					<li><a href="#">Sell Your Truck</a></li>
					<li><a href="#">Servicing</a></li>
				</ul>
			<form class="search-form">
				<input type="text" placeholder="Search"> 
				<button>Search</button>
				</form>
				</div>
			</nav>
			 <div class="SlideShow-container">

                <div class="mySlides">
                <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
                <a class="next" onclick="plusSlides(1)">&#10095;</a>
                    <div class="#">1 / 3</div>
                    <img src="BoJackson.jpeg" style="width:100%">
                    <div class="text">#</div>
                </div>
                <div class="mySlides">
                        <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
                        <a class="next" onclick="plusSlides(1)">&#10095;</a>
                    <div class="numbertext">2 / 3</div>
                    <img src="#" style="width:100%">
                    <div class="text">#</div>
                </div>
                <div class="mySlides">
                        <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
                        <a class="next" onclick="plusSlides(1)">&#10095;</a>
                        <div class="numbertext">3 / 3</div>
                        <img src="#" style="width:100%">
                        <div class="text">#</div>
                </div>
            </div>
            <br>
            <div style="text-align:center">
                <span class="dot" onclick="currentSlide(1)"></span>
                <span class="dot" onclick="currentSlide(2)"></span>
                <span class="dot" onclick="currentSlide(3)"></span>
            </div>
            <script>
            var slideIndex = 1;
            showSlides(slideIndex);

            function plusSlides(n) {
            showSlides(slideIndex += n);
            }

            function currentSlide(n) {
            showSlides(slideIndex = n);
            }

            function showSlides(n) {
            var i;
            var slides = document.getElementsByClassName("mySlides");
            var dots = document.getElementsByClassName("dot");
            if (n > slides.length) {slideIndex = 1}    
            if (n < 1) {slideIndex = slides.length}
            for (i = 0; i < slides.length; i++) {
                slides[i].style.display = "none";  
            }
            for (i = 0; i < dots.length; i++) {
                dots[i].className = dots[i].className.replace(" active", "");
            }
            slides[slideIndex-1].style.display = "block";  
            dots[slideIndex-1].className += " active";
            }
            </script>
  	</body>
</html>
