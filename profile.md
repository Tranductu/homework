# homework

<!DOCTYPE html>
<html>
<title>My Profile</title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Raleway">
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
    <head>
        <meta charset="utf-8">
        <style>
          * {
            box-sizing:border-box
          }
          h2 {
            text-align: center;
          }
          .slideshow-container {
            max-width: 500px;
            position: relative;
            margin: auto;
          }
          .mySlides {
              display: none;
          }
          .text {
            color: #f2f2f2;
            font-size: 15px;
            padding: 8px 12px;
            position: absolute;
            bottom: 8px;
            width: 100%;
            text-align: center;
          }

          }
          .active, .dot:hover {
            background-color: #717171;
          }
          .fade {
            -webkit-animation-name: fade;
            -webkit-animation-duration: 3s;
            animation-name: fade;
            animation-duration: 3s;
          }

          @-webkit-keyframes fade {
            from {opacity: .4} 
            to {opacity: 1}
          }

          @keyframes fade {
            from {opacity: .4} 
            to {opacity: 1}
          }
        </style>
    </head>
    <body> 
      <div class="slideshow-container">
        <div class="mySlides fade">
          <img src="family.jpg" style="width:100%">
        </div>

        <div class="mySlides fade">
          <img src="family1.jpg" style="width:100%">
        </div>

        <div class="mySlides fade">
          <img src="family2.jpg" style="width:100%">
        </div>
        <div class="mySlides fade">
          <img src="family4.jpg" style="width:100%">
        </div>       
      </div>
      <br>

      <div style="text-align:center">
        <span class="dot" onclick="currentSlide(0)"></span> 
        <span class="dot" onclick="currentSlide(1)"></span> 
        <span class="dot" onclick="currentSlide(2)"></span> 
      </div>  
    </body>
    <script>
      var slideIndex;
      function showSlides() {
          var i;
          var slides = document.getElementsByClassName("mySlides");
          var dots = document.getElementsByClassName("dot");
          for (i = 0; i < slides.length; i++) {
             slides[i].style.display = "none";  
          }
          for (i = 0; i < dots.length; i++) {
              dots[i].className = dots[i].className.replace(" active", "");
          }

          slides[slideIndex].style.display = "block";  
          dots[slideIndex].className += " active";
          slideIndex++;
          if (slideIndex > slides.length - 1) {
            slideIndex = 0
          }    
          setTimeout(showSlides, 5000);
      } 
      showSlides(slideIndex = 0);


      function currentSlide(n) {
        showSlides(slideIndex = n);
      }
    </script>
<style>
body,h1,h2,h3,h4,h5 {font-feature-settings:  "Raleway", sans-serif}
</style>
<body class="w3-light-grey">
<div class="w3-content" style="max-width:1400px">
<header class="w3-container w3-center w3-padding-32"> 
  <h1><b>MY PROFILE</b></h1>
  <p>Welcome to the profile of <b>Trần Đức Tú</b></p>
</header>
<div class="w3-row">
<div class="w3-col l8 s12">
  <header class="w3-container w3-center w3-padding-32">
  <h3><b>Những Chuyến Đi Dài</b></h3>
  </header>
  <div class="w3-card-4 w3-margin w3-white">
    <img src="phinhho.jpg" alt="Autumw" style="width:100%">
    <div class="w3-container">
      <h3><b>MHX - 2013</b></h3>
      <h5>Phinh Ho, <span class="w3-opacity">July , 2013</span></h5>
    </div>

    <div class="w3-container">
      <p>=================================================  .</p>
    </div>
  </div>
  <hr>
  <div class="w3-card-4 w3-margin w3-white">
  <img src="ngay1.jpg" alt="Norway" style="width:100%">
    <div class="w3-container">
      <h3><b>MHX - 2014</b></h3>
      <h5>Phuc Tuy, <span class="w3-opacity">July, 2014</span></h5>
    </div>

    <div class="w3-container">
      <p>=================================================.</p>
    </div>
  </div>
</div>
<div class="w3-col l4">
  <header class="w3-container w3-center w3-padding-32"> 
  <h3><b>My Profile</b></h3>
</header>
  <div class="w3-card-2 w3-margin w3-margin-top">
  <img src="tu0.jpg" class="img-thumbnail" alt="Cinque Terre" width="250" height="200">
    <div class="w3-container w3-white">
      <p>My Name : Trần Đức Tú</p>
      <p>Date of birth : 29 - 08 - 1993</p>
      <p>My hobby : chơi game, đọc sách</p>
      <p>My Phone number <span class="glyphicon glyphicon-phone-alt"></span> : 0981969311</p>
      <p>Facebook <a href="https://www.facebook.com/Lynn.siwi" target="_blank"> Link </a></p>
    </div>
  </div><hr>
  <head>
    <h3><b>Gallety</b></h3>
<style>
div.gallery {
    margin: 5px;
    border: 1px solid #ccc;
    float: left;
    width: 180px;
}

div.gallery:hover {
    border: 1px solid #777;
}

div.gallery img {
    width: 100%;
    height: auto;
}

div.desc {
    padding: 15px;
    text-align: center;
}
</style>
</head>
<body>

<div class="gallery">
  <a target="_blank" href="ky1.jpg">
    <img src="ky1.jpg" alt="Ky yeu 2014" width="600" height="400">
  </a>
  <div class="desc">Ky yeu 2014</div>
</div>

<div class="gallery">
  <a target="_blank" href="f.jpg">
    <img src="f.jpg" alt="My friend" width="600" height="400">
  </a>
  <div class="desc">My friend</div>
</div>

<div class="gallery">
  <a target="_blank" href="family.jpg">
    <img src="family.jpg" alt="Gia Dinh" width="600" height="400">
  </a>
  <div class="desc">My family</div>
</div>

<div class="gallery">
  <a target="_blank" href="ngay1.jpg">
    <img src="ngay1.jpg" alt="Nhungchuyendi" width="600" height="400">
  </a>
  <div class="desc">MHX-2014</div>
</div>

</body>
  <div class="w3-card-2 w3-margin">
    <div class="w3-container w3-padding">
      <h4>Popular Posts</h4>
    </div>
    <ul class="w3-ul w3-hoverable w3-white">
      <li class="w3-padding-16">
        <img src="tr.jpg" alt="Image" class="w3-left w3-margin-right" style="width:50px">
        <span class="w3-large">Tran Duc Trung</span><br>
        <p>Vietnamese <a href="https://www.facebook.com/tdtrung93" target="_blank">My Bro</a></p>
      </li>
      <li class="w3-padding-16">
        <img src="ath.jpg" alt="Image" class="w3-left w3-margin-right" style="width:50px">
        <span class="w3-large">Tran Duc Thang</span><br>
        <p>Vietnamese <a href="https://www.facebook.com/thangtd90" target="_blank">My bro</a></p>
      </li>
      <li class="w3-padding-16">
        <img src="hoan.jpg" alt="Image" class="w3-left w3-margin-right" style="width:50px">
        <span class="w3-large">Tran Duc Hoan</span><br>
        <p>Vietnamese <a href="https://www.facebook.com/profile.php?id=100006037779878" target="_blank">My Bro</a></p>
      </li>   
      <li class="w3-padding-16">
        <img src="li.jpg" alt="Image" class="w3-left w3-margin-right" style="width:50px">
        <span class="w3-large">Tran Ngoc Linh</span><br>
        <p>Vietnamese <a href="https://www.facebook.com/linh.tranngoc.16" target="_blank">My Sis</a></p>
      </li>  
    </ul>
  </div>
  <hr> 

</div>


</div><br>


</div>


<footer class="w3-container w3-dark-grey w3-padding-32 w3-margin-top">
  <button class="w3-button w3-black w3-disabled w3-padding-large w3-margin-bottom">Previous</button>
  <button class="w3-button w3-black w3-padding-large w3-margin-bottom">Next &raquo;</button>
</footer>

</body>
</html>
