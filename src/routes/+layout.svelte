<script lang="ts">
  import './layout.css';
//   import "../app.css";
  import favicon from '$lib/assets/favicon.svg';
  import Particles from '$lib/Components/Particles.svelte';

  let { children } = $props();
</script>

<svelte:head>
  <link rel="icon" href={favicon} />
</svelte:head>

<div class="relative z-0">
  <Particles />
  
  <div class="relative z-10 text-white">
    <!-- This is how Svelte 5 displays page content -->
    {@render children()}
  </div>
</div>
