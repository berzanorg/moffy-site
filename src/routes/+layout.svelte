<script lang="ts">
  import '../app.css'

  let { children } = $props()

  const title = 'Moffy - Sad. Poor. Fat. On testnet.'
  const description = 'Sad. Poor. Fat. On testnet.'
  const url = 'https://moffy.pages.dev'
  const themeColor = '#ffffff'
  const colorScheme = 'only light'
  const keywords = ['moffy', 'moffysad', 'monad', 'kuru']
  const twitter = '@Moffysad'
  const author = 'Berzan'
  const image = 'preview.webp'
</script>

<svelte:head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <link rel="manifest" href="/manifest.webmanifest" />
  <link rel="icon" href="/favicon.svg" type="image/svg+xml" />
  <link rel="apple-touch-icon" href="/apple-touch-icon.png" />
  <meta name="theme-color" content={themeColor} />
  <meta name="color-scheme" content={colorScheme} />
  <meta name="keywords" content={keywords.join(', ')} />
  <meta name="author" content={author} />
  <meta property="og:type" content="website" />
  <meta name="twitter:card" content="summary_large_image" />
  <meta name="twitter:site" content={twitter} />
  <meta name="twitter:creator" content={twitter} />
  <title>{title}</title>
  <meta name="description" content={description} />
  <link rel="canonical" href={url} />
  <meta property="og:url" content={url} />
  <meta property="og:title" content={title} />
  <meta property="og:description" content={description} />
  <meta property="og:image" content="{url}/{image}" />
  <meta property="twitter:image" content="{url}/{image}" />
</svelte:head>

{@render children()}
