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

  <!-- <div class="main-content px-3 py-2">
    <NuxtLink to="/event">
      <img src="~/assets/img/home.jpeg" alt="Ella Gonzales, Light Gather, watercolour on jusi silk and pinewood support (image credit and courtesy of the artist)">
      <small>Ella Gonzales, <em>Light Gather</em>, 2022, Image credit and courtesy of the artist.</small>

    </NuxtLink>

  </div> -->

  <div class="d-flex row main-content px-3 py-2">
    <div class="align-self-center my-5">

      <div class="home-img">
        <small>Ella Gonzales, <em>Light Gather</em>, 2022, Image credit and courtesy of the artist.</small>
        <NuxtLink to="/event"><img src="~/assets/img/home.jpeg" alt="Ella Gonzales, Light Gather, watercolour on jusi silk and pinewood support (image credit and courtesy of the artist)"></NuxtLink>
      </div>

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
  layout: 'home',
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
img {
  width: 100%;
  height: 100%;
  object-fit: contain;
}
</style>
