<template>
  <div class="rs-recent-uploads">
    <RsCard title="Recent uploads" icon="mdi-folder-multiple-image">
      <v-row class="rs-recent-uploads-container">
        <v-col cols="3" v-for="image in images" :key="image.id">
          <v-img :src="image.url"></v-img>
        </v-col>
      </v-row>
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
          url: 'https://picsum.photos/id/0/367/267',
        },
        {
          id: 2,
          url: 'https://picsum.photos/id/10/367/267',
        },
        {
          id: 3,
          url: 'https://picsum.photos/id/100/367/267',
        },
        {
          id: 4,
          url: 'https://picsum.photos/id/1001/367/267',
        },
        {
          id: 5,
          url: 'https://picsum.photos/id/1002/367/267',
        },
        {
          id: 6,
          url: 'https://picsum.photos/id/1003/367/267',
        },
        {
          id: 7,
          url: 'https://picsum.photos/id/1004/367/267',
        },
        {
          id: 8,
          url: 'https://i.picsum.photos/id/1005/5760/3840.jpg?hmac=2acSJCOwz9q_dKtDZdSB-OIK1HUcwBeXco_RMMTUgfY',
        },
        {
          id: 9,
          url: 'https://picsum.photos/id/1006/367/267',
        },
        {
          id: 10,
          url: 'https://picsum.photos/id/1008/367/267',
        },
        {
          id: 11,
          url: 'https://i.picsum.photos/id/101/2621/1747.jpg?hmac=cu15YGotS0gIYdBbR1he5NtBLZAAY6aIY5AbORRAngs',
        },
        {
          id: 12,
          url: 'https://picsum.photos/id/1010/367/267',
        },
      ],
    }
  },
}
</script>
