<template>
  <main>
    <v-google-translate @select="googleTranslateSelectedHandler" />
    <Curriculum />
  </main>
</template>

<script>
import Vue from "vue";
import vGoogleTranslate from "v-google-translate";
import languages from "assets/languages";
import Curriculum from "../components/Curriculum.vue";

Vue.use(vGoogleTranslate);

export default {
  name: "IndexPage",
  components: { Curriculum },
  data() {
    return {
      languages,
    };
  },
  methods: {
    googleTranslateSelectedHandler(language) {
      const { code, name, cname, ename } = language;
      // todo ...
    },
  },
};
</script>
