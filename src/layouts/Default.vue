<template>
  <div>
    <header class="header">
      <strong>
        <g-link to="/">{{ $static.metadata.siteName }}</g-link>
      </strong>
      <nav class="nav">
        <g-link class="nav__link" to="/">
          Home
        </g-link>
        <g-link class="nav__link" to="/about/">
          About
        </g-link>
      </nav>
    </header>
    <div class="container mx-auto px-4">
      <slot />
    </div>
  </div>
</template>

<static-query>
  query {
    metadata {
      siteName
    }
  }
</static-query>

<style>
body {
  margin: 0;
  padding: 0;
  line-height: 1.5;
}
</style>
