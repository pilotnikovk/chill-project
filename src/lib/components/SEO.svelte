<script>
  export let title = "Chill — Создаем простоту";
  export let description = "Профессиональная разработка современных интерфейсов с акцентом на UX, скорость и чистоту кода.";
  export let url = "https://chill-project.vercel.app";
</script>

<svelte:head>
  <title>{title}</title>
  <meta name="description" content={description} />
  
  <!-- Open Graph -->
  <meta property="og:type" content="website" />
  <meta property="og:url" content={url} />
  <meta property="og:title" content={title} />
  <meta property="og:description" content={description} />
  <meta property="og:image" content="{url}/og-image.jpg" />

  <!-- Twitter -->
  <meta property="twitter:card" content="summary_large_image" />
  <meta property="twitter:url" content={url} />
  <meta property="twitter:title" content={title} />
  <meta property="twitter:description" content={description} />

  <!-- Schema.org JSON-LD -->
  <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "WebSite",
      "name": "Chill Project",
      "url": "{url}",
      "description": "{description}",
      "potentialAction": {
        "@type": "SearchAction",
        "target": "{url}/search?q={search_term_string}",
        "query-input": "required name=search_term_string"
      }
    }
  </script>
</svelte:head>
