<template>
  <div class="rs-upload">
    <RsCard title="Upload" icon="mdi-cloud-upload">
      <div class="rs-upload-container">
        <v-form>
          <v-file-input
            prepend-icon=""
            outlined
            placeholder="file"
          ></v-file-input>
          <v-text-field
            outlined
            name="title"
            placeholder="Title"
          ></v-text-field>
          <v-textarea
            outlined
            name="description"
            placeholder="Description"
          ></v-textarea>
          <div class="rs-btn-container d-flex justify-end">
            <v-btn depressed color="success" @click="OnClick"> Submit </v-btn>
          </div>
        </v-form>
      </div>
    </RsCard>
  </div>
</template>

<script>
export default {
  methods: {
    OnClick() {
      console.log('Hola Mundo')
    },
  },
}
</script>
