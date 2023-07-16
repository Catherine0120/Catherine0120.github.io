---
title: "Tsinghua Overall-Merit Scholarship Presentation"
excerpt: "An introduction to me myself by the end of my freshman year.<br/> <img src='/images/portfolio_1/slide1.png' style="zoom:80%"/>"
collection: portfolio
---

Here is the PowerPoint where I used in presentation for my Tsinghua Overall-Merit Scholarship. You may find more about me during my freshman year through it.

<html>
<head>
  <style>
    .marquee {
      width: 100%;
      overflow: hidden;
      white-space: nowrap;
      box-sizing: border-box;
    }
    .marquee span {
      display: inline-block;
      padding-left: 100%;
      animation: marqueeText 15s linear infinite;
    }
    @keyframes marqueeText {
      0% { transform: translateX(0); }
      100% { transform: translateX(-100%); }
    }
    /* Additional styles for slide container */
    .slide-container {
      width: 100%;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      overflow: hidden;
    }
    .slide {
      width: 100%;
      height: 100%;
      object-fit: contain;
    }
    /* Navigation buttons */
    .navigation {
      display: flex;
      justify-content: center;
      margin-top: 20px;
    }
    .navigation button {
      margin: 0 10px;
    }
  </style>
  <script>
    var slides = [];
    var currentSlide = 0;
    slides.push("/images/portfolio_1/slide1.png");
    slides.push("/images/portfolio_1/slide2.png");
    slides.push("/images/portfolio_1/slide3.png");
    slides.push("/images/portfolio_1/slide4.png");
    slides.push("/images/portfolio_1/slide5.png");
    slides.push("/images/portfolio_1/slide6.png");
    slides.push("/images/portfolio_1/slide7.png");
    slides.push("/images/portfolio_1/slide8.png");
    function changeSlide(index) {
      var slideElement = document.getElementById("slide");
      currentSlide = index;
      slideElement.src = slides[currentSlide];
    }
    function previousSlide() {
      currentSlide = (currentSlide - 1 + slides.length) % slides.length;
      changeSlide(currentSlide);
    }
    function nextSlide() {
      currentSlide = (currentSlide + 1) % slides.length;
      changeSlide(currentSlide);
    }
  </script>
</head>
<body>
  <div class="slide-container" id="slide-container">
    <img class="slide" id="slide" src="/images/portfolio_1/slide1.png">
  </div>
  <div class="navigation">
    <button onclick="previousSlide()">Previous Page</button>
    <button onclick="nextSlide()">Next Page</button>
  </div>
</body>
</html>