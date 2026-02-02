<script lang="ts">
     export let items = [
    { id: 1, title: "Brandmuster <span>&#8599</span>", image: "src/lib/assets/proj1-img-cover.jpg", link: "https://brandmuster.info", isHovered: false },
    { id: 2, title: "Der Montag", image: "src/lib/assets/proj2-img-cover.jpg", link: "/der-montag" , isHovered: false },
    { id: 3, title: "Shark Island", image: "src/lib/assets/proj3-img-cover.jpg", link: "/shark-island" , isHovered: false },
    { id: 5, title: "Sanctions, Scams & Deepfakes <span>&#8599</span>", image: "src/lib/assets/proj5-img-cover.jpg", link: "https://russia-eu-cars.airwars.org/" , isHovered: false},
    { id: 4, title: "Mind The Gap", image: "src/lib/assets/proj4-img-cover.jpg", link: "/mind-the-gap" , isHovered: false },
    { id: 6, title: "Dutch Airstrikes", image: "src/lib/assets/proj6-img-cover.jpg", link: "/dutch-airstrikes" , isHovered: false }
    // { id: 7, title: "Unvergessen", image: "src/lib/assets/proj7-img-cover.jpg", link: "/unvergessen" , isHovered: false }     
    ];

    let text = false;
    const toggleText = () => text = !text;
    
</script>
<!-- <div class="dot"></div> -->
<div id="header"></div>
<div class="header-bar">
  <div class="bar-text">
    <p class="main-title">
      Joel Schülin
    </p>
    <button class="about" on:click={toggleText}>
      Über mich 
      {#if text}
      <span>
        &#10005
      </span>
      {/if}
    </button>
    <button class="lang-button">
      <span class="german-button">DE </span><span class="slash-lang">/</span><span> ENG</span>
    </button>
  </div>
  {#if text}
    <p class="title-description" >
        Ich bin Architekt, Urbanist und Visual Researcher, habe in Leipzig, Weimar und London studiert und unter anderem bei Forensic Architecture und Airwars gearbeitet. Meine Arbeit setzt sich kritisch und kreativ mit räumlichen Phänomenen und Konflikten auseinander, ob im virtuellen, physischen oder konzeptionellen. Außerdem verfasse ich sporadisch Meinungsbeiträge für das <a href="https://www.migazin.de/author/joel-schuelin/" target="_blank">Migazin</a>. Wenn ihr Interesse an meiner Arbeit habt, <a class="mail-link" href="mailto:joelschuelin@gmail.com">schreibt mir gerne</a>!
        <br><br>
        Hier noch ein paar weitere Projekte, an denen ich mitgearbeitet habe: <a href="https://forensic-architecture.org/investigation/a-cartography-of-genocide" target="_blank">Cartography of a Genocide</a> &#8226; <a href="https://idf-tweets-gaza.airwars.org/" target="_blank">The Killings They Tweeted</a> &#8226; <a href="https://ghf.airwars.org/" target="_blank">Surviving the Gaza Humanitarian Foundation</a>
    </p>
  {/if}
</div>

<div class="masonry-container">
  {#each items as item (item.id)}
    <div class="masonry-item">
    <a href={item.link}>
        <img class=" blur-[3px]" src={item.image} alt={item.title} draggable="false" on:mouseenter={() => item.isHovered = true}
    on:mouseleave={() => item.isHovered = false}/>
    {#if item.isHovered}
    <div class="hover-img-text">
      {@html item.title}
    </div>
  {/if}
    </a>
    </div>
  {/each}
</div>
<div class="footer">
    <div class="footer-content">
      <p class="copyright-text">
          © 2026 Joel Schülin
      </p>
      <p class="typeface-credit">
        Typeface
        <a href="https://www.collletttivo.it/typefaces/ronzino" class="underline" target="_blank">
            RONZINO
        </a>
        <span class="typeface-foote-media">designed by Luigi Gorlero, Nunzio MazzaferroRONZINO by Colletttivo</span>
    </p>
    <p class="up-button">
      <a href="#header">
        hoch &#8593
      </a>
    </p>
    </div>
</div>