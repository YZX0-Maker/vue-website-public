<template>
    <div class="projects">
      <Project/>
      <Footer/>
    </div>
  </template>
  
  <script>
  // @ is an alias to /src
  import Project from '@/components/projects/fragment_1.vue'
  import Footer from '@/components/footer.vue'
  
  export default {
    name: 'Projects',
    components: {
      Project, Footer
    }
  }
  </script>
  