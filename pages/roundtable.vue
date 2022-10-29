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
      <h1 class="placeholder" v-html="posts[4].title"></h1>

      <h3 id="opening">Opening Plenary</h3>
      <p>In this opening plenary, long-time community activists, Martha Ocampo, Kara Manso, and queer femme radical birthworker, Anna Balagtas, come together to reflect on community histories of migrant care activism, transformative queer care, and decolonizing birthwork. In conversation with Conely de Leon, they discuss defining moments that mobilized the Filipina/x/o diasporic community to action - from People Power to the 2022 Philippine election of Marcos-Duterte, and the overturning of Roe v. Wade. We take time to pay tribute to beloved friends and mentors, and together, shed light on the enduring importance of intergenerational community care, mutual aid, abolition work, and art and performance in and beyond the pandemic. The plenary closes with reflections, questions, and aspirations for a new chapter of FilipiNEXT.</p>
      <h3 id="healthlabour">Health and Labour</h3>
      <p>In this two-part panel, speakers cover a robust range of topics related to the broader themes of health and labour. In Part One, panelists invite us to question the ways in which the mental health and well-being of Filipina/x/o children,
        youth, care workers, and community leaders have been addressed prior to and throughout COVID-19. For example, Hilario speaks to the role of equity-oriented health services in supporting young people's mental health, while Damasco&rsquo;s work
        addresses the structural, social, and cultural determinants of health that may impact the well-being of frontline healthcare workers. Further deepening this discussion on health and well-being is Blower&rsquo;s research on the corporeality of
        migration and the psychological and physical injuries that care workers accrue over time.</p>
      <p>In Part Two, panelists focus explicitly on challenging existing narratives and perceptions of gendered and racialized labour. For example, Bautista contests masculinist and conservative attitudes at work within the Filipina/x/o community in
        *Canada, reading gender, labour and diaspora into her analysis of the roles that community leaders play in the reproduction of gendered and racialized work. Panelists&rsquo; particular attention to the temporal dimensions of labour invite us
        to consider what work lies ahead of us. For example, Tungohan reflects on how the temporal uncertainties facing Filipinx migrant workers affect their everyday experiences of &lsquo;belonging&rsquo;, while also, paradoxically, serving as a
        catalyst for activist endeavours. Magsumbol addresses how labour is perceived through affective time: factoring in the time (zone) difference between family members, the years lost between parting and meeting, and the ways in which love is
        communicated across time and space. Enlivening this intergenerational conversation is Javier&rsquo;s research, which contests white cisheteronormative theories of childhood and childhood innocence as it relates to the children of former
        live-in caregivers. Together, these presentations not only build on the work produced in <em>Filipina/x/os in Canada: Disturbing Invisibility</em> (2012) a decade ago, but also signal critical shifts in our growing understanding of labour and
        health issues today</p>
      <h3 id="faithreligion">Religion and Faith</h3>
      <p><em>Religion and Faith,</em> brings together community religious leaders, activists, and scholars to discuss Filipinx religious identities past, present and future. Although Catholicism is usually representated as the religious majority
        among Filipinx in Canada and elsewhere, contributors offer a timely and critical perspective on the variety of lived religions that have come to shape Filipinx communities. Many Filipinx are looking to religion for alternative modalities to
        think and reflect on their experiences in Canada. The aim of this panel is two-fold: first, to identify and intervene in the historical and contemporary erasure of Filipinx religious identities, affiliations, and political and social
        networking that have come to shape the uneven processes in becoming and being Canadian; and second, to consider the ways that Filipinx Christians, Catholics and Muslims make sense of their transnational mobility, labour experiences, and
        integration into Canada that allow for an imagination and futurity of Filipinx religiosities.&nbsp;</p>
      <h3 id="nature">Nature and Ecologies</h3>
      <p>What might be gained, analytically and politically, if Filipinx Canadian studies considers the implications of hydromorphic, geomorphic, territorial and environmental issues and processes on Filipinx Canadian histories and communities?
        Participants in this roundtable variously examine the natures, ecologies and politics of Filipinx-ness by attending to rocks, waterways, climate changes, resources and land. They do so through conceptual tools that expand Filipinx Canadian
        studies itself, among them applied theatre, socio-spatial analysis, eco-criticism and oceanic methods. Together, they invite Filipinx Canadian studies to assess global ecological and environmental politics as issues of significance for a more
        capacious Filipinx Studies in Canada and beyond.</p>
      <h3 id="culturalprod">Cultural Production</h3>
      <p>This roundtable examines the role of cultural production as a conduit of Filipinx diasporic expression. Participants will discuss how digital, sonic, performative, and literary production can animate the complex entanglements of gender,
        race, class, and citizenship. Some questions that will guide our conversation are: What does cultural production, as both conceptual and material possibility, reveal about our understandings of Filipinx diaspora in Canada? How have art and
        other modes of symbolic expression by Filipinx people grappled with injustice, especially within the context of COVID-19 and related anti-Asian racism? How can we make links between the multiple temporalities of Filipinx diasporic cultural
        imaginaries?</p>
      <h3 id="closing">Keynote (Closing Plenary):</h3>
      <p>This roundtable discussion invites emerging and junior Filipinx scholars to collectively revisit and reflect on the edited the book, <em>Filipinos in Canada: Disturbing Invisibility </em>(University of Toronto Press, 2012). Over the past
        decade, the book has offered a steppingstone for students to engage in research on the Filipinx diaspora. The panel aims to allow emerging Filipinx scholars, who have taken up the questions and challenges the book offered, to be in
        conversation with scholars involved in the making of <em>Filipinos in Canada</em>. Building on the work that the book has generated, this intergenerational dialogue will reflect on the question of where a critical Filipinx studies in
        so-called Canada and politics needs to go in the colonial and capitalist present.</p>
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
