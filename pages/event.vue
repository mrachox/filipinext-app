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
        </ul>
        <li>
          <a href="https://www.google.com/maps/@43.7206796,-79.5121837,12z/data=!3m1!4b1!4m3!11m2!2sIcghjJhITZyoW1qyQmNwDQ!3e3">
            FilipiNEXT Map
          </a>
        </li>
      </ul>
    </div>
  </b-sidebar>

  <div class="main-content px-3 py-2">
    <div class="my-5">
      <h1 class="my-5 placeholder" v-html="posts[2].title"></h1>
      <p><strong>FilipiNEXT</strong> is a transdisciplinary workshop that engages in creative and generative discussions around Filipinx Studies emerging from the Canadian context. The workshop and accompanying events take place from July 13-15,
        2022, at York University (Toronto). Bringing together scholars, artists, activists and community members from all over Canada, the workshop explores the following questions: What tensions, aspirations, and lines of inquiry can emerge when we
        think critically about the history and future of Filipinx people in Canada? How will the past and present inform what is NEXT for Filipinx Studies in Canada?</p>
      <p>The organizing committee is formed by Filipinx scholars from multiple institutions: <strong>Dr. Casey Mecija</strong> (York), <strong>Dr. Marissa Largo</strong> (York) and <strong>Dr. John Paul Catungal</strong> (UBC) are the workshop
        chairs. Committee members include: <strong>Dr. Valerie Damasco</strong> (UofT), <strong>Dr. Conely De Leon</strong> (TMU), <strong>Dr. Lisa Davidson</strong> (York), <strong>Dr. May Farrales</strong> (SFU) and <strong>Dr. Ethel
          Tungohan</strong> (York).</p>

      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>Context</h2>
          </template>
          <template v-slot:content>
            <p>The burgeoning field of Filipinx Studies in Canada continues to offer critical commentaries on the ongoing legacies of imperial power, and yet the palimpsestic qualities of these intellectual engagements require specific historical,
              cultural, and political contextualization. FilipiNEXT thus takes up a temporal critique to show the limits, re-inscriptions, and future trajectories of Filipinx Studies in Canada and beyond. Temporality as a key analytic directs
              theoretical and conceptual attention to the exigencies of colonialism, as well as the multivalent expressions of transnational and diasporic imaginaries that link between the past, present, and future in linear and non-linear ways
              (Coloma et al. 2012; Espiritu et. al 2016; Isaac 2021). In this contemporary moment, amidst the reorganizing of social life spurred by the global pandemic, COVID-19&rsquo;s threat to public health reveals the continued disposability and
              replaceability of racialized and migrant people who are mercilessly jettisoned from Canadian borders, partly through the exhaustion of their labour. The disproportionate number of Filipinx laborers, nurses, and caregivers that have
              contracted the virus because of a lack of protection is staggering (Catungal 2021). The current crisis of health and labour experienced by Filipinx people in the Philippines and its diasporas are indelibly shaped by ongoing histories of
              colonialism. The theme of FilipiNEXT focuses on these temporal entanglements as sites of chronic, ephemeral, and aspirational forms of time that link Filipinx scholars across social, cultural, and political debates.</p>
            <p>The first edited collection on Filipinxs in Canada titled <em>Filipinos in Canada: Disturbing Invisibility </em>(Coloma et al. 2012) was released almost a decade ago. A subsequent edited volume, <em>Diasporic Intimacies: Queer
                Filipinos and Canadian Imaginaries</em> (Diaz, Largo, &amp; Pino 2017), expanded on existing scholarship to include an examination of the contributions of queer Filipinos to the Canadian cultural landscape. Building upon the landmark
              contributions of these two edited collections, FilipiNEXT addresses the shifting temporalities of Filipinx Studies, now, ten years after the first collection was released. Much of the existing research on Filipinx diaspora in Canada
              from the past decade has focused on the dominant labour economies of Filipinx immigrants and their impact on transnational kinship and diasporic subject formation (Kelly 2000; Tungohan 2015). The release of <em>Diasporic Intimacies
              </em>(Diaz, Largo, &amp; Pino 2017) signaled an important shift in Filipino Canadian Studies that dislodged an emphasis on issues of Filipinx invisibility (Espiritu et. al 2016, 7) and put forward queer Filipino Canadian sexualities as
              a framework for engaging with the creative and affective interventions of Filipinx diasporic life. FilipiNEXT is indebted to the epistemological terrain laid out by these anthologies and their legacies stimulate our examination of
              Filipinx Studies in contemporary times. Indeed, our workshop is framed by the premise that Filipinx subjectivity is articulated through multiple registers of time: the temporalities of labour, migration, settler colonialism, capital,
              climate change and the queer temporalities of diasporic life more broadly.</p>
            <p>Adapting Allan Issac&rsquo;s argument that &ldquo;[s]ubjects make worlds out of one colonized by capital time&rdquo; (2021), Filipinx Studies in Canada continues to reckon with how our lives are conditioned by the logics of
              colonialism. The field has importantly seen an increase in research that critically engages with, and reflects on, settler colonialism and white supremacy (Farrales 2019; Largo 2017; De Leon 2019). There has also been an emergence of
              Filipinx scholarship that examines transnational connections across Canada, the Philippines, and other sites, that expands on the socio-political conditions, historical contingencies and affective dimensions that produce global Filipinx
              experiences. Filipinx scholars in Canada have put forward formidable research about diasporic activism against fascist governments (Angeles 2020), the role of Christian faith in diasporic place-making, colonial sanitation regimes (Go
              &amp; Docot 2021), social media as sites of community policing and subversion (Cruz 2019), Indigenous research methodologies within the context of climate change (Aysel et al. 2021), the impacts of COVID-19 on Filipinx students and
              temporary migrant workers (Catungal &amp; Tungohan 2021) and sound as an aesthetic mode of queer representation (Mecija 2021). This workshop also importantly engages in popular and contemporary debates about the term
              &ldquo;Filipinx.&rdquo; As a linguistic entry point to discussing the material experiences and demands for rights and equity of LGBTQI+ people of Philippine-descent (Barrett et al., 2021,146), our use of &ldquo;Filipinx&rdquo; calls
              attention to the discursive developments and limits of the terms Filipino and Filipina with regards to contemporary understandings of gender and sexuality. The workshop name FilipiNEXT engages with the &ldquo;X&rdquo; in order to
              highlight the historical and intellectual shifts that signal what is &ldquo;NEXT&rdquo; for Filipinx Studies in Canada.
              <br>
              - Dr. Casey Mecija
            </p>
          </template>
        </V-accordion>
        <V-accordion>
          <template v-slot:title>
            <h2>List of References</h2>
          </template>
          <template v-slot:content>
            <p>Angeles, Leonora. &ldquo;Only in the Philippines? Postcolonial Exceptionalisms and Filipina Feminisms.&rdquo; <em>Critical Asian studies</em> 52.2 (2020): 226&ndash;247. Web.</p>
            <p>Aysal, Lara, et al. &ldquo;Voices We Carry within Us: A Trialogue about Climate Change, Indigenous Ways of Knowing and Activism.&rdquo; <em>Theatre Pedagogy in the Era of Climate Crisis</em>, Routledge, London, 2021, pp. 47&ndash;58.
            </p>
            <p>Barrett, K. U, Hanna, K. B, &amp; Palomar, A. (2021). In Defense of the X: Centering Queer, Trans, and Non-Binary Pilipina/x/os, Queer Vernacular, and the Politics of Naming. <em>Alon:&nbsp;</em><em>Journal for Filipinx American and
                Diasporic Studies</em>, 1(2). http://dx.doi.org/10.5070/LN41253177 Retrieved from https://escholarship.org/uc/item/7148255f</p>
            <p>Catungal, John Paul. &ldquo;Essential Workers and the Cultural Politics of Appreciation: Sonic, Visual and Mediated Geographies of Public Gratitude in the Time of COVID-19.&rdquo; <em>Cultural&nbsp;</em><em>geographies</em> 28.2
              (2021): 403&ndash;408. Web.</p>
            <p>Catungal, John Paul, and Ethel Tungohan. &ldquo;Racial Narratives on Repeat: Reflections on Collaborative Research on Asian International Students in COVID Times.&rdquo; Canadian literature 245 (2021): 157&ndash;193. Print.</p>
            <p>Coloma, Roland Sintos et al. Filipinos in Canada : Disturbing Invisibility. Toronto: University of Toronto Press, 2018. Web.</p>
            <p>Cruz, Cesi. &ldquo;Social Networks and the Targeting of Vote Buying.&rdquo; Comparative political studies 52.3 (2019): 382&ndash;411. Web.</p>
            <p>Docot, Dada. &ldquo;Multimodal Extractivism.&rdquo; American anthropologist 123.3 (2021): 689&ndash;693. Web.</p>
            <p>De Leon, Adrian. &ldquo;Sugarcane Sakadas: The Corporate Production of the Filipino on a Hawai&rsquo;i Plantation.&rdquo; <em>Amerasia journal</em> 45.1 (2019): 50&ndash;67. Web.</p>
            <p>Diaz, Robert, Marissa Largo, and Fritz Pino. &ldquo;Diasporic Intimacies : Queer Filipinos and&nbsp;Canadian Imaginaries.&rdquo; Evanston, Illinois: Northwestern University Press, 2018. Print.</p>
            <p>Farrales, May. &ldquo;Repurposing Beauty Pageants: The Colonial Geographies of Filipina Pageants in Canada.&rdquo; Environment and planning. D, Society &amp; space 37.1 (2019): 46&ndash;64. Web.</p>
            <p>Freire, P. Pedagogy of the oppressed. New York: Continuum, 2000.</p>
            <p>Go, Matthew C, and Dada Docot. &ldquo;Fire and Fear: Rapid Cremations in the Philippines Amidst COVID-19.&rdquo; Forensic Science International: Synergy 3 (2021): 100132&ndash;100132. Web.</p>
            <p>Isaac, Allan Punzalan. <em>Filipino Time: Affective Worlds and Contracted Labor</em>, New York, USA: Fordham University Press, 2021.</p>
            <p>Largo, Marissa. &ldquo;Transnational Kinship, Diasporic Mourning and Belonging in the Canadian Animation World: The Moving Images of Leslie Supnet&rsquo;s Gains + Losses.&rdquo; <em>Topia&nbsp;</em><em>(Montreal)</em> 38 (2017):
              123&ndash;133. Web.</p>
            <p>Manalansan, Martin F., and Augusto Fauni Espiritu, editors. <em>Filipino Studies: Palimpsests of&nbsp;</em><em>Nation and Diaspora</em>. New York University Press, 2016.</p>
            <p>Mecija, Casey. &ldquo;Skin as Ecstatic Surface: Listening to Queer Diaspora in the Work of Patrick Cruz.&rdquo; Journal of Canadian studies 54.2 (2020): 508&ndash;525. Web.</p>
            <p>Pino, Fritz, et al., editors. <em>Diasporic Intimacies: Queer Filipinos and Canadian Imaginaries</em>. Northwestern University Press, 2018.</p>
            <p>Tungohan, Ethel. &ldquo;Reconceptualizing Motherhood, Reconceptualizing Resistance: Migrant Domestic Workers, Transnational Hyper-Maternalism and Activism.&rdquo; <em>International&nbsp;</em><em>Feminist Journal of Politics</em>, vol.
              15, no. 1, 2013, pp. 39-57.</p>
          </template>
        </V-accordion>
      </template>

    </div>
  </div>

</div>
</template>

<script>
import Vaccordion from 'vue-nuxt-accordion';

export default {
  name: 'IndexPage',
  components: {
    'V-accordion': Vaccordion
  },
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
body {
    background: #ffffff;
}
img {
    width: 100%;
}
</style>
