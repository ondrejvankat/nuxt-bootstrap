<template>
  <main>

    <section class="py-5 text-center container">
      <div class="row py-lg-5">
        <div class="col-lg-6 col-md-8 mx-auto">
          <h1 class="fw-light">Youtube videa</h1>
        </div>
      </div>
    </section>

    <div class="album py-5 bg-light">
      <div class="container">

        <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 g-3">
        <youtube-card
          v-for = "(link, index) of links"
          :key = "(index + 2)"
          :link = "link"
          :link-to-image = linksToImage[index]
        />
        </div>
      </div>
    </div>

  </main>
</template>

<script>
import YoutubeCard from "~/components/MainPart/YoutubeCard"
export default {
  components: {
    YoutubeCard
  },
  data () {
    return {
      links: [
        'https://www.youtube.com/watch?v=E1koDpTt9ro',
        'https://www.youtube.com/watch?v=60ItHLz5WEA',
        'https://www.youtube.com/watch?v=kXYiU_JCYtU'
      ],
      linksToImage: [
        'https://img.youtube.com/vi/E1koDpTt9ro/0.jpg',
        'https://img.youtube.com/vi/60ItHLz5WEA/0.jpg',
        'https://img.youtube.com/vi/kXYiU_JCYtU/0.jpg'
      ]
    }
  }

}
</script>
