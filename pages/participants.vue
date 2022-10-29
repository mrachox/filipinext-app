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
      <h1 class="placeholder" v-html="posts[5].title"></h1>
      <p>&nbsp;</p>

      <!--///PRESENTERS/////////////////////////////////////////-->

      <p><strong class="presenter">Katherine Achacoso</strong></p>
      <!-- <p>Location: Canada and Philippines</p> -->
      <p>Affiliation: Department of American Studies, University of Hawaiʻi at Mānoa</p>
      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>Undermining Canadian Empire: On Dangerously Remembering Diasporic Filipino Canadian Mappings of Lands, Rocks, and Peoples that Move</h2>
          </template>
          <template v-slot:content>
            <p>What kinds of stories do rocks (re)member? What diasporic and Oceanic routes do they recount? What kinds of transnational, settler/colonial, and neoliberal violences get written in the materiality and ontology of rocks? What narratives
              of
              resistance and agency do rocks enact? How does our relationship to rocks (re)map new/old relationships to land and seas from the vantage point of the Philippine diaspora?</p>
            <p>This paper seeks to (re)member the stories and lives of rocks migrating from the Philippines to Canada (Turtle Island). It seeks to bear witness to the ongoing violence of the displacement of rocks vis-a-vis North American mining in
              Surigao
              (Mindanao). Through weaving together poetry and photography mined from the colonial archive, alongside oral histories conducted with Indigenous and non-Indigenous Philippine migrants forced to move as a result of disaster capitalism,
              this
              multi-media paper seeks to decenter geontopower (Povinelli) through (re)membering the agency, livelihood and resistance of rocks at home and in the diaspora. In doing so, this piece reflects on how turning towards the stories and sites
              of
              submerged archipelagos of extracted lands allow us to map alternative modes of sociality and social ecologies that critique and exceed (settler) capitalism. In addition, it considers how mapping the relationship between Canada and the
              Philippines gestures to the possibility of emerging &ldquo;constellations of co-resistance (Simpson)&rdquo; amongst (diasporic) Filipinos/x and Indigenous peoples in Canada and the Philippines.&nbsp;</p>
            <p><strong>Bio:</strong> Katherine Achacoso is a daughter of the Filipinx diaspora (Surigaonon/Boholano), raised on the unceded territories of the Haudenosaunee, Anishinaabe and Huron-Wendant confederacy in Tkaronto. She is a doctoral
              candidate
              in American Studies at the University of Hawaii at Manoa, where she teaches classes on American empire, Indigenous and Transnational Feminisms, Filipinx Studies, and Environmental Justice. Katherine also serves as co-chair of the Asian
              Settler Colonialism Caucus within the Association for Asian American Studies, and the president of the Hawaii American Studies Association. Her dissertation, Undermining Canadian Empire builds from a broader anti-colonial genealogy of
              resistance to Canadian settler capitalism and extractivism, to consider the radical possibilities of dangerously (re)membering transnational and diasporic Filipina/x critiques of Canadian resource extractive imaginaries that span Canada
              and
              the Philippines. Expanding the current literature emerging from Indigenous Feminisms and Critical Ecology Studies which emphasizes the gendered colonial logics underpinning Canada&rsquo;s mining empire, she considers how diasporic
              Filipina
              Canadian women (re)map our geographic understanding of the transnational reach of Canadian mining through embodied cartographies which (re)member the physical, spatial, and imaginative reach of Canada&rsquo;s mining infrastructure.</p>
          </template>
        </V-accordion>
      </template>

      <hr>

      <p><strong class="presenter">Anna Balagtas</strong></p>
      <!-- <p>Location: Canada/ Philippines</p> -->
      <p>Affiliation: Pocket Doula</p>
      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>
              Opening Plenary: Care Work in and Beyond the Pandemic
            </h2>
          </template>
          <template v-slot:content>
            <img class="bio" src="~/assets/img/blush.png" alt="Anna Balagtas">
            <p><strong>Bio:</strong> Kamusta! Ako si Anna Balagtas (she/her) and I'm a Queer + Pinay femme radical birthworker, educator, facilitator, energy worker, and pleasure advocate. I'm the founder of Pocket Doula and I support emerging
              birthworkers in radicalizing their practice through heart-centered mentorships, facilitations, and community organizing. My practice is housed under the decolonization of birthwork and transformative queer care. My deepest joys come
              from witnessing our communities thrive through community care, mutual aid, and abolition work.</p>

          </template>
        </V-accordion>
      </template>

      <hr>

      <p><strong class="presenter">Darlyne Bautista</strong></p>
      <!-- <p>Location:&nbsp;Canada</p> -->
      <p>Affiliation:&nbsp;University of Toronto</p>
      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>
              The politics of shoveling snow: Reading gender, labour, and diaspora in the Jon Reyes Twitter debacle
            </h2>
          </template>
          <template v-slot:content>
            <p>On January 8, 2022, Manitoba cabinet minister and Filipino Canadian Jon Reyes garnered international notoriety for a photo he shared of his wife shoveling their driveway after a 12-hour shift as a nurse. The post sparked outrage as it
              went
              viral with media and tabloid outlets picking up on the story to discuss gender roles, frontline workers, and the pandemic. As a Filipino Canadian, Reyes represents masculinist and conservative attitudes found within the Filipino
              Canadian
              community. As a governing politician, he also expresses the value placed on productivity versus that of the gendered and racialized labourer. How do these attitudes align with the feminization of care work in the diaspora? What role do
              Filipino Canadian leaders play in the process and implementation of gendered and racialized work? This presentation will offer an analysis via gender, labour, and diaspora studies.</p>
            <p><strong>Bio:</strong> Darlyne Bautista is a PhD student in Women and Gender Studies at the University of Toronto. Her current research is on transnational affect and inter-generational knowledge production among Winnipeg&rsquo;s early
              Filipino garment recruits (1968 to 1986). This research was awarded the SSHRC Canadian Graduate Scholarship-Doctoral in 2021.</p>
          </template>
        </V-accordion>
      </template>

      <hr>

      <p><strong class="presenter">Jenna Blower</strong></p>
      <!-- <p>Location:&nbsp;Canada</p> -->
      <p>Affiliation:&nbsp;York University</p>
      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>
              The corporeality of migration
            </h2>
          </template>
          <template v-slot:content>
            <p>This presentation is informed by the stories shared by Filipina elders, their family members, and participant observation conducted during my fieldwork. I reflect on how the journey of migration and care work over the life course marks
              one&rsquo;s body. My research acknowledges the diversity of forms of care and the multiple ways in which care is expressed. Caring is deeply embodied through a range of sensorial techniques that help caregivers attune their physical
              bodies
              and emotional selves to the people for whom they are caring.&nbsp;</p>
            <p>This presentation is informed by the stories shared by Filipina elders, their family members, and participant observation conducted during my fieldwork. I build on Strathern&rsquo;s (2020) notion of relations as elusive and attractive
              whereby people are drawn into relations with the things, beings, and entities that form their environment. The centrality of shifting social, political, and economic conditions that shape social relations among transnational families
              and over
              the life course informs my research. In observing physical ailments, experiences of poverty and generational trauma, the significance of migration and a career as a care worker shapes the health and well-being of an individual and their
              family. Attending to the psychological and physical injuries that accrue over time, this presentation will explore the corporeality of migration, care work, and its impact on the life course.&nbsp;</p>
            <p><strong>Bio:</strong> Jenna Blower is a Ph.D. candidate at York University in the Department of Social Anthropology. Jenna has an MA in Immigration and Settlement Studies from Ryerson University and previously worked at Cities of
              Migration
              where she contributed to the My City of Migration Diagnostic (MyCOM) Tool and the Immigrant Futures project. Jenna currently works as a Research Consultant for the Migration Research Division at the International Organization for
              Migration
              supporting the Word Migration Report series.&nbsp;</p>
          </template>
        </V-accordion>
      </template>

      <hr>

      <p><strong class="presenter">John Paul Catungal</strong></p>
      <!-- <p>Location: Canada</p> -->
      <p>Affiliation: Institute for Gender, Race, Sexuality and Social Justice, University of British Columbia</p>
      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>Community organizing as vernacular critique: Filipinx Canadian youth theorize educational abandonment&nbsp;</h2>
          </template>
          <template v-slot:content>
            <p>Drawing on community based participatory research with the Kababayan Academic Mentorship Program, this paper examines the phenomenon of educational abandonment, which names the institutionally sanctioned narrowing of possible futures
              for
              Filipinx Canadian youth through the racial organization of schooling. It does so with a focus on the education-focused organizing work of Filipinx Canadian youth in so-called Vancouver. As powerful, yet underappreciated, forms of
              vernacular
              critique, stories shared by Filipinx Canadian youth about their schooling experiences and their efforts to create culturally appropriate, peer-led supports testify to the consignment of Filipinx Canadian youth to futures of racially
              narrowed
              socio-economic opportunity. Quite importantly, their vernacular critique locates educational abandonment within a larger ecology of institutions that produce unequal racialized futures, among them education, immigration, labour,
              policing and
              the media. In the face of this institutional ecology of abandonment, organizing by Filipinx Canadian youth, along with their efforts to publicly share their stories, must thus be understood as a powerful form of agentive&nbsp;refusal.
            </p>
            <p><strong>Bio: </strong>Dr. JP Catungal is Assistant Professor in the Institute for Gender, Race, Sexuality and Social Justice and Interim Director of the Asian Canadian and Asian Migration Studies Program at the University of British
              Columbia. A queer, first-generation Filipinx Canadian settler living in unceded Coast Salish territories, JP is an interdisciplinary scholar trained in the nexus of critical human geography and intersectional feminist theorizing. His
              research, teaching and public facing work concern the community organizing and cultural production practices of migrant, racialized and LGBTQ+ communities, with particular interests in sexual health, education and social services. He
              approaches his work indebted to and in conversation with Filipinx and Asian diaspora studies and queer and trans of colour theorizing. JP was co-editor of the Filipinos in Canada: Disturbing Invisibility (2012, University of Toronto
              Press)
              and has served on the editorial collective of ACME: International Journal of Critical Geographies since August 2017.</p>
          </template>
        </V-accordion>
      </template>

      <hr>

      <p><strong class="presenter">Liza Constantino</strong></p>
      <!-- <p>Location: Canada/ Philippines</p> -->
      <p>Affiliation: York University</p>
      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>
              Kinesthetic Interventions: Dances in the 2022 Philippine Elections
            </h2>
          </template>
          <template v-slot:content>
            <p>Philippine Dance is a space that abounds with political intention&mdash;from the assertion and/or interrogation of ethnic and national identities (Aquino, Locsin, Villaruz) to meditations on one&rsquo;s relationship with religious
              hierarchies (Alcedo, Ness, Peterson) to physical education and the reinforcement of disciplinal (colonial) techniques (Gonzalves, Perillo). Dance permeates various political units&mdash;from the family, barangay, the region, and the
              nation as
              an imagined community. Imagining dance as a response to sociopolitical events, while foregrounding the overlap between movement as both &ldquo;civic&rdquo; and &ldquo;kinesthetic,&rdquo; I explore dances in the events leading up to the
              2022
              Philippine Presidential elections.&nbsp;<strong>Why has dance figured as such a visible part of community-led events? What do dances during elections tell us about bodies&rsquo; desire to move?</strong>&nbsp;To answer, I highlight
              the&nbsp;<em>visibility</em>&nbsp;of dance by surveying a selection of dances performed as part of the 2022 national elections. Collectively, I call these, &ldquo;election season dances.&rdquo; From this selection, I examine three
              recorded
              dance texts circulated through Twitter. Using the method of movement observation, I describe dances as I have witnessed online as a migrant worker and dance scholar in Toronto, Canada. Moreover, I suggest that these election season
              dances
              figure as strategic appeals to affect and to bodies&rsquo; desires to move as a collective&mdash;important components of Philippine performative traditions.&nbsp;</p>
            <p><strong>Bio:&nbsp;</strong></p>
            <p>Liza Constantino is a dance scholar enrolled at York University&rsquo;s PhD program in Dance Studies. Her present research revolves around the pole dance community in Metro Manila, which she has been part of since 2015. She has also
              taught
              literature in Ateneo de Manila University, where she completed her MA in Literary &amp; Cultural Studies.</p>
          </template>
        </V-accordion>
      </template>

      <hr>

      <p><strong class="presenter">Valerie Damasco</strong></p>
      <!-- <p>Location: Canada</p> -->
      <p>Affiliation: Ontario Institute for Studies in Education, University of Toronto&nbsp;</p>
      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>
              Problematizing the resilience of Filipino frontline healthcare workers in Canada during the COVID-19 pandemic
            </h2>
          </template>
          <template v-slot:content>
            <p>While a large proportion of Filipinos continue to work on the frontlines across various healthcare settings in Canada and in other countries during the COVID-19 pandemic, it remains unclear how they manage the stresses they experience
              in
              their jobs. Although these workers have been portrayed as resilient, this conceals health and mental health related issues, as well as unidentified workplace stresses, they may be experiencing. Furthermore, compounding pressures
              associated
              with the immigration process, such as adaptation, acculturation, and discrimination, for example, may also increase health disparities overall. This presentation discusses: (i) the structural, social, and cultural determinants of health
              that
              may impact the health, well-being, and work effectiveness of Filipino frontline healthcare workers; (ii) the coping strategies they employ; (iii) the supports they access and associated barriers; and (iv) the practices by which they are
              retained at these institutions.</p>
            <p><strong>Bio:</strong> Valerie G. Damasco is a Lecturer and Researcher at the University of Toronto. Her doctoral research focused on the migration of Filipino nurses who arrived in Canada from the Philippines and via the United States
              during
              the 1950s and 1960s. Currently, her current research explores how organizational healthcare policies in hospitals across Canada affect the work of racialized frontline healthcare workers. She is examining how individuals, communities,
              and
              institutions respond to health crises and inequities across local, transnational, and international contexts. In her work, she applies critical health education, participatory, and interdisciplinary approaches to examine how communities
              advocate and mobilize for equity in health, access health and related supports, strengthen capacity, and promote inclusion.</p>
          </template>
        </V-accordion>
      </template>

      <hr>

      <p><strong class="presenter">Lisa Davidson</strong></p>
      <!-- <p>Location: Canada</p> -->
      <p>Affiliation: York University</p>
      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>
              All in God&rsquo;s Time: Hope, Conviviality and Place Making among Filipino Canadian Protestants
            </h2>
          </template>
          <template v-slot:content>
            <p>This presentation centers on the religious lives of urban Filipino communities living in Toronto, Montreal, and Winnipeg to elucidate how Filipino Protestant congregations are working to create and sustain a sense of place, community,
              and
              belonging. Filipinx narratives of migration and integration into Canada are fraught due to a wide yet polarizing range of personal interpretations in becoming Canadian. Some Filipinx see their migration and downward class mobility in
              Canada
              as a political and Christian awakening while others, make sense of their migration and integration as God&rsquo;s divine plan for uplift into a better life in Canada. How are Filipinx Protestant communities carving out spaces that unify
              the
              diversity within their congregations? In this presentation, I will look to the kinds of programs Filipinx protestants are developing to support political and spiritual connections within their own communities with newly arrived
              immigrants,
              second and third generation Canadian Filipinos and mixed race Filipinos.&nbsp;</p>
            <p><strong>Bio:</strong> Lisa M. Davidson is an Assistant Professor, Teaching Stream, in the Department of Anthropology at York University. Her research focuses on intergenerational and interracial belonging in Filipino Protestant
              congregations
              in Canada. She is co editor and contributing author of Filipinos in Canada: Disturbing Invisibility (University of Toronto Press, 2012).</p>
          </template>
        </V-accordion>
      </template>
      <hr>

      <p><strong class="presenter">Conely de Leon</strong></p>
      <!-- <p>Location: Canada/ Philippines</p> -->
      <p>Affiliation: York University</p>
      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>
              Opening Plenary: Care Work in and Beyond the Pandemic
            </h2>
          </template>
          <template v-slot:content>
            <p><strong>Bio:&nbsp;</strong></p>
            <p>Conely de Leon is an Assistant Professor in the Department of Sociology at Toronto Metropolitan University. Dr. de Leon’s current work focuses on community care in
 addressing experiences of grief and loss among racialized migrant communities. Given this critical shift in focus, Dr. de Leon is also pursuing professional certification as a grief educator and counselor. Further, in response to heightened grief and loss
 during the pandemic, Dr. de Leon co-founded the Pahinga Collective with Filipina/x/o graduate students, community organizers, and service providers representing migrant, queer, and feminist grassroots organizations in Tkaronto. Through digital kwentuhan, soundscapes,
 and other forms of co-creation, the Pahinga Collective aims to contribute to embodied understandings of rest as a form of anti-colonial and anti-capitalist resistance, and healing justice.</p>
          </template>
        </V-accordion>
      </template>

      <hr>

      <p><strong class="presenter">Ariel Dela Cruz</strong></p>
      <!-- <p>Location: United States/Canada</p> -->
      <p>Affiliation: Cornell University&nbsp;</p>
      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>The Limits of Pamilya and Mourning: Queer Loss, Citizen-Making, and Carework in My Grandmother and I</h2>
          </template>
          <template v-slot:content>
            <p>An investigation of the legacies of the Foreign Domestics Movement and Live-In Caregiver Program in Canada rarely conceptualize carework through the perspectives of sexually excluded racialized youth, particularly queer children of
              Filipino/a caregivers. Using a visual and textual analysis, this paper explores the possibilities and limits of queer kinship in the Filipinx pamilya in Canada through the recording and text of the 1994 play, My Grandmother and I
              (Montreal,
              2016). By situating this play in a political moment in which the triangulation of HIV/AIDS, multiculturalism, and transnational migrant labour programs condition kinstillatory possibilities through processes of citizen-making, this
              paper
              explores how Dino and his Lola, the main characters of the play and video, forage new possibilities of intimacy through their kinship. I argue that these possibilities are constitutively restrained within and conditioned by the
              formation of
              the nuclear family and the political capacities of carework within the Filipinx home.&nbsp;</p>
            <p><strong>Bio:</strong> Ariel Dela Cruz (they/them and he/him) is a queer, nonbinary, trans Filipinx-Canadian community worker and current PhD student at Cornell University in the Department of Performing and Media Arts. Their current
              research
              operates at the intersection of care/work, performance studies, queer theory, Filipinx diasporic studies, and trans theory. His present research project conceptualizes care as both a mode of labour that informs the Filipinx-Canadian
              diaspora
              as well as a liberatory praxis enacted by transmasculine Filipinx people for survivance and world-making. They completed both their Honours Bachelor of Science and Master of Arts in Women and Gender Studies at the University of Toronto.
            </p>
          </template>
        </V-accordion>
      </template>

      <hr>

      <p><strong class="presenter">May Farrales</strong></p>
      <!-- <p>Location: Canada</p> -->
      <p>Affiliation: Geography and Gender, Sexuality, &amp; Women's Studies, Simon Fraser University</p>
      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>Queering Land and Labour: The Filipinx Diaspora in the Settler Colonial Racial Geographies of the North</h2>
          </template>
          <template v-slot:content>
            <p>&nbsp;In this paper, I trace the racial geographies contoured by the overlapping configurations of land and labour that condition both the Filipinx diaspora and the dispossession of Indigenous peoples in northern BC. I follow calls in
              Indigenous, Black, and critical race scholarship that push back against relying on the common land-labour dialect that tends to lock geographic imaginings squarely in the rubrics of white supremacy and settler colonial projects. I
              propose
              that there might be queer ways of disentangling land and labour configurations by paying attention to the everyday negotiations of Filipinxs who are working and making lives in northern BC in relation to Indigenous resistance and
              resurgence.
            </p>
            <p><strong>Bio: </strong>May Farrales is Assistant Professor in the Departments of Geography and Gender, Sexuality &amp; Women's Studies at Simon Fraser University (SFU) on&nbsp;the unceded lands of the Sḵwx̱w&uacute;7mesh
              &Uacute;xwumixw,
              səl̓ilw̓ ətaʔɬ, xʷmə&theta;kʷəy̓əm &amp; kʷikʷəƛ ̓ əm Nations. As an interdisciplinary scholar, her teaching and research are animated by questions of racialization, queer politics, and logics of power fundamental to colonial,
              empire-building, and capitalist projects. Her current research program on the relationships and politics of people of colour in the racial geographies of settler colonialism is grounded in her interest, as a Filipinx scholar, stretching
              Filipinx diaspora studies to be in dialogue with Critical Indigenous Studies, critical race studies, feminist geographies, queer theory, and Black geographies.</p>
          </template>
        </V-accordion>
      </template>

      <hr>

      <p><strong class="presenter">Excel Garay</strong></p>
      <!-- <p>Location: Canada/Philippines</p> -->
      <p>Affiliation: NSCAD University/ Apathy is Boring</p>
      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>
              Tropical Gothic
            </h2>
          </template>
          <template v-slot:content>
            <p>Inspired by Filipino author, Nick Joaquin, the term &ldquo;tropical gothic&rdquo; came from a compilation of fictional short stories titled Tales of the Tropical Gothic. This literary work is a result of a historical moment of
              tumultuous
              social transitions because of colonial forces violating autochthonous cultures. In Joaquin&rsquo;s work, the tropical gothic as a nascent genre resists the imperialist ideology of its European predecessor, infusing Filipinx folklore,
              ways of
              being, and imaginaries into the anglophone literary canon. In the presentation of the group exhibition titled Tropical Gothic, nocturnal aspects of the unknown and solar visions of the Eurocentric canon paradoxically come together to
              shatter
              hegemonic narratives. The exhibition invites a group of artists from tropical diasporas to articulate their unique visions of tropical gothic. By subverting preconceptions of both the tropical and the gothic, this exhibition centers the
              voices and stories of artists who identify their origins with the tropics.</p>
            <p><strong>Bio: </strong>Excel Garay is a Filipina Canadian diasporic settler occupying Mi'kma&rsquo;ki territory in K&rsquo;jipuktuk, Eskikewa&rsquo;kik (Halifax, Nova Scotia). They work as a curator, expanded-media painter, and cultural
              worker. Garay is interested in contradictions that lead subjects, like them, into complicity and complacency. These materially manifest through paintings, ready-made objects, immersive installations and more. Their interest lies in the
              prismatic unseen contradictions and incommensurable situations while focusing on themes of fugitivity, time, and labor. Hauntology and melodrama under a queer necropolitical lens foregrounds their practice.</p>
          </template>
        </V-accordion>
      </template>

      <hr>

      <p><strong class="presenter">Dennis Gupa</strong></p>
      <!-- <p>Location: Canada and Philippines</p> -->
      <p>Affiliation: Department of Theatre and Film, Faculty of Arts, University of Winnipeg</p>
      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>Applied Theatre as Practice of Community Building and Indigenous Ecological Stewardship in the Afterlife of Disaster</h2>
          </template>
          <template v-slot:content>
            <p>In this paper, I aim to tell a story on how I employed my methods of inquiry that deal with climate change, Indigenous ecological knowledge, and applied theatre that resulted in a conceptualization of performance strategies to build a
              dramaturgy of ecological stewardship in island communities constantly negotiating with climate crises in the Philippines. By asking how applied theatre explores agency, relationality, and creativity in the aftermath of a disaster, I
              hope to
              propose a methodological intervention and decolonial collaboration with communities impacted by climate change. The paper will end with a narrative inquiry on the co-creation of community-based-theatre performances that underscore
              transnational solidarity engendered by community members, elders, local government officials, local artists in the Philippines and diasporic Filipinos in Canada to address the existing colonial mode of theorizing theatre and
              post-disaster
              recovery programs deploy in local island community decimated by climate crises.&nbsp;</p>
            <p><strong>Bio:</strong> Dennis is a theatre director and an Assistant Professor in the Department of Theatre, University of Winnipeg. He received his PhD in Applied Theatre from the University of Victoria and his MFA Theatre (Directing)
              from
              the University of British Columbia. He has an MA in Theatre Arts from the University of the Philippines. His intercultural theatre works have been exhibited in North America and Southeast Asia. Dennis is included in The CCP Encyclopedia
              of
              Philippine Arts for his contribution to the theatrical heritage of the Philippines. In 2010, he received a scholarship from the Republic of Indonesia. The Asian Cultural Council awarded him the 2011 director-in-residence program in New
              York
              City. He is the recipient of Vanier Graduate Scholarship, Performance Studies international&rsquo;s Dwight Conquergood Award, the Ada Slaight Drama in Education Award and the National Commission for Culture and the Arts&rsquo; Doctoral
              Award.
            </p>
          </template>
        </V-accordion>
      </template>

      <hr>

      <p><strong class="presenter">PJ Javier</strong></p>
      <!-- <p>Location: Canada</p> -->
      <p>Affiliation: Brock University&nbsp;</p>
      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>
              Belong, but don&rsquo;t belong: Narratives of youths sponsored by former participants of the Live in Caregiver Program
            </h2>
          </template>
          <template v-slot:content>
            <p>This presentation considers the impact of the former Live in Caregiver Program on children left behind as they are depicted in Global Care Chains literature. I interview youth who were sponsored for permanent resident status by former
              participants of the LCP. I use Valerie Francisco Menchavez's concept of multidirectional care to reimagine Western constructs of childhood. I suggest that youth whose childhoods are informed by colonialism, migration, and economic
              uncertainty
              resist normative theorizations of childhood development that assume white families as ideal. I connect the experiences of my participants to unravel critical debates of childhood innocence, including analysis of race, class, and gender
              to
              unravel how some children are not protected by innocence. This process allows childhood experiences wrought under globalization and colonization to start writing themselves into theories of childhood.&nbsp;</p>
            <p><strong>Bio:</strong> PJ is a doctoral student in the Child and Youth Studies program at Brock University under the supervision of Dr. Hannah Dyer. She has an MA in Women's and Gender Studies and a BA in Communication Studies from
              Carleton
              University. Her current research theorizes the impacts of international childcare policies and state endorsed programs. Her work suggests for the inclusion of the experiences of diasporic youth onto global discussions about children's
              rights
              and theories of child development.</p>
          </template>
        </V-accordion>
      </template>

      <hr>

      <p><strong class="presenter">Marissa Largo</strong></p>
      <!-- <p>Location: Canada</p> -->
      <p>Affiliation: York University</p>
      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>
              Applying a Decolonial Diaspora Aesthetic lens to Museum Community Engagement:&nbsp;Faith and Fortune&nbsp;at the Art Gallery of Ontario
            </h2>
          </template>
          <template v-slot:content>
            <p>The Art Gallery of Ontario, the largest art museum in Canada, is mounting its first ever exhibition related to Philippine visual culture entitled&nbsp;Faith and Fortune: Art Across the Global Spanish&nbsp;Empire, opening June 11, 2022.
              This
              exhibition, on loan from the Hispanic Society in New York City, consists of art and artifacts spanning from 1492 to 1898.&nbsp;In the shadow of the&nbsp;500th&nbsp;anniversary of the&nbsp;rise and spread of the Spanish Empire and
              Christianising mission in the Philippines in 2021, this exhibition may be met by diasporic Filipinos with a mix of reverence, ambivalence, and anti-colonial resistance. I speculate on how the application of a&nbsp;decolonial diaspora
              aesthetic&nbsp;(Largo, 2018) to the forward-facing programming around this exhibition may&nbsp;ethically and meaningfully engage with diasporic Filipinos in a way that attends to the multiplicity of understandings, affects, and beliefs
              in
              relation to Spanish colonialism.&nbsp;</p>
            <p><strong>Bio:</strong> Dr. Marissa Largo is an assistant professor of Creative Technologies at York University.&nbsp;Her work focuses on the intersections of community engagement, race, gender and Asian diasporic cultural production.
              Her
              forthcoming book,&nbsp;Unsettling Imaginaries: Filipinx Contemporary Artists in Canada&nbsp;(University of Washington Press)&nbsp;examines the work and oral histories of artists who imagine Filipinx subjectivity beyond colonial logics.
              Largo
              was a recipient of the 2019 Outstanding Dissertation Award from the Research on the Education of Asian and Pacific Americans special interest group of the American Educational Research Association. Her 2021 curatorial
              project&nbsp;Elusive
              Desires:&nbsp;Ness Lee &amp; Florence Yee&nbsp;at the Varley Art Gallery of Markham was awarded a Canada Council for the Arts grant and an&nbsp;Ontario Arts Council Grant for&nbsp;Curatorial Projects: Indigenous and Culturally
              Diverse.&nbsp;Since 2018, Largo has served as the Canada Area Editor of the Journal of Asian Diasporic Visual Cultures and the Americas (ADVA).</p>

          </template>
        </V-accordion>
      </template>

      <hr>

      <p><strong class="presenter">Kara Manso</strong></p>
      <!-- <p>Location: Canada/ Philippines</p> -->
      <p>Affiliation: Caregivers Action Centre</p>
      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>
              Opening Plenary: Care Work in and Beyond the Pandemic
            </h2>
          </template>
          <template v-slot:content>
            <img class="bio" src="~/assets/img/manso.jpeg" alt="Kara Manso">
            <p><strong>Bio:</strong> Kara Manso is a Care Worker, who came to Canada through the Live-in caregiver program.
              After seeing the atrocious conditions in the program, they got involved with the Caregivers
              Action Centre. Manso eventually became the staff organizer of the Caregivers Action Centre,
              where they spent their time building up Care Worker leaders, organizing Know Your Rights
              workshops and advocating at different levels of government.</p>
            <p>Kara also has a personal illustration arts practice. They’ve used it to highlight the experiences
              and resistance of Care Workers in Canada, and have shown at Mayworks Festival, Cue Arts
              and at multiple rallies, demos and direct actions.</p>
            <p>For the last few years, Kara has been working as a Care Worker with people living with
              Alzheimer&#39;s. They were on the long-term care home front lines of the covid-19 pandemic and
              have processed the experience through daily comic vignettes.</p>

          </template>
        </V-accordion>
      </template>

      <hr>



      <p><strong class="presenter">Dani Magsumbol&nbsp;</strong></p>
      <!-- <p>Location:&nbsp;Canada</p> -->
      <p>Affiliation:&nbsp;York University</p>
      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>
              Love and labour: Lessons from the liminality of labour migrants
            </h2>
          </template>
          <template v-slot:content>
            <p>&ldquo;The political economy of emotions, while grounded in the role of the Philippines as a state that brokers its citizens as labourers, approaches the question of labour from the perspective of love and affection. Labour is often
              perceived through time: hourly wages, clocking in and clocking out, the commute to and from work. Within the Filipino labour diaspora, labour is also perceived through affective time: counting the time difference between family members,
              the
              years lost between parting and meeting, the flights counted painstakingly into trips home to make the most out of being with family and kin networks. The life of the Filipino migrant worker is bookended by two imperatives: that of
              leaving for
              employment outside the national borders, and that of return, in its many different modalities. As the world plunged into isolation during COVID19, there were and continue to be many lessons to be drawn from the ways in which Filipino
              labour
              migrants, especially migrant mothers, communicated love across time and space, through cell phone, laptop, and computer screens, and through the remittances that they sent home to the Philippines.</p>
            <p><strong>Bio: </strong>Dani is a doctoral candidate in the Department of Politics at York University.&nbsp;Her research looks at the interconnections between the global care economy and how diasporic Filipinos experience legal
              citizenship and
              affective national membership. She was awarded a Canada Graduate Scholarship, Doctoral in 2021.</p>
          </template>
        </V-accordion>
      </template>

      <hr>

      <p><strong class="presenter">Casey Mecija</strong></p>
      <!-- <p>Location: Canada</p> -->
      <p>Affiliation: York University</p>
      <p><strong></strong></p>
      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>
              Sounding Futures: Queer Sonics and Filipinx Intimacies
            </h2>
          </template>
          <template v-slot:content>
            <p>In this presentation, I suggest that sound offers a methodological framework that can uniquely register modes of collectivity and desire that may otherwise go unrecognized. My theory of queer sound expands on how the sonic might be
              used as a
              conceptual resource for making sense of the affective and psychic lives of diasporic communities, particularly Filipinx. I emphasize how sound is both a material and metaphorical force that can enable us to better understand the
              possibilities
              and limits of diaspora. To do this, my presentation focuses on Filipinx examples of transpacific aesthetic expression, from pop music to Elvis impersonation, as a means to foreground the many ways that marginalized people practice care,
              enliven creativity, and repair from colonial violence, across multiple geographic spaces such as Canada and the Philippines.&nbsp;</p>
            <p><strong>Bio:</strong> Casey Mecija is an Assistant Professor in the Department of Communication Studies and holds a PhD from the University of Toronto. Her current research theorizes sounds made in and beyond Filipinx diaspora to make
              an
              argument about a queer sound that permeates diasporic sensibilities. Her work suggests that media production enables diasporic people to create forms of belonging that defy racialized ascriptions born from racism, colonialism, and their
              gendered dimensions. She is also a musician and filmmaker, whose work has received a number of accolades and has been presented internationally.&nbsp;</p>
          </template>
        </V-accordion>
      </template>

      <hr>

      <p><strong class="presenter">Dr. Ashley Caranto Morford</strong> (she/her)</p>
      <!-- <p>Location: Lenapehoking (so-called Philadelphia, PA, USA)</p> -->
      <p>Affiliation: Assistant Professor of English, Department of Liberal Arts, Pennsylvania Academy of the Fine Arts</p>
      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>Settler of Colour Kinship Work: Refusing Canada with/in Rita Wong and Fred Wah&rsquo;s beholden</h2>
          </template>
          <template v-slot:content>
            <p>How can settler Filipinos be better kin to Indigenous lands and life within so-called Canada? My paper begins to unpack this question through close reading the poem (2018) by Chinese-Canadian writers Rita Wong and Fred Wah. beholden is
              a
              poem of/about the so-called Columbia River, a sacred Indigenous waterway that extends across the colonial boundaries of British Columbia, Washington State, and Oregon (Wong and Wah ii; 142). This poem enables settler Filipinos to
              witness how
              settlers of colour living in Indigenous lands are working to refuse settler conceptualizations of place, and contending with their positionings as uninvited inhabitants in Indigenous lands. In my reading, I engage with White Earth
              Ojibwe
              scholar Jean M. O&rsquo;Brien&rsquo;s concept of &ldquo;firsting&rdquo; &mdash; those acts that portray &ldquo;the colonial regime&rdquo; as &ldquo;the &lsquo;first&rsquo; to bring &lsquo;civilization&rsquo; and authentic history
              to&rdquo;
              this territory (xv) &mdash; and Anishinaabe-M&eacute;tis-Norwegian scholar Melissa K. Nelson&rsquo;s concept of &ldquo;eco-eroticism&rdquo; &mdash; intimate human-nonhuman relations. I believe that beholden strives to un-first colonial
              conceptualizations of place, and to uplift eco-erotic relations with/in Indigenous territories.</p>
            <p><strong>Bio:</strong> Dr. Ashley Caranto Morford, Ph.D., is a Filipina British settler scholar and educator whose work is in relationship with Filipinx/a/o studies, Indigenous studies, anti colonial practices, and digital humanities.
              Her
              work
              focuses on how settler Filipinx/a/os can be better kin to Black and Indigenous communities in so called North America. Ashley is an Assistant Professor in Liberal Arts at the Pennsylvania Academy of the Fine Arts in Lenapehoking
              (so-called
              Philadelphia). | amorford@pobox.pafa.edu</p>
          </template>
        </V-accordion>
      </template>

      <hr>



      <p><strong class="presenter">Martha Ocampo</strong></p>
      <!-- <p>Location: Canada/ Philippines</p> -->
      <p>Affiliation: Caregiver Connection Education and Support Organization (CCESO)</p>
      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>
              Opening Plenary: Care Work in and Beyond the Pandemic
            </h2>
          </template>
          <template v-slot:content>
            <img class="bio" src="~/assets/img/martha.jpeg" alt="Martha Ocampo">
            <p>Martha Ocampo is a founding member and is part of the Advisory of the Caregiver
              Connection Education and Support Organization (CCESO). She has been a long-time
              advocate for the rights of caregivers and domestic workers since the late seventies and was a
              leading member of INTERCEDE. She developed a Leadership and Advocacy Training
              specifically for caregivers and newcomers and, she co-authored “Let’s Talk” a guidebook on
              education about Violence Against Women in the Filipino community. She is a Race, Culture
              and Mental Health consultant with Martha Ocampo and Associates, providing educational and
              training workshops at mental health and addiction agencies, and the general public. She is
              co-editor of a book, Critical Psychiatry and Mental Health published in 2014. Martha is a
              founding member of Across Boundaries: An Ethnoracial Mental Health Centre in Toronto.
              She played a key role in developing the Centre’s Holistic Model of Care within an AntiRacism/Anti-Oppression Framework. She is a founding member of both the Kapisanan for
              Arts and Culture and the Carlos Bulosan Theatre CBT) in Toronto. She is currently the chair
              of the Board of CBT. She is on the Board of the Assaulted Women's Helpline, a member of
              the Advisory Committee at George Brown College Community Worker's Program.</p>

          </template>
        </V-accordion>
      </template>

      <hr>


      <p><strong class="presenter">The Pahinga Collective:</strong></p>
      <p>Dr. Conely de Leon, Jhona Binos, Jann Tracee Ko Din, Joelle Navarro, Mycah Panjaitan, and Mauriene Tolentino</p>
      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>
              Read more
            </h2>
          </template>
          <template v-slot:content>
            <p>We are a small and newly formed collective of Filipina/x/o faculty, graduate students, community organizers, and service
              providers representing migrant, queer, and feminist grassroots organizations in Tkaronto. Our desire to form the Pahinga Collective stemmed from an urgent need to create a space that was by us and for us, a space where we could imagine
              otherwise. To us, pahinga encompasses many things. It means rest as much as it means stillness, ease, pause, reflection, and slowing down. <br /><br />Our intention is to build an emergent community praxis centered on pahinga as a form
              of
              collective care and healing justice. Through digital storytelling we hope to capture our reflections on what it means to: enact a politic of refusal guided by Quechua scholar, Sandy Grande&rsquo;s call to &ldquo;refuse the university
              [as] the
              arm of the settler state&rdquo;[1] building on Mohawk scholar, Audra Simpson&rsquo;s broader work on refusal[2]; embody rest as a form of resistance that pushes back against racial capitalism, white supremacy, and cisheteronormativity,
              guided
              by the work of the Nap Ministry, founded by Tricia Hersey[3] and grounded in Black liberation, womanism, somatics, and Afrofuturism; and to think creatively and capaciously about what pahinga as a form of collective care can contribute
              to
              conversations about collective rest and healing. We ask, how might such a framework sustain us - sustain our community-, movement-, and solidarity building efforts?<br /><br />To sustain ourselves and our work throughout the pandemic,
              we have
              needed many reminders to rest.&nbsp;<em>Magpahinga ka muna</em>&nbsp;(rest for a while).&nbsp;<em>Dahan dahan lang</em>&nbsp;(take it easy, take it slow, or slow down).&nbsp;<em>Pagod na pagod na tayo</em>&nbsp;(we are already so
              tired).
              Importantly, our creative process has involved conversations around safety, trust, accessibility, and community. We share our multimodal approach - our digital kwentuhan, our songs, our poetry, our photographs of loved ones, as well as
              accompanying transcripts, learning community resource list, and collaborative Spotify playlist - as an invitation to further develop our process with you.</p>
          </template>
        </V-accordion>
      </template>


      <hr>


      <p><strong class="presenter">John Paul Catungal</strong></p>
      <!-- <p>Location: Canada</p> -->
      <p>Affiliation: Institute for Gender, Race, Sexuality and Social Justice, University of British Columbia</p>
      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>Community organizing as vernacular critique: Filipinx Canadian youth theorize educational abandonment&nbsp;</h2>
          </template>
          <template v-slot:content>
            <p>Drawing on community based participatory research with the Kababayan Academic Mentorship Program, this paper examines the phenomenon of educational abandonment, which names the institutionally sanctioned narrowing of possible futures
              for
              Filipinx Canadian youth through the racial organization of schooling. It does so with a focus on the education-focused organizing work of Filipinx Canadian youth in so-called Vancouver. As powerful, yet underappreciated, forms of
              vernacular
              critique, stories shared by Filipinx Canadian youth about their schooling experiences and their efforts to create culturally appropriate, peer-led supports testify to the consignment of Filipinx Canadian youth to futures of racially
              narrowed
              socio-economic opportunity. Quite importantly, their vernacular critique locates educational abandonment within a larger ecology of institutions that produce unequal racialized futures, among them education, immigration, labour,
              policing and
              the media. In the face of this institutional ecology of abandonment, organizing by Filipinx Canadian youth, along with their efforts to publicly share their stories, must thus be understood as a powerful form of agentive&nbsp;refusal.
            </p>
            <p><strong>Bio: </strong>Dr. JP Catungal is Assistant Professor in the Institute for Gender, Race, Sexuality and Social Justice and Interim Director of the Asian Canadian and Asian Migration Studies Program at the University of British
              Columbia. A queer, first-generation Filipinx Canadian settler living in unceded Coast Salish territories, JP is an interdisciplinary scholar trained in the nexus of critical human geography and intersectional feminist theorizing. His
              research, teaching and public facing work concern the community organizing and cultural production practices of migrant, racialized and LGBTQ+ communities, with particular interests in sexual health, education and social services. He
              approaches his work indebted to and in conversation with Filipinx and Asian diaspora studies and queer and trans of colour theorizing. JP was co-editor of the Filipinos in Canada: Disturbing Invisibility (2012, University of Toronto
              Press)
              and has served on the editorial collective of ACME: International Journal of Critical Geographies since August 2017.</p>
          </template>
        </V-accordion>
      </template>

      <p><strong class="presenter">Mel Racho</strong></p>
      <p>Affiliation:&nbsp;York University/Toronto Metropolitan University</p>
      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>Cultural Production
            </h2>
          </template>
          <template v-slot:content>
            <p><strong>Bio: </strong>Bio: Mel Racho (he/him) is a queer, trans POC Internet researcher enrolled in X and York Universities’ jointly administered Communication and Culture PhD program. His research interests include the leaky and data-insecure infrastructures of the Internet, data feminism and the successive ‘versions’ of the WWW. </p>
          </template>
        </V-accordion>
      </template>


      <hr>

      <p><strong class="presenter">Kim Joshua Salcedo</strong></p>
      <p>Affiliation:&nbsp;Alberta Bible College</p>
      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>The Rising Filipino Ethnic Churches in Canada

            </h2>
          </template>
          <template v-slot:content>
            <p>Despite the already many established different churches in Canada, the rising number of Filipino congregations is making waves in the country. Overseas Filipino Workers (OFW) and families obtaining permanent residency in the country
              are
              looking for opportunities for employment, education, and a future for their children. But religion and faith play important roles in the immigrants&rsquo; move. Almost all Canadians of Filipino origin belong to a Christian faith and
              maintain
              more than just sentimental cultural ties to life back home. Is maintaining their own religious churches a necessity for Filipinos in keeping their own belongingness and self-identity as Filipinos to a new country? Is having an
              ethnocentric
              church aids the transition to a foreign place? Does the Filipino diaspora play an important role in God&rsquo;s agenda to impact the world for the Gospel? </p>
            <p><strong>Bio: </strong>Kim is a believer, husband of Jahaziel, and father to their dogs Ogie and Bear. He is passionate about reaching out to the next generation of leaders, and those who have immigrated to Canada. He believes in
              planting
              seeds in people. God has a calling for every tribe, nation, and language to be equipped for effective service and witness for Christ, and he is excited to be a part of connecting with people across Canada and around the globe. In his
              free
              time, he loves to minister to people as he plays and coaches basketball games. He practices being a teacher, coach, and pastor in his roles as an ABC Enrollment Coordinator and volunteer to Shekinah Victory Church. He is currently
              working on
              finishing up his master's studies in Theological Studies at Wycliffe College.</p>
          </template>
        </V-accordion>
      </template>

      <hr>
      <p><strong class="presenter">Ethel Tungohan</strong></p>
      <!-- <p>Location:&nbsp;Canada </p> -->
      <p>Affiliation Institution/Organization:&nbsp;York University&nbsp;</p>
      <template>
        <V-accordion>
          <template v-slot:title>
            <h2>
              Endlessly waiting, always hoping: Filipinx migrant workers and Canadian immigration policies
            </h2>
          </template>
          <template v-slot:content>
            <p>In this presentation, I will assess how Canadian immigration policies, particularly during the pandemic, has presented numerous challenges for Filipinx migrant workers. Not only does the pandemic increase workplace vulnerabilities,
              placing
              Filipinx migrant workers in essential workplaces at higher risks of getting exposed to COVID19, it has also negatively affected Filipinx migrant workers&rsquo; security of status in Canada by making it harder for them to meet the
              requirements
              for Canadian citizenship.&nbsp;All of these challenges, combined, lead Filipinx migrant workers to face lengthier time frames for realizing their ambitions which may include reunifying with their families in Canada, transitioning into
              another
              profession and paying their debts (both financial and debts of obligation) to community members who supported them. Using Melanie Griffith&rsquo;s theory on temporality and immigration as the basis for my analysis, I reflect on how the
              temporal uncertainties facing Filipinx migrant workers affect their everyday experiences of belonging, including impeding their mental and emotional health, while also, paradoxically, serves as a catalyst for activist endeavours.</p>
            <p><strong>Bio:</strong> Ethel Tungohan is an Associate Professor of Politics and a Canada Research Chair (Tier 2) in Canadian Migration Policy, Impacts, and Activism. Her work uses socially engaged research methods to examine the effects
              of
              Canadian immigration policies on communities of migrant workers with a specific emphasis on Filipinx migrant workers and their families. Her forthcoming book manuscript include Containing Diversity: Canadian Immigration Policy and
              Politics in
              the 21st&nbsp;Century, coauthored with Yasmeen Abu-Laban and Christina Gabriel (University of Toronto Press).</p>
          </template>
        </V-accordion>
      </template>

      <hr>






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
.bio {
    width: 50%;
    object-fit: contain;
    float: left;
    padding-right: 1em;
}
</style>
