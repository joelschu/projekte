<script>
    export let items;
</script>

<!-- <div class="back-next-button">
  <button>
    <a href="/">
      &#10005 Zurück
    </a>
  </button>
  <button>
    <a href="/">
      Nächstes &#8594
    </a>
  </button>
</div> -->

<div class="horizontal-scroll-container">
  {#each items as item (item.id)}
  <div class="img-horizontal-scroll">
      <img class=" blur-[3px]" src={item.image} alt={item.title} draggable="false" on:mouseenter={() => item.isHovered = true}
    on:mouseleave={() => item.isHovered = false}/>
    {#if item.isHovered}
    <div class="hover-img-text">
        {item.title}
    </div>
    {/if}
  </div>
  {/each}
</div>
