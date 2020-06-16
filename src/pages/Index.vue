<template>
  <Layout>
    <h1 class="text-6xl font-bold">
      Cameron Baney
    </h1>
    <h2 class="text-3xl font-semibold mb-6">
      Front-end Engineer
    </h2>
    <p class="text-2xl">
      I am a front-end engineer focusing on JavaScript, Vue, Sass and semantic
      HTML. My experience in design and UX helps create quality user friendly
      websites and software.
    </p>

    <ul>
      <li v-for="item in social" :key="item.icon">
        <a :href="item.link" target="_blank">{{ item.label }}</a>
      </li>
    </ul>
  </Layout>
</template>

<script>
export default {
  metaInfo: {},

  data() {
    return {
      social: [
        {
          link: 'https://github.com/cameronbaney',
          icon: 'github',
          label: 'GitHub'
        },
        {
          link: 'https://github.com/cbaney',
          icon: 'gitlab',
          label: 'GitLab'
        },
        {
          link: 'https://twitter.com/cameronbaney',
          icon: 'twitter',
          label: 'Twitter'
        },
        {
          link: 'https://linkedin.com/in/cameronbaney',
          icon: 'linkedin',
          label: 'LinkedIn'
        },
        {
          link: 'https://codepen.io/cameronbaney',
          icon: 'codepen',
          label: 'Codepen'
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped></style>
