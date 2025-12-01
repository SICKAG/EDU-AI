# SICK Training kit: Artificial intelligence

Welcome to the GitHub for the SICK's Training kit: Artificial intelligence!

If you purchased the Training kit: Artificial intelligence from SICK, you are right here.

<style>
  .slideshow-container {
    position: relative;
    width: 600px; /* adjust as needed */
    margin: auto;
    overflow: hidden;
  }

  .slide {
    display: flex;
    transition: transform 1s ease-in-out;
    width: 100%;
  }

  .slide img {
    width: 100%;
    flex-shrink: 0;
  }

  /* Arrows */
  .arrow {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    font-size: 2rem;
    color: gray;
    background: none;
    border: none;
    cursor: pointer;
    z-index: 10;
  }

  .arrow-left {
    left: 10px;
  }

  .arrow-right {
    right: 10px;
  }
</style>

<div class="slideshow-container">
  <div class="slide" id="slide">
    <img src="images/set1.jpg" alt="Image 1">
    <img src="images/set2.jpg" alt="Image 2">
    <img src="images/set3.jpg" alt="Image 3">
  </div>
  <button class="arrow arrow-left" onclick="prevImage()">&lt;</button>
  <button class="arrow arrow-right" onclick="nextImage()">&gt;</button>
</div>

<script>
  const slide = document.getElementById('slide');
  const totalImages = slide.children.length;
  let index = 0;

  function updateSlide() {
    slide.style.transform = `translateX(-${index * 100}%)`;
  }

  function nextImage() {
    index = (index + 1) % totalImages;
    updateSlide();
  }

  function prevImage() {
    index = (index - 1 + totalImages) % totalImages;
    updateSlide();
  }

  // Auto-slide every 3 seconds
  setInterval(nextImage, 5000);
</script>

<br>
Don’t have a kit yet? Purchase yours here!

**[sick.com](https://www.sick.com/p/p665966)**

Please note that this kit is intended for educational purposes only and must not be used in production environments.

Got your Training Kit? Start exploring now!

- [Overview](overview/foreword.md)
- [Exercises](exercises/exercise1.md)
- [Troubleshooting](troubleshoot.md)
