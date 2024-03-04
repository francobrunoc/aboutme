<template>
  <div id="main">
    <Title />
    <Contact />
    <Profile />
    <Education />
    <Languages />
    <Skills />
    <PersonalProjects />
    <ProfessionalExperience />
    <Competencies />
  </div>
</template>

<script>
import Title from "./components/Title.vue";
import Contact from "./components/Contact.vue";
import Profile from "./components/Profile.vue";
import Education from "./components/Education.vue";
import Languages from "./components/Languages.vue";
import PersonalProjects from "./components/PersonalProjects.vue";
import ProfessionalExperience from "./components/Experience.vue";
import Competencies from "./components/Competencies.vue";
import Skills from "./components/Skills.vue";
export default {
  name: "NuxtCV",
  components: {
    Title,
    Contact,
    Profile,
    Education,
    Languages,
    Skills,
    PersonalProjects,
    ProfessionalExperience,
    Competencies,
  },
};
</script>

<style>
@import "../../styles/Curriculum.css";
</style>
