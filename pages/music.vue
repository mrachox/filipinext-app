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
      <h1 class="placeholder" v-html="posts[6].title"></h1>
      <p><strong><em>Filipinx Diasporic Mix Tapes</em></strong> is an audio visual archive of music produced by Filipinx musicians in Canada in the last decade. These music mixes invite the public to engage in sounds made in the Filipinx diaspora in
        order to recognize the history and ongoing creative labour of Filipinx musicians in Canada. These music lists were compiled by Joanna Delos Reyes as part of a SSHRC project entitled: <em>Diasporic Mix Tape: Fostering Filipinx Intimacies in
          Canada Through Sound: </em>PI: Dr. Casey Mecija.</p>
      <!-- Filipinx Diasporic Mix Tapes -->
      <iframe style="border-radius:12px" src="https://open.spotify.com/embed/playlist/6aRzVriwL3NJW7K8dlK5in?utm_source=generator" width="100%" height="380" frameBorder="0" allowfullscreen=""
        allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"></iframe>

      <hr>

      <p>Videoplaylist of Filipinx musicians from or located in Canada.</p>

      <iframe width="100%" height="500" src="https://www.youtube.com/embed/videoseries?list=PLONFfJHzk-0MvGR2vP-X9tM_ws5IkdGkW" title="YouTube video player" frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

      <hr>

      <p><strong>The Pahinga Collective:</strong></p>
      <p>Dr. Conely de Leon, Jhona Binos, Jann Tracee Ko Din, Joelle Navarro, Mycah Panjaitan, and Mauriene Tolentino<br /><br />We are a small and newly formed collective of Filipina/x/o faculty, graduate students, community organizers, and service
        providers representing migrant, queer, and feminist grassroots organizations in Tkaronto. Our desire to form the Pahinga Collective stemmed from an urgent need to create a space that was by us and for us, a space where we could imagine
        otherwise. To us, pahinga encompasses many things. It means rest as much as it means stillness, ease, pause, reflection, and slowing down. </p>


      <iframe style="border-radius:12px" src="https://open.spotify.com/embed/playlist/30mzffVisIXayVMOd34NDt?utm_source=generator" width="100%" height="380" frameBorder="0" allowfullscreen=""
        allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"></iframe>


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
