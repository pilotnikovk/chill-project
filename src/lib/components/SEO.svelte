<script>
  import { onMount } from 'svelte';
  
  export let title = "Chill | Простота в каждом пикселе";
  export let description = "Профессиональная разработка интерфейсов с акцентом на UX, скорость и чистоту кода.";
</script>

<svelte:head>
  <title>{title}</title>
  <meta name="description" content={description} />
  <meta property="og:title" content={title} />
  <meta property="og:description" content={description} />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <meta charset="utf-8" />
</svelte:head>
