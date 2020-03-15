<template>
  <div>
    <h1>Movie</h1>
    <PfMovie
      v-for="movie in movies"
      :key="movie.title"
      :title="movie.title"
      :movieUrl="movie.movieUrl"
    />
  </div>
</template>

<script>
import PfMovie from "@/components/Molecules/PfMovie.vue";

export default {
  data: function() {
    return {
      movies: [
        {
          title: "Breakdown of sanity - Hero (Guitar & Bass cover)",
          movieUrl: "https://www.youtube.com/embed/vOqz0o8TUjc"
        },
        {
          title: "Utsu-P - THE DYING MESSAGE / PTSD ver. (Guitar cover)",
          movieUrl: "https://www.youtube.com/embed/PePeDQwsMrc"
        }
      ]
    };
  },

  components: {
    PfMovie
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
