<template>
  <!-- <Tutorial/> -->
  <div class="container">
  <span id="menu-btn" v-b-toggle.sidebar-1><b-icon icon="list"></b-icon></span>
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
      <h1 class="placeholder" v-html="posts[9].title"></h1>

      <div class="row">
        <p>York University; School of the Arts, Media, Performance, & Design at York U, Liberal Arts & Professional Studies at York U; York Centre for Asian Research;  Communication and Media Studies at York U; Anthropology at York U; Visual Art and Art History at York U; Centre for Feminist Research; Global Labour Research Centre; Institute for Research on Digital Literacies; Sensorium Centre for Digital Arts and Technology; Filipino Student’s Association at York;  Innis College, Urban Studies Program; OCAD, Public Visualization Lab, Dias:stories; Toronto Metropolitan University; Centre for Asian Canadian Research and Engagement at UBC; The Institute for Gender, Race, Sexuality, & Social Justice, Kultura, & Social Sciences and Humanities Research Council (SSHRC).</p>
        <!-- <div class="col-md-6 col-lg-4 col-sm-12">
            <img class="logo" src="~/assets/img/anth.jpg" alt="Anthropology logo">
        </div>
        <div class="col-md-6 col-lg-4 col-sm-12">
            <img class="logo" src="~/assets/img/comn.jpg" alt="Comn logo">
        </div>
        <div class="col-md-6 col-lg-4 col-sm-12">
            <img class="logo" src="~/assets/img/laps.png" alt="laps logo">
        </div>
        <div class="col-md-6 col-lg-4 col-sm-12">
            <img class="logo" src="~/assets/img/ampd.png" alt="ampd logo">
        </div>
        <div class="col-md-6 col-lg-4 col-sm-12">
            <img class="logo" src="~/assets/img/ycar.png" alt="ycar logo">
        </div>
        <div class="col-md-6 col-lg-4 col-sm-12">
            <img class="logo" src="~/assets/img/sshrc.jpg" alt="sshrc logo">
        </div>
        <div class="col-md-6 col-lg-4 col-sm-12">
            <img class="logo" src="~/assets/img/fsay.jpeg" alt="sshrc logo">
        </div>
        <div class="col-md-6 col-lg-4 col-sm-12">
            <img class="logo" src="~/assets/img/ubc.jpg" alt="ubc logo">
        </div>
        <div class="col-md-6 col-lg-4 col-sm-12">
            <img class="logo" src="~/assets/img/tmu.png" alt="ubc logo">
        </div>
        <div class="col-md-6 col-lg-4 col-sm-12">
            <img class="logo" src="~/assets/img/ocad.jpg" alt="Ocad logo">
        </div>
        <div class="col-md-6 col-lg-4 col-sm-12">
            <img class="logo" src="~/assets/img/grsj.png" alt="grsj logo">
        </div>
        <div class="col-md-6 col-lg-4 col-sm-12">
            <img class="logo" src="~/assets/img/innis.png" alt="innis logo">
        </div>
        <div class="col-md-6 col-lg-4 col-sm-12">
            <img class="logo" src="~/assets/img/irdl.png" alt="irdl logo">
        </div>
        <div class="col-md-6 col-lg-4 col-sm-12">
            <img class="logo" src="~/assets/img/sens.png" alt="sensorium logo">
        </div>
        <div class="col-md-6 col-lg-4 col-sm-12">
            <img class="logo" src="~/assets/img/dias.jpg" alt="dias logo">
        </div> -->

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
.logos {
  // background: #fff;
  padding:1em;
  .logo {
    padding: 1em;
    width: 100%;
    object-fit: contain;
  }
}

</style>
