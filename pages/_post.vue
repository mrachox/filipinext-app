<template>
<div>
  <!-- <h1>Continent: {{ continent }}</h1> -->
  <!-- <h2>Page: {{ page }}</h2> -->
  <p>Path: {{ $route.path }}</p>
  <!-- <NuxtLink to="/">Back to Mountains</NuxtLink> -->
</div>
</template>
<script>
export default {
  async asyncData({ params, redirect }) {
    const pages = await fetch(
      '/api/pages.json'
    ).then((res) => res.json())

    const pages_data = []
    pages_data.push([pages]);

    console.log(pages_data[0][0])
    console.log(Array.isArray(pages_data[0]), pages_data[0])

    const filteredPage = pages_data[0].find(
      (element) => element.slug === params.post
      // function(el) {
      //   el.url === params.page
      // }
    )

    // if (filteredPage) {
    //   return {
    //     post: filteredPage.title
    //   }
    // }
    // else {
    //   redirect('/')
    // }
  }

}

// export default {
//   async asyncData({ params, redirect }) {
//     const mountains = await fetch(
//       'https://api.nuxtjs.dev/mountains'
//     ).then((res) => res.json())
//
//     const filteredMountain = mountains.find(
//       (el) =>
//         // el.continent.toLowerCase() === params.continent &&
//         el.slug === params.mountain
//     )
//     if (filteredMountain) {
//       return {
//         // continent: filteredMountain.continent,
//         mountain: filteredMountain.title
//       }
//     }
//     // else {
//     //   redirect('/')
//     // }
//   }
// }


</script>
