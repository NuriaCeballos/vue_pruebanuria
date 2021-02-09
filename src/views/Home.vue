<template>
  <div class="home">
     <Personaje fuerza="10"/>
   </div>
</template>

<script>
// @ is an alias to /src
import Personaje from '@/components/Personaje.vue'

export default {
  name: 'home',
  components: {
    Personaje
  }
}
</script>

