<template>
<!-- <Tutorial/> -->
<div class="container">
  <span id="menu-btn" v-b-toggle.sidebar-1>
    <b-icon icon="list"></b-icon>
  </span>
  <b-sidebar id="sidebar-1" title="Menu" shadow>
    <div class="px-3 py-2">
      <ul class="main-menu">
        <ul class="main-menu">
          <li v-for="post in posts" :key="post.ID_post">
            <NuxtLink :to="post.slug" v-html="post.title"></NuxtLink>
          </li>
          <li>
            <a href="https://www.google.com/maps/@43.7206796,-79.5121837,12z/data=!3m1!4b1!4m3!11m2!2sIcghjJhITZyoW1qyQmNwDQ!3e3">
              FilipiNEXT Map
            </a>
          </li>
        </ul>
      </ul>
    </div>
  </b-sidebar>

  <div class="d-flex row main-content px-3 py-2">
    <div class="align-self-center my-5">
      <h1 class="placeholder" v-html="posts[1].title"></h1>
      <p>We recognize that many Indigenous Nations have longstanding relationships with the territories upon which York University campuses are located that precede the establishment of York University. York University acknowledges its presence on the traditional territory of many Indigenous Nations. The area known as Tkaronto has been care taken by the Anishinabek Nation, the Haudenosaunee Confederacy, and the Huron-Wendat. It is now home to many First Nation, Inuit and Métis communities. We acknowledge the current treaty holders, the Mississaugas of the Credit First Nation. This territory is subject of the Dish with One Spoon Wampum Belt Covenant, an agreement to peaceably share and care for the Great Lakes region. We are grateful for the opportunity to carry out our intellectual and creative work on Turtle Island, the present-day home to a diverse population of Indigenous and other peoples and respect the continued connections with the past, present and future in forging decolonial relations with Indigenous and other peoples within Canada, the Philippines, and beyond.</p>
    </div>
  </div>

</div>
</template>

<script>
export default {
  name: 'IndexPage',
  data() {
    return {
      posts: []
    }
  },
  async asyncData({
    $axios
  }) {
    const posts = await $axios.$get('/api/pages.json')
    return {
      posts
    }
  }
}
</script>

<style lang="scss">
</style>
