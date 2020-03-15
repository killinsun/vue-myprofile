<template>
  <section class="youtube-movie">
    <h2 class="movie-title">
      <span wovn-ignore>{{ title }}</span>
    </h2>
    <div class="movie">
      <iframe
        width="560"
        height="315"
        v-bind:src="movieUrl"
        frameborder="0"
        allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen
      ></iframe>
    </div>
    <div class="likes-buttons"></div>
  </section>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: "no title",
      required: true
    },
    movieUrl: {
      type: String,
      default: "https://www.youtube.com/embed/vOqz0o8TUjc",
      required: true
    }
  }
};
</script>

<style scoped>
section.youtube-movie {
  padding-top: 3vh;
}

div.movie {
  padding-top: 0vh;
}
</style>
