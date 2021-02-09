<template>
  <div class="about" >
    <h3> Los he visto peores</h3>
    <Personaje fuerza="5"/>
  </div>
</template>
<script>
// @ is an alias to /src
import Personaje from '@/components/Personaje.vue'


export default {
  name: 'About',
  components: {
    Personaje
    
  }
}
</script>
