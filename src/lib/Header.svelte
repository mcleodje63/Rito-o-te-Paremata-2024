<script>
  import { onMount } from "svelte";
  let vid;
  onMount(() => {
    vid = document.getElementById("myVideo");
  });
</script>

<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<header>
  <h1 class="title">Rito o te Pāremata 2024</h1>
  <h2>
    <a href="mailto:jessiejammcleod@gmail.com"><img src="gmail.png" alt="gmail" /></a><a href="https://www.linkedin.com/in/jessie-mcleod-a44b3a249"><img src="linkedin.png" alt="linkedin" /></a>
    <a href="https://instagram.com/jessiejammcleod?igshid=MzMyNGUyNmU2YQ=="><img src="instagram.png" alt="instagram" /></a>
  </h2>
</header>

<div class="cropped-image">
  <div class="headings">
    <h2>Jessie McLeod</h2>
  </div>
  <video id="myVideo" max-width="100%" height="auto" autoplay loop muted>
    <source src="rito2.0.mp4" type="video/mp4" />
  </video>
</div>

<style>
  header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    /* background-color: black; */
  }
  h1 {
    margin: 1vw;
    font-size: 4vw;
    color: #20cca4;
    text-shadow: 0.5px 0.5px 0.5px black;
  }
  img {
    width: 1.8vw;
    margin: 0.3vw;
    margin-top: 1vw;
  }
  video {
    display: block;
    margin-left: auto;
    margin-right: auto;
  }

  .cropped-image {
    position: relative;
    max-width: 100%; /* Set the desired width */
    height: 315px; /* Set the desired height */
    overflow: hidden; /* Hide overflowing parts of the image */
  }

  .cropped-image video {
    width: 100vw; /* Make the image fill the container */
    height: 24.5vw; /* Make the image fill the container */
    object-fit: cover; /* Maintain aspect ratio and cover the container */
    object-position: bottom;
  }
  .cropped-image h2 {
    position: absolute;
    top: 50%;
    padding-left: 30vw;
    transform: translate(-50%, -50%);
    color: white;
    font-size: 3.5vw; /* Adjust the font size as needed */
    text-shadow: 2px 2px 2px #000000;
  }
</style>
