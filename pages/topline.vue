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
      <h1 class="placeholder" v-html="posts[8].title"></h1>
      <img class="topline" src="~/assets/img/topline.jpg" alt="Topline">

      <div class="topline-desc">
        <h2><strong>FilipiNEXT presents </strong><strong><em>Topline</em></strong><strong>: Filipinx Diaspora <br>and Sonic Aspirations in the City</strong></h2>
        <p><strong>July 13</strong><strong>th</strong><strong>, 2022</strong></p>
        <p><strong>7-9pm</strong></p>
        <p><strong>Doors at 6:30pm</strong></p>
        <p><strong>Innis Town Hall, </strong><strong>2 Sussex Ave, Toronto.</strong></p>
      </div>

      <p><strong>Screening, Q &amp; A, and live performances by creator, Romeo Candido, and lead actor, Cyrena Fiel.&nbsp;</strong></p>
      <p><strong>Special performance from Alexis Estropia and Gregory Dy Sun (Filipino Student&rsquo;s Association at York)</strong></p>
      <p><strong>Moderated by: Dr. Casey Mecija</strong></p>
      <p>Topline follows the story of a young Filipina from Scarborough who is discovered online and becomes a part of a popular music production team as one of their main songwriters. This event will feature a screening of three <em>Topline
      </em>episodes (approx. 15mins each), a question-and-answer period, and performances from the series creator and songwriter/composer, Romeo Candido, and lead actor, Cyrena Fiel.<em> Topline</em> is unprecedented as a
        pop culture representation of Filipinx youth, diaspora, music production and performance, and family in the contemporary city. This event will open discussion about the musical lineages and aspirations of Filipinx musicians making and playing
        music in the city, and about the larger place of Filipinx diasporas and their musical contributions in urban Canada.</p>
      <p><em>Please note that masks will be required.&nbsp;</em></p>
      <p>FREE, but numbers are limited. You must register to attend: <a href="https://tinyurl.com/2en6b4yx">https://tinyurl.com/2en6b4yx</a></p>

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
.topline-desc {
    text-align: center;
    margin-top: 1em;
}

.topline {
    width: 100%;
}
</style>
