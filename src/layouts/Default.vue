<template>
  <div class="container mx-auto">
    <header class="header grid grid-cols-2 gap-4 mb-8 pt-4">
      <strong>
        <g-link class="text-2xl" to="/">Cameron Baney</g-link>
      </strong>
      <nav class="flex flex-row justify-end space-x-8">
        <g-link class="text-xl" to="/">
          Home
        </g-link>
        <g-link class="text-xl" to="/about/">
          About
        </g-link>
      </nav>
    </header>

    <slot />
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
