<template>
  <div id="app">
    <quill-editor v-model="texto" :options="editorOption"></quill-editor>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {},
  data() {
    return {
      texto: "hola",
      editorOption: {
        placeholder: "Inserte el texto aquí",
        modules: {
          //imageDrop: true,
          imagePaste: true,
          toolbar: [
            ["bold", "italic", "underline", "strike"],
            ["blockquote", "code-block"],
            [{ header: 1 }, { header: 2 }],
            [{ list: "ordered" }, { list: "bullet" }],
            [{ script: "sub" }, { script: "super" }],
            [{ indent: "-1" }, { indent: "+1" }],
            [{ direction: "rtl" }],
            [{ size: ["small", false, "large", "huge"] }],
            [{ header: [1, 2, 3, 4, 5, 6, false] }],
            [{ font: [] }],
            [{ color: [] }, { background: [] }],
            [{ align: [] }],
            ["clean"],
            ["link", "image", "video"],
            ["template-partediario"]
          ]
        }
      }
    };
  }
};
</script>

<style></style>
