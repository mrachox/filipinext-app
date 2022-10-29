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
    <div class="my-5">
      <h1 class="placeholder" v-html="posts[3].title"></h1>
      <p><strong>Day 1:&nbsp;</strong><strong>Wednesday, July 13</strong><strong>th</strong><strong>, 8:30-4 pm&nbsp;</strong></p>
      <table>
        <tbody>
          <tr>
            <td>
              <p><strong>8:30 &ndash; 9:00 am</strong></p>
            </td>
            <td>
              <p>Registration, coffee and tea, meet and greet<br/>Media release forms</p>
            </td>
          </tr>
          <tr>
            <td>
              <p><strong>9:00 &ndash; 9:30 am</strong></p>
            </td>
            <td>
              <p>Welcome, land acknowledgement, and opening remarks. Drs. Mecija, Catungal, and Largo</p>
            </td>
          </tr>
          <tr>
            <td>
              <p><strong>9:30 &ndash; 10:30 am</strong></p>
            </td>
            <td>
              <p><strong><a href="/roundtable#opening">Opening Plenary: Care Work in and Beyond the Pandemic</a></strong> with Kara Manso, Martha Ocampo, Anna Balagtas and Dr. Conely de Leon</p>
            </td>
          </tr>
          <tr>
            <td>
              <p><strong>10:30 &ndash; 10:45 am</strong></p>
            </td>
            <td>
              <p>Break/Snack</p>
            </td>
          </tr>
          <tr>
            <td>
              <p><strong>10:45 &ndash; 12:00 pm</strong></p>
            </td>
            <td>
              <p><strong>Roundtable: <a href="/roundtable#healthlabour">Labour and Health # 1</a></strong>: <br>Moderator: Dr. Valerie Damasco<br> Presenters: Dr. Valerie Damasco, Jenna Blower, Darlyne Bautista, Dr. Conely de Leon</p>
            </td>
          </tr>
          <tr>
            <td>
              <p><strong>12:00 &ndash; 1:00 pm</strong></p>
            </td>
            <td>
              <p>Lunch</p>
            </td>
          </tr>
          <tr>
            <td>
              <p><strong>1:00 &ndash; 2:30 pm</strong></p>
            </td>
            <td>
              <p><strong>Roundtable: <a href="/roundtable#faithreligion">Faith and Religion</a></strong>: <br>Moderator: Dr. Lisa Davidson <br>
                Presenters: Dr. Lisa Davidson, Kim Joshua Salcedo, Aileen Santiago, Drexler Ortiz, Kevin Laxamana.</p>
            </td>
          </tr>
          <tr>
            <td>
              <p><strong>2:30 &ndash; 2:45 pm</strong></p>
            </td>
            <td>
              <p>Break</p>
            </td>
          </tr>
          <tr>
            <td><p><strong>2:45 &ndash; 3:45pm</strong></p></td>
            <td><p><strong>Roundtable: <a href="/roundtable#nature">Nature and Ecologies</a></strong>: <br>Moderator: Dr. JP Catungal <br>
              Presenters: Dr. May Farrales, Dr. Ashley Caranto Morford, Christine Anonuevo</p></td>
          </tr>
          <tr>
            <td><p><strong>3:45 &ndash; 4:00pm</strong></p></td>
            <td><p>Closing remarks (+ Day 1 Group Photo)<br>Dr. JP Catungal</p></td>
          </tr>
        </tbody>
      </table>

      <p>7:00-9:00 pm <strong>Off Campus Event:&nbsp;</strong><br><strong>FilipiNEXT presents </strong><strong><em>Topline</em></strong><strong>: Filipinx Diaspora and Sonic Aspirations in the City&nbsp;</strong></p>
      <p>Screening, Q & A, and live performances by creator, Romeo Candido, and lead actor, Cyrena Fiel.
Special performance from Alexis Estropia and Gregory Dy Sun (Filipino Student’s Association at York)</p>
      <p>Innis Town Hall<br>2 Sussex Ave., Toronto.</p>

      <hr>

      <p><strong>Day 2: Thursday, July 14, 8:30-4 pm</strong></p>
      <table>
        <tbody>
          <tr>
            <td>
              <p><strong>8:30 &ndash; 9:00 am</strong></p>
            </td>
            <td>
              <p>Registration, coffee/tea <br>Media release forms</p>
            </td>
          </tr>
          <tr>
            <td>
              <p><strong>9:00 &ndash; 9:30 am</strong></p>
            </td>
            <td>
              <p>Land Acknowledgement, refreshments, Day 1 reflections</p>
            </td>
          </tr>
          <tr>
            <td><p><strong>9:30 &ndash; 10:45am</strong></p></td>
            <td><p><strong>Roundtable: <a href="/roundtable#healthlabour">Labour and Health #2</a></strong>: <br>Moderator: Dr. Ethel Tungohan <br>
Presenters: Dr. Ethel Tungohan, PJ Javier, Dani Magsumbol, Dr. JP Catungal</p></td>
          </tr>
          <tr>
            <td>
              <p><strong>10:45 &ndash; 11:00 am</strong></p>
            </td>
            <td>
              <p>Break/Snack</p>
            </td>
          </tr>
          <tr>
            <td>
              <p><strong>11:00 &ndash; 12:15 pm</strong></p>
            </td>
            <td>
              <p><strong>Roundtable: <a href="/roundtable#healthlabour">Nature and Ecologies</a></strong>: <br>Moderator: Dr. JP Catungal<br>
Presenters: with Dr. Dennis Gupa, Katherine Achacoso, Ariel Dela Cruz, Liza Constantino</p>
            </td>
          </tr>
          <tr>
            <td>
              <p><strong>12:15 &ndash; 1:15 pm</strong></p>
            </td>
            <td>
              <p>Lunch</p>
            </td>
          </tr>
          <tr>
            <td>
              <p><strong>1:15pm &ndash; 2:45 pm</strong></p>
            </td>
            <td>
              <p><strong>Roundtable: <a href="/roundtable#culturalprod">Cultural Production</a></strong>: <br>Moderator: Dr. Marissa Largo
                <br>Presenters: Dr. Casey Mecija, Dr. Marissa Largo, Excel Garay, Mel Racho, Karla Commanda</p>
            </td>
          </tr>
          <tr>
            <td>
              <p><strong>2:45 &ndash; 3:00 pm</strong></p>
            </td>
            <td>
              <p>Break</p>
            </td>
          </tr>
          <tr>
            <td>
              <p><strong>3:00 &ndash; 4:00 pm</strong></p>
            </td>
            <td>
              <p><strong><a href="/roundtable#closing">Closing Plenary</a></strong>: Intergenerational Dialogs in Filipinx Studies in Canada <br>Moderator: Dr. May Farrales<br>
Panelists: Katherine Achacoso, Ariel Dela Cruz, Christine Anonuevo, Dr. JP Catungal, Dr. Marissa Largo, Dr. Lisa Davidson <br/>
Day 2 Group Photo
</p>
            </td>
          </tr>
        </tbody>
      </table>
      <p><strong>Opening Reception</strong><strong><em>:</em></strong> <strong><em>X Marks the Spot</em></strong></p>
      <p>4:30-6:30pm</p>
      <p>Gales Gallery - 105 ACW (Accolade West Building), York University.</p>
      <p>Curated by: Dr. Marissa Largo</p>

      <hr>

      <p><strong>Day 3: Graduate Workshop</strong>&nbsp;</p>
      <table>
        <tbody>
          <tr>
            <td>
              <p><strong>9:00 &ndash; 9:30 am</strong></p>
            </td>
            <td>
              <p> Meet and greet, refreshments</p>
            </td>
          </tr>
          <tr>
            <td>
              <p><strong>9:30 &ndash; 10:45am</strong></p>
            </td>
            <td>
              <p>1. Check-in circles (in small groups)<br>
                2. Report back <br>
                3. Breath work and presentation from the Pahinga Collective</p>
            </td>
          </tr>
          <tr>
            <td><p><strong>10:45 &ndash; 11:00am</strong></p></td>
            <td><p>Break</p></td>
          </tr>
          <tr>
            <td>
              <p><strong>11:00 &ndash; 12:00pm</strong></p>
            </td>
            <td>
              <p>Rotating Huddles (x2): “Things you need to know that no one tells you”<br>
                1. <strong>Community-engaged work</strong> (ethics, logistics, philosophy) - Ethel<br>
                2. <strong>Navigating Institutions</strong>  – PD, Scholarships, funding, ethics, IRB process </p>
            </td>
          </tr>
          <tr>
            <td>
              <p><strong>12:00 &ndash; 1:00pm</strong></p>
            </td>
            <td>
              <p>Lunch</p>
            </td>
          </tr>
          <tr>
            <td>
              <p><strong>1:00 &ndash; 2:00pm</strong></p>
            </td>
            <td>
              <p>Rotating Huddles (x2): “Things you need to know that no one tells you”<br>
                3. <strong>Life After and Outside of Graduate Studies</strong> - Marissa <br>
                4. <strong>Making space and time for care</strong> - Conely </p>
            </td>
          </tr>
          <tr>
            <td><p><strong>2:00 &ndash; 3:00pm</strong></p>
            </td>
            <td><p>Interrogating the NEXT…<br>
            Prompts:<br>
            What is your take away from the 3-day workshop?<br>
            What is your next step?<br>
            What is our next step?</p>
            </td>
          </tr>
        </tbody>
      </table>
      <br>
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
table {
    width: 100%;
    font-size: 0.55em;
    margin-bottom: 1em;
    strong {
        font-weight: bold;
    }
    td {
        padding: 0.65em;
    }
    tr:nth-child(odd) {
        background-color: #CAC4AC;
    }
    tr:nth-child(even) {
        background-color: #CDB298;
    }
}
</style>
