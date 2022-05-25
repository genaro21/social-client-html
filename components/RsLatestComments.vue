<template>
  <div class="rs-lastest-comments">
    <RsCard title="Lastest comments" icon="mdi-comment">
      <RsCommentItem
        v-for="comment in comments"
        :key="comment.id"
        :image="comment.image"
        :email="comment.email"
        :comment="comment.comment"
      />
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
          image:
            'https://comohacerunapagina.es/wp-content/uploads/2018/04/WordPress-insertar-imagen-url.png',
          email: 'pepe1@gmail.com',
          comment: 'comentario1',
        },
        {
          id: 2,
          image: 'https://picsum.photos/536/354',
          email: 'pepe2@gmail.com',
          comment: 'comentario2',
        },
        {
          id: 3,
          image: 'https://picsum.photos/id/237/536/354',
          email: 'pepe3@gmail.com',
          comment: 'comentario3',
        },
        {
          id: 4,
          image: 'https://picsum.photos/id/870/536/354?grayscale&blur=2',
          email: 'pepe4@gmail.com',
          comment: 'comentario4',
        },
      ],
    }
  },
}
</script>
