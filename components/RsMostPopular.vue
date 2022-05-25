<template>
  <div class="rs-most-popular">
    <RsCard title="Most Popular" icon="mdi-camera-image">
      <div class="rs-images-container">
        <v-row>
          <v-col
            cols="6"
            v-for="image in images"
            :key="image.id"
            class="rs-images-container-item"
          >
            <v-img :src="image.url"></v-img>
          </v-col>
        </v-row>
      </div>
    </RsCard>
  </div>
</template>

<script>
export default {
  data() {
    return {
      images: [
        {
          id: 1,
          url: 'https://comohacerunapagina.es/wp-content/uploads/2018/04/WordPress-insertar-imagen-url.png',
        },
        {
          id: 2,
          url: 'https://picsum.photos/536/354',
        },
        {
          id: 3,
          url: 'https://picsum.photos/id/237/536/354',
        },
        {
          id: 4,
          url: 'https://picsum.photos/id/870/536/354?grayscale&blur=2',
        },
      ],
    }
  },
}
</script>
