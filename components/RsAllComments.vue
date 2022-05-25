<template>
  <div class="rs-all-comments">
    <RsCard :header="false">
      <div class="rs-all-comments-container">
        <v-row v-for="comment in comments" :key="comment.id">
          <v-col class="d-flex justify-center" cols="4">
            <v-avatar size="100">
              <v-img :src="comment.avatar" />
            </v-avatar>
          </v-col>
          <v-col cols="8">
            <p class="font-weight-black">{{ comment.title }}</p>
            <p>{{ comment.comment }}</p>
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
      comments: [
        {
          id: 1,
          email: 'pepe1@gmail.com',
          title: 'Title 1',
          avatar: 'https://picsum.photos/id/1060/536/354?blur=2',
          comment: 'Comentario 1',
        },
        {
          id: 2,
          email: 'pepe2@gmail.com',
          title: 'Title 2',
          avatar: 'https://picsum.photos/id/1084/536/354?grayscale',
          comment: 'Comentario 2',
        },
        {
          id: 3,
          email: 'pepe3@gmail.com',
          title: 'Title 3',
          avatar: 'https://picsum.photos/seed/picsum/536/354',
          comment: 'Comentario 3',
        },
      ],
    }
  },
}
</script>
