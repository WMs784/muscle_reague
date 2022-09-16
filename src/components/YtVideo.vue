<template>
  <div class="field">
    <v-container fluid>
      <v-row justify="center">
        <iframe
      width="100%"
      height="600"
      :src="`https://www.youtube.com/embed/${videoId}`"
      title="YouTube video player"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
      allowfullscreen
    ></iframe>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  props: {
    width: {
      type: Number,
      default: 100,
    },
    height: {
      type: Number,
      default: 720,
    },
    videoId: {
      type: String,
      required: true,
    },
  },
};
</script>