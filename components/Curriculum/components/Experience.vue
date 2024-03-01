<template>
  <div class="resume-container">
    <h2 class="section-heading">Professional experience</h2>
    <div v-for="(job, index) in jobs" :key="index">
      <h3 class="job-title">{{ job.title }}</h3>
      <p class="job-details">{{ job.date }}</p>
      <p class="job-details">{{ job.location }}</p>
      <p class="job-details">{{ job.description }}</p>
      <ul class="tech-list">
        <li v-for="(tech, techIndex) in job.techList" :key="techIndex">
          <p class="notranslate tech-item">- {{ tech }}</p>
        </li>
      </ul>
      <div class="section-spacing"></div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      jobs: [
        {
          title:
            "Fullstack Developer na Cia Latinoamericana de Medicamentos (CLAMED)",
          date: "out 2021 Joinville - Santa Catarina / BR",
          location:
            "Innovation analyst and software engineer. Exploring the most modern ways to do universal and portable software using JavaScript and cloud resources.",
          description: "out 2021 Joinville - Santa Catarina / BR",
          techList: [
            "Vue 3",
            "Next JS",
            "React Native",
            "Azure and AWS Cloud",
            "TypeScript",
            "Serverless",
            "Node JS",
            "Microsoft Power Automate",
          ],
        },
        {
          title: "Software Engineer na Prime Serviços Médicos Ltda",
          date: "jun 2021 - out 2021",
          location: "Porto Alegre - Rio Grande do Sul / BR",
          description:
            "Full stack developer exploring magnificence with JavaScript and cloud resources.",
          techList: [
            "Vue 3",
            "Next JS",
            "React JS",
            "Azure and AWS Cloud",
            "Serverless",
            "Kotlin",
          ],
        },
        {
          title: "Frontend Software Developer na Ommed",
          date: "mar 2021 - jun 2021",
          location: "Florianópolis - Santa Catarina / BR",
          description: "Frontend leader developer:",
          techList: ["Vue 3", "gRPC", "PrimeVUE", "Sass"],
        },
        {
          title: "Fullstack Developer Self employed",
          date: "mar 2020 - mar 2021 Florianópolis - Santa Catarina / BR",
          description:
            "Development and maintenance of web applications based on JavaScript, Node JS, and cloud server (AWS and Google).",
          techList: [
            "Nuxt.js",
            "Vue.js",
            "AWS Cloud",
            "Google Cloud",
            "Node.js",
            "R",
          ],
        },
        {
          title: "Software and hardware engineer Self employed",
          date: "mar 2016 - mar 2020 Florianópolis - Santa Catarina / BR",
          description:
            "Independent work developing and maintaining static and dynamic web systems for multiple clients. Development and research of new electronic products for home automation combining hardware components with software developed for the web (IoT).",
          techList: [
            "React JS",
            "Angular 2+",
            "MySQL",
            "Vue 2",
            "Arduino",
            "Raspberry Pi",
          ],
        },
        {
          title: "Software Developer no Grupo Dimed",
          date: "aug 2015 - nov 2015",
          location: "Eldorado do Sul - Rio Grande do Sul / BR",
          description:
            "Development and maintenance of web technological resources of the Dimed group (Dimed distributor, Panvel pharmacies and Lifar laboratories), using web and open source languages. Main technologies absorbed and improved:",
          techList: [
            "Java",
            "JSF",
            "Javascript",
            "Maven",
            "Gradle",
            "Jetty",
            "JBoss",
            "REST",
          ],
        },
        {
          title: "Java Programmer na Safetech Informática",
          date: "oct 2011 - aug 2015",
          location: "Sapiranga - Rio Grande do Sul / BR",
          description:
            "Professional experience in developing web applications based on Java and Groovy technologies. Improvement and productivity through frameworks like Grails, Struts and Spring. Development of customized commercial applications according to the company's area of activity.",
        },
        {
          title: "IT Analyst na Johann Alimentos",
          date: "jan 2008 - oct 2011",
          location: "Estância Velha - Rio Grande do Sul / BR",
          description:
            "Worked as an IT assistant, becoming a support analyst with an emphasis on in systems development and maintenance, technical support, analysis and software approval and responsible for the entire IT infrastructure of the company.",
        },
        {
          title: "Electronics Technician na ChipByte Informática",
          date: "jan 2006 - jan 2008",
          location: "Novo Hamburgo - Rio Grande do Sul / BR",
          description: "Performed maintenance and tests on computer equipment.",
        },
        {
          title: "Electronics Technician na New Tech Informática",
          date: "jan 2005 - jan 2006",
          description:
            "Performed maintenance and tests on computer equipment. (Internship)",
        },
        {
          title:
            "Electronics Technician na Himaco Hidraulicos E Maquinas Ind. E Com Ltda",
          date: "jan 2005 - jun 2005",
          location: "Novo Hamburgo - Rio Grande do Sul / BR",
          description:
            "Assembly and composition of electronic control boards for industrial machines.",
        },
      ],
    };
  },
};
</script>

<style>
.resume-container {
  font-family: Arial, sans-serif;
}

.job-title {
  text-indent: 0pt;
  line-height: 109%;
  text-align: left;
}

.job-details {
  padding-top: 3pt;
  text-indent: 0pt;
  line-height: 138%;
  text-align: left;
}

.tech-list {
  padding-left: 14pt;
  text-indent: -5pt;
  text-align: left;
}

.tech-item {
  margin: 3pt 0;
}
</style>
