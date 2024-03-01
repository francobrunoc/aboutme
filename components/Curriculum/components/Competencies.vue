<template>
  <div>
    <h2 class="section-heading">Basic competencies</h2>
    <div class="competencies-container">
      <div
        v-for="competency in competencies"
        class="competency notranslate"
        :key="competency.id"
      >
        {{ competency.name }}
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Competencies",
  data() {
    return {
      competencies: [
        { id: 1, name: "HTML5" },
        { id: 2, name: "CSS3" },
        { id: 3, name: "JavaScript" },
        { id: 5, name: "TypeScript" },
        { id: 4, name: "Linux" },
        { id: 16, name: "Docker" },
        { id: 17, name: "Kubernetes" },
        { id: 18, name: "Git" },
        { id: 19, name: "Jest" },
        { id: 20, name: "Cypress" },
        { id: 21, name: "Jenkins" },
        { id: 22, name: "GitLab" },
      ],
    };
  },
};
</script>

<style>
.section-heading {
  padding-top: 30pt;
  text-indent: 0pt;
  text-align: left;
}

.competencies-container {
  display: flex;
  width: 100%;
  flex-direction: row;
  flex-wrap: wrap;
}

.competency {
  font-size: 15px;
  padding: 5px 10px;
  margin: 5px;
  border-radius: 15px;
  background-color: #f0f0f0;
  font-family: "Trebuchet MS", sans-serif;
}
</style>
