<script>
  import Header from "$lib/Header.svelte";
  import Footer from "$lib/Footer.svelte";
  import { onMount } from "svelte";
  let vid;
  onMount(() => {
    vid = document.getElementById("myVideo");
  });
</script>

<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />

<main>
  <header><Header /></header>

  <div class="cropped-image">
    <video id="myVideo" max-width="100%" height="auto" autoplay loop muted>
      <source src="rito2.0.mp4" type="video/mp4" />
    </video>
    <div class="headings">
      <h2>Jessie McLeod</h2>
    </div>
  </div>
  <section class="content section columns">
    <article class="column left">
      <p>My name is Jessie McLeod, I’m 16, and a year 12 student at Craighead Dioscean. I live in Timaru, a port town two hours south of Christchurch, and have for my whole life. This constant stability in a chaotic world has allowed me to get involved and make connections in a variety of areas which I hold a passion for. In my spare time I enjoy spending time outdoors with my friends and family, cooking, reading and writing poetry, but also coding, photography, watching tv, football and playing guitar.</p>
    </article>
    <figure class="column right">
      <img src="seaweek.jpg" alt="Seaweek" />
      <!-- remember to link to news article  -->
    </figure>
  </section>
  <section class="content section columns">
    <figure class="column left">
      <img src="scumna.JPG" alt="sumnerYouthGroup" />
    </figure>
    <article class="column right">
      <ul>
        <li>Top SVA Volunteer Craighead 2023</li>
        <li>Member of national Anglican General Snyod 2024</li>
        <li>Experience working with people, from babies to seniors</li>
      </ul>
      <p>Since the start of this year, I’ve been on Vestry at St John’s Anglican Church, and attended Christchurch Dioscean Synod, which has been a great experience for me, and I plan to remain in this role until I’ve graduated high school. Another aspect of St. Johns Church which I am heavily involved in, is our church's A Rocha’s EcoChurch group, which involves working in organising events, teaming up with people from different generations/backgrounds, and sending a lot of emails.</p>
      <br />
    </article>
  </section>
  <section class="content section columns">
    <article class="column left">
      <p>During my time at Craighead, I was lucky enough to be selected to attend two model EU’s held at the University of Canterbury, which allowed me to explore diplomacy and working with others. Volunteering for my community has also been very important to me, I’ve been involved in helping with the Craighead uniform shop, Sunday school, Sustainable Coastlines, early vote counting, as well as many others, and gathered over 100 hours on the SVA website.</p>
      <br />
      <p>I want to be a part of Rito to discover hands on the inner workings of a system which affects me and learn more about Aotearoa New Zealand’s government. I may not know much about Parliament, however I’m naturally a curious and interested person, so this role is right for me.</p>
    </article>
    <figure class="column right">
      <img src="@MtCook.JPG" width="100%" alt="mountCook" />
    </figure>
  </section>
</main>

<Footer />

<style>
  ul {
    background-color: #20cca4;
    border: 1px solid #19a182;
    padding: 5vh;
    font-size: 1.3vw;
  }
  h2 {
    font-size: 130%;
    text-align: center;
  }
  p {
    font-size: 1.6vw;
    margin-left: 5px;
  }
  video {
    display: block;
    margin-left: auto;
    margin-right: auto;
  }
  /* come back to columns */
  .columns {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .left {
    width: 50vw;
  }
  .right {
    width: 50vw;
  }

  .cropped-image {
    position: relative;
    max-width: 100%; /* Set the desired width */
    height: 315px; /* Set the desired height */
    overflow: hidden; /* Hide overflowing parts of the image */
  }

  .cropped-image video {
    width: 100%; /* Make the image fill the container */
    height: 100%; /* Make the image fill the container */
    object-fit: cover; /* Maintain aspect ratio and cover the container */
    object-position: bottom;
  }
  .cropped-image h2 {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    color: white;
    text-align: center;
    font-size: 3em; /* Adjust the font size as needed */
    text-shadow: 1px 1px 1px #000000;
  }
</style>
