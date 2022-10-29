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
      <h1 class="placeholder" v-html="posts[10].title"></h1>
      <p>Organizers of FilipiNEXT recognize that COVID-19 continues to circulate within our communities and that precautions must continue in order to maintain the health and safety of our workshop participants. <strong>Masks continue to be required
          in all indoor spaces at York.&nbsp;</strong><br /><br />Please see the registration table for rapid antigen tests, hand sanitizer, and masks, should you require any and visit <a
          href="https://www.yorku.ca/bettertogether/2022/04/13/york-to-keep-mandatory-masking/">this site</a> for updates around York University&rsquo;s COVID-19 response. Contact
        workshop organizers if you have any questions or concerns regarding our procedures around COVID-19. </p>
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
