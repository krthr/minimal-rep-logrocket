<template>
  <div>
    <FormulateInput
      type="file"
      name="file"
      label="Select your documents to upload"
      validation="mime:image/jpeg,image/png"
      :uploader="uploadFile"
    />
  </div>
</template>

<script>
export default {
  name: "IndexPage",

  methods: {
    uploadFile(file) {
      console.log("uploading the file", { file });
    },
  },
};
</script>

<style>
@import "https://cdn.jsdelivr.net/npm/@braid/vue-formulate@2.5.3/dist/snow.min.css";
</style>
