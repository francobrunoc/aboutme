<template>
  <main>
    <button
      class="fixed top- 0 right-0 p-2 m-2 bg-white rounded-full shadow-lg"
      @click="showtranslator()"
    >
      @
    </button>
    <div ref="googleTranslate" style="visibility: hidden">
      <v-google-translate />
    </div>
    <Curriculum />
  </main>
</template>

<script>
import Vue from "vue";
import vGoogleTranslate from "v-google-translate";
import languages from "assets/languages";
import Curriculum from "../components/Curriculum";

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
    showtranslator() {
      if (this.$refs.googleTranslate.style.visibility === "visible") {
        this.$refs.googleTranslate.style.visibility = "hidden";
        return;
      }
      this.$refs.googleTranslate.style.visibility = "visible";
    },
  },
};
</script>
