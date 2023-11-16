<script>
  import Header from "$lib/Header.svelte";
  import Footer from "$lib/Footer.svelte";
  import { onMount } from "svelte";
  let vid;
  onMount(() => {
    vid = document.getElementById("myVideo");
  });
</script>

<Header />

<main>
  <h2>Jessie McLeod</h2>
  <video id="myVideo" width="320" height="176" autoplay loop muted>
    <source src="ritoVideo.mp4" type="video/mp4" />
  </video>

  <p>My name is Jessie McLeod, I’m 16, and a year 12 student at Craighead Dioscean I live in Timaru, a port town two hours south of Christchurch, and have for my whole life. This constant stability in a chaotic world has allowed me to get involved and make connections in a variety of areas which I hold a passion for. In my spare time I enjoy spending time outdoors with my friends and family, cooking, reading and writing poetry, but also coding, photography, watching tv, football and playing guitar.</p>

  <p>Since the start of this year, I’ve been on Vestry at St John’s Anglican Church, and attended Christchurch Dioscean Synod, which has been a great experience for me, and I plan to remain in this role until I’ve graduated high school. Another aspect of St. Johns Church which I am heavily involved in, is our church's A Rocha’s EcoChurch group, which involves working in organising events, teaming up with people from different generations/backgrounds, and sending a lot of emails. During my time at Craighead, I was lucky enough to be selected to attend two model EU’s held at the University of Canterbury, which allowed me to explore diplomacy and working with others. Volunteering for my community has also been very important to me, I’ve been involved in helping with the Craighead uniform shop, Sunday school, Sustainable Coastlines, early vote counting, as well as many others, and gathered over 100 hours on the SVA website.</p>

  <p>I want to be a part of Rito to discover hands on the inner workings of a system which affects me and learn more about Aotearoa New Zealand’s government. I may not know much about Parliament, however I’m naturally a curious and interested person, so this role is right for me.</p>
</main>

<Footer />

<style>
  h2 {
    font-size: 1.5vw;
    text-align: center;
  }
  p {
    margin: 1vw;
  }
  video {
    display: block;
    margin-left: auto;
    margin-right: auto;
  }
</style>
