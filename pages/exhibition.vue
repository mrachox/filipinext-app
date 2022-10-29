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

  <div class="main-content px-3 py-2">
    <div class="row mt-5">
      <h1 class="placeholder" v-html="posts[7].title"></h1>

      <div class="col-md-6 col-lg-6 col-sm-12">
        <img style="width: 100%" src="~/assets/img/xmarksig.jpeg" alt="X Marks the Spot">
      </div>

      <div class="col-md-6 col-lg-6 col-sm-12">
        <img style="width: 100%" src="~/assets/img/xmarkslogo.jpeg" alt="X Marks the Spot">        
      </div>

      <div class="description">
        <br>
        <h2><strong>X Marks the Spot: Filipinx Futurities</strong></h2>
        <p><strong>Gales Gallery - 105 ACW (Accolade West Building) | York University</strong></p>
        <p><strong>July 13</strong><strong>th</strong><strong> &ndash; July 22</strong><strong>nd</strong><strong>, 2022</strong></p>
        <p><strong>Opening Reception: Thursday, July 14</strong><strong>th</strong><strong>, 4:30 &ndash; 6:30pm</strong></p>
        <p><strong>Artists:<br>Patrick Cruz X Excel Garay</strong></p>
        <p><strong>Julius Poncelet Manapul X John Ephraim Velasco</strong></p>
        <p><strong>Ella Gonzales X Revill Villanueva</strong></p>
        <p><strong>Curated by Marissa Largo</strong></p>


        <!-- <div class="row mb-1">
          <div class="col-md-3">
            <img src="~/assets/img/visarthist.png" alt="X Marks the Spot">

          </div>
        </div> -->


      </div>

    </div>
    <hr>

    <div class="row">
      <div class="col-md-12">
        <p>Curated by Dr. Marissa Largo, scholar of Asian diasporic contemporary art, <strong><em>X Marks the Spot</em></strong> takes the <em>X</em> in &ldquo;Filipinx&rdquo; as a theoretical and methodological intervention in curation. The X signals an intergenerational relationality &ndash; a sort of &ldquo;call and response&rdquo; &ndash; between recognized and rising practitioners working on Turtle Island that speaks to the legacies, influences, and transformations of Filipinx visual art in last decade. These relationalities generously explore themes such as spiritual healing and hauntings (Cruz x Garay), queer recuperations of colonial gazes and consumerist desire (Manapul x Velasco), and migration, movement, and transcendence (Gonzales x Villanueva). Marking &ldquo;the spot&rdquo; identifies our particular moment in time and space that gives rise to aesthetic possibilities that imagine and embody diasporic Filipinx subjectivity. They transcend nationhood, normativity, capitalist aspirations, and colonial temporality. These investigations take form through sculpture, painting, video, and photocollage and propose alternative engagements with space, place, materiality, selfhood, and community that defy modernism&rsquo;s limiting ideologies. Beyond identitarian politics, <strong><em>X Marks the Spot</em></strong><em>, </em>gestures to the multifarious ways in which diasporic Filipinx artists invent aesthetic futurities as an emancipatory practice.
          <br/>
        </p>

        <hr>

        <img style="width: 100%; height: auto;" src="~/assets/img/artists.jpeg" alt="X Marks the Spot">
        <p>&nbsp;</p>
      </div>

      <div class="col-md-6">
        <p><strong>Patrick Cruz </strong>(He/Him) is an artist, organizer and educator born in Quezon City, Philippines. Cruz studied painting at the University of the Philippines, Diliman and holds a Master of Fine Arts from the University of
          Guelph,
          a certificate in Pochinko clowning and a Bachelor of Fine Arts from Emily Carr University of Art + Design. Cruz is a co-founding member of Kamias Special Projects (KSP) a curatorial collective that hosts the Kamias Triennial in his
          hometown
          of Quezon City. His practice is informed by the intersections of folk spirituality, diasporic aesthetics, cultural hybridity, and the project of decolonization. Cruz is an Assistant Professor at the Department of Arts, Culture and
          Media at
          the University of Toronto Scarborough. <a href="http://www.patrickcruz.org">www.patrickcruz.org</a>| <a href="http://www.kamiasspecialprojects.com">www.kamiasspecialprojects.com</a></p>
      </div>

      <div class="col-md-6">
          <p><strong>Excel Garay</strong> (They/She) is an expanded-media painter, community worker, and curator. Garay&rsquo;s work is informed by prismatic contradictory experiences they continue to have as a transgender diasporic-settler
            currently
            occupying Mi'kma&rsquo;ki territory in Kjipuktuk, Eskikewa&rsquo;kik (Halifax, Nova Scotia). They graduated with a BA in Art History and BFA in Fine Arts from NSCAD University in 2022. They are&nbsp;the recipient of the RBC Emerging
            BIPOC
            Artist Award in 2021. Hauntology and Queer Phenomenology under a necropolitical lens foregrounds their practice. Garay&rsquo;s artistic practice&nbsp;materially manifest as paintings, immersive installations, and interdisciplinary
            assemblage.&nbsp;</p>
      </div>

    </div>

      <hr>
      <div class="row">

      <div class="col-md-6">
        <p><strong>Ella Gonzales</strong> (She/Her) is a Filipina-Canadian artist working between painting and Computer-Aided Design programs, as led by her interest in space making. Her paintings and installations are inspired by narratives of
          migration that inform the Filipino Diaspora. She has shown work with Galerie Nicolas Robert (Toronto), the plumb (Toronto), Patel Brown (Toronto), Modern Fuel Artist-Run Centre (Kingston), and Zalucky Contemporary (Toronto). Gonzales
          holds a
          Master of Fine Arts Degree in Studio Art from the University of Guelph and was the recent recipient of the 2021 Nancy Petry Award in painting.&nbsp;gonzalesella.com Instagram: @ellaggonzales&nbsp;</p>
      </div>

      <div class="col-md-6">
        <p><strong>Julius Poncelet Manapul</strong> (They/Them, b. 1980 Manila, Philippines) immigrated to Canada in 1990 and identifies as a queer migrant Filipinx artist of Ilocano ancestry. In 2009, they completed BFA at OCAD and MFA (U of
          T) in
          2013.&nbsp;Over the last decade, Julius P. Manapul has exhibited across North America and Europe. They had held positions as Associate Chair of Contemporary Drawing &amp; Painting and are currently an assistant professor in the
          Faculty of
          Arts at OCADU.&nbsp;Through research-based art practice, Julius Poncelet Manapul examines eternal displacement, complicated by colonialism, sexual identity, diasporic bodies, global identity construction, and the Eurocentric Western
          hegemony.
          Focusing on the hybrid nature of Filipinx culture through post-colonial realities, as well as through the gaze of queer identities as taxonomy, they study narratives specific to diasporic queer bodies; the loss of motherlands,
          feelings of
          belonging as a consequence of the colonial pedagogy and imperial power.&nbsp;<a href="http://www.juliusponceletmanapul.com">www.juliusponceletmanapul.com</a>&nbsp;</p>
      </div>

    </div>

      <hr>
      <div class="row">

      <div class="col-md-6">
        <p><strong>John Ephraim Velasco</strong> (He/Him, b. 2001 Philippines) is currently a Visual Arts major at York University. He is diasporic Filipinx illustrator and interdisciplinary artist.&nbsp;Ephraim&rsquo;s mediums through his
          artistry are
          mostly composed of mixed media, digital drawings, collages, drawing and painting. Through a vibrant and energetic style, he explores people and portraitures, examining their role in popular culture, mass media, and the constantly
          changing
          landscape of social media. He mostly conveys the denial of labels and expectations of gender and sexuality through visualizations of the human subject. As a non-Western creative force, he expresses his longing of his Philippine
          heritage using
          cultural designs and creating a hybrid of this along different imageries reminiscent to material commodity.&nbsp;His philosophy creating his works is to empower self-confidence through the human subject and propel them to their full
          potential.&nbsp;Instagram: @flaming.hot.papi&nbsp;</p>
      </div>

      <div class="col-md-6">
        <p><strong>Revill Villanueva</strong> (He/Him) is a Filipino-Canadian visual artist whose works explore the synthesization of modern technology, futuristic aesthetics, along with incorporating themes and concepts from his Filipino
          culture.
          Villanueva was born in Saudi Arabia in the year 2000, raised in the Philippines since 2007, and immigrated to Canada in 2013. Villanueva's migration to different countries results in a feeling of alienation to a new world. Therefore,
          he uses
          science fiction and futuristic visual qualities as a form of storytelling to resemble his experience of being an outsider. In addition, Villanueva embraces the usage of both classical&nbsp;and high technology in his creative practice
          to
          reveal the unification between the obsolete and the contemporary. He is currently an Undergraduate BFA Special Honours Visual Arts Major&nbsp;at York University. He was recently a recipient of the 2022 Dean&rsquo;s Purchase Award,
          Willowdale
          Painting Award, G44 Award, and Art History Honorarium Award at York University&rsquo;s Visual Arts and Art History Open House. Instagram: @revillvillanueva&nbsp;</p>
      </div>

    </div>

      <hr>




      <!-- <template>
        <V-accordion>
          <template v-slot:title>
            <h2>
              Artists
            </h2>
          </template>
          <template v-slot:content>
            <div class="artists">
              <p><img class="artist" src="~/assets/img/cruz.jpg" alt="cruz">
                <strong>Patrick Cruz </strong>(He/Him) is an artist, organizer and educator born in Quezon City, Philippines. Cruz studied painting at the University of the Philippines, Diliman and holds a Master of Fine Arts from the University of
                Guelph,
                a certificate in Pochinko clowning and a Bachelor of Fine Arts from Emily Carr University of Art + Design. Cruz is a co-founding member of Kamias Special Projects (KSP) a curatorial collective that hosts the Kamias Triennial in his
                hometown
                of Quezon City. His practice is informed by the intersections of folk spirituality, diasporic aesthetics, cultural hybridity, and the project of decolonization. Cruz is an Assistant Professor at the Department of Arts, Culture and
                Media at
                the University of Toronto Scarborough. <a href="http://www.patrickcruz.org">www.patrickcruz.org</a>| <a href="http://www.kamiasspecialprojects.com">www.kamiasspecialprojects.com</a></p>
              <p><img class="artist" src="~/assets/img/garay.jpg" alt="garay"><strong>Excel Garay</strong> (They/She) is an expanded-media painter, community worker, and curator. Garay&rsquo;s work is informed by prismatic contradictory experiences they continue to have as a transgender diasporic-settler
                currently
                occupying Mi'kma&rsquo;ki territory in Kjipuktuk, Eskikewa&rsquo;kik (Halifax, Nova Scotia). They graduated with a BA in Art History and BFA in Fine Arts from NSCAD University in 2022. They are&nbsp;the recipient of the RBC Emerging
                BIPOC
                Artist Award in 2021. Hauntology and Queer Phenomenology under a necropolitical lens foregrounds their practice. Garay&rsquo;s artistic practice&nbsp;materially manifest as paintings, immersive installations, and interdisciplinary
                assemblage.&nbsp;</p>
            </div>

            <div class="artists">
              <p><img class="artist" src="~/assets/img/gonzales.jpeg" alt="gonzales"><strong>Ella Gonzales</strong> (She/Her) is a Filipina-Canadian artist working between painting and Computer-Aided Design programs, as led by her interest in space making. Her paintings and installations are inspired by narratives of
                migration that inform the Filipino Diaspora. She has shown work with Galerie Nicolas Robert (Toronto), the plumb (Toronto), Patel Brown (Toronto), Modern Fuel Artist-Run Centre (Kingston), and Zalucky Contemporary (Toronto). Gonzales
                holds a
                Master of Fine Arts Degree in Studio Art from the University of Guelph and was the recent recipient of the 2021 Nancy Petry Award in painting.&nbsp;gonzalesella.com Instagram: @ellaggonzales&nbsp;</p>
              <p><img class="artist" src="~/assets/img/manapul.jpg" alt="manapul"><strong>Julius Poncelet Manapul</strong> (They/Them, b. 1980 Manila, Philippines) immigrated to Canada in 1990 and identifies as a queer migrant Filipinx artist of Ilocano ancestry. In 2009, they completed BFA at OCAD and MFA (U of
                T) in
                2013.&nbsp;Over the last decade, Julius P. Manapul has exhibited across North America and Europe. They had held positions as Associate Chair of Contemporary Drawing &amp; Painting and are currently an assistant professor in the
                Faculty of
                Arts at OCADU.&nbsp;Through research-based art practice, Julius Poncelet Manapul examines eternal displacement, complicated by colonialism, sexual identity, diasporic bodies, global identity construction, and the Eurocentric Western
                hegemony.
                Focusing on the hybrid nature of Filipinx culture through post-colonial realities, as well as through the gaze of queer identities as taxonomy, they study narratives specific to diasporic queer bodies; the loss of motherlands,
                feelings of
                belonging as a consequence of the colonial pedagogy and imperial power.&nbsp;<a href="http://www.juliusponceletmanapul.com">www.juliusponceletmanapul.com</a>&nbsp;</p>
            </div>

            <div class="artists">
              <p><img class="artist" src="~/assets/img/velasco.jpg" alt="velasco"><strong>John Ephraim Velasco</strong> (He/Him, b. 2001 Philippines) is currently a Visual Arts major at York University. He is diasporic Filipinx illustrator and interdisciplinary artist.&nbsp;Ephraim&rsquo;s mediums through his
                artistry are
                mostly composed of mixed media, digital drawings, collages, drawing and painting. Through a vibrant and energetic style, he explores people and portraitures, examining their role in popular culture, mass media, and the constantly
                changing
                landscape of social media. He mostly conveys the denial of labels and expectations of gender and sexuality through visualizations of the human subject. As a non-Western creative force, he expresses his longing of his Philippine
                heritage using
                cultural designs and creating a hybrid of this along different imageries reminiscent to material commodity.&nbsp;His philosophy creating his works is to empower self-confidence through the human subject and propel them to their full
                potential.&nbsp;Instagram: @flaming.hot.papi&nbsp;</p>
              <p><img class="artist" src="~/assets/img/villanueva.jpg" alt="villanueva"><strong>Revill Villanueva</strong> (He/Him) is a Filipino-Canadian visual artist whose works explore the synthesization of modern technology, futuristic aesthetics, along with incorporating themes and concepts from his Filipino
                culture.
                Villanueva was born in Saudi Arabia in the year 2000, raised in the Philippines since 2007, and immigrated to Canada in 2013. Villanueva's migration to different countries results in a feeling of alienation to a new world. Therefore,
                he uses
                science fiction and futuristic visual qualities as a form of storytelling to resemble his experience of being an outsider. In addition, Villanueva embraces the usage of both classical&nbsp;and high technology in his creative practice
                to
                reveal the unification between the obsolete and the contemporary. He is currently an Undergraduate BFA Special Honours Visual Arts Major&nbsp;at York University. He was recently a recipient of the 2022 Dean&rsquo;s Purchase Award,
                Willowdale
                Painting Award, G44 Award, and Art History Honorarium Award at York University&rsquo;s Visual Arts and Art History Open House. Instagram: @revillvillanueva&nbsp;</p>
            </div>
          </template>
        </V-accordion>
      </template> -->

      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>
              Curator
            </h2>
          </template>
          <template v-slot:content>
            <div class="artists">
              <p><img class="artist" src="~/assets/img/largo.jpg" alt="largo"><strong>Dr. Marissa Largo</strong> (She/Her) is an assistant professor in Creative Technologies at York University. She is researcher, artist, curator, and educator whose work focuses on the intersections of community
                engagement, race,
                gender and Asian diasporic cultural production. Her forthcoming book,&nbsp;<em>Unsettling Imaginaries: Filipinx Contemporary Artists in Canada </em>(University of Washington Press)&nbsp;examines the work and oral histories of artists
                who
                imagine Filipinx subjectivity beyond colonial logics. She is co-editor of <em>Diasporic Intimacies: Queer Filipinos and Canadian Imaginaries</em> (Northwestern University Press, 2017) and since 2018, she has served as the Canada Area
                Editor
                of the Journal of Asian Diasporic Visual Cultures and the Americas (ADVA). Her projects have been presented in venues and events across Canada, such as the Varley Art Gallery of Markham (2021), A Space Gallery (2017 &amp; 2012), Royal
                Ontario
                Museum (2015), WorldPride Toronto (2014), Nuit Blanche in Toronto (2019, 2018, 2012 and 2009), and MAI (Montr&eacute;al, arts interculturels) (2007). <a href="http://www.marissalargo.com">www.marissalargo.com</a></p>
            </div>

          </template>
        </V-accordion>
      </template>
      <br>
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
.description {
  width: 100%;
    h2, p {
        text-align: center;
    }

    img {
      width: 100%;
    }
}

.artist {
    width: 50%;
    object-fit: contain;
    float: left;
    padding-right: 1em;
}
</style>
