<template>
  <div class="rs-image-details">
    <RsCard :title="title" remove>
      <div class="rs-image-details-container">
        <v-img src="https://picsum.photos/536/354" height="400px" />
        <div class="rs-image-details-container-description">
          <p class="headline font-weight-black">{{ title }}</p>
          <p>{{ description }}</p>
        </div>
        <div class="rs-image-details-container-icons d-flex">
          <div class="rs-image-details-container-start d-flex justify-start">
            <v-btn color="success"
              ><v-icon class="mx-2">mdi-thumb-up</v-icon>Like</v-btn
            >
            <div class="mx-12">
              <v-icon class="d-flex justify-center">mdi-cards-heart</v-icon>
              <p>Likes 12</p>
            </div>
            <div class="mx-12">
              <v-icon class="d-flex justify-center">mdi-eye-settings</v-icon>
              <p>Views 4</p>
            </div>
          </div>
          <v-spacer></v-spacer>
          <div class="rs-image-details-container-end">
            <p>Date</p>
          </div>
        </div>
      </div>
    </RsCard>
  </div>
</template>

<script>
export default {
  data() {
    return {
      title: 'Image title',
      description:
        'Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries',
    }
  },
}
</script>
