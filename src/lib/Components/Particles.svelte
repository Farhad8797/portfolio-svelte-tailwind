<script lang="ts">
  import { onMount } from 'svelte';
  import { tsParticles } from "@tsparticles/engine";
  import { loadSlim } from "@tsparticles/slim";

  onMount(async () => {
    await loadSlim(tsParticles);

    await tsParticles.load({
      id: "tsparticles",
      options: {
        fullScreen: { enable: true, zIndex: -1 },
        background: {
          // Change this to #000000 for a solid black background
          color: {value: "transparent"}
        },
        particles: {
          number: { value: 80 },
          color: {value: "#0000ff"}, // Particle color (White)
          links: { 
            enable: true, 
            distance: 150, 
            color: {value: "#0000ff"}, // Line color (White)
            opacity: 1.5
          },
          move: { enable: true, speed: 2 }
        }
      }
    });
  });
</script>

<div id="tsparticles"></div>