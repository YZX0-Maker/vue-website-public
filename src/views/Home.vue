<template>
  <div class="home">
    <HelloWorld/>
    <Footer/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/index/top_header.vue'
import Footer from '@/components/footer.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld, Footer
  }
}
</script>
