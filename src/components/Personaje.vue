<template>
 <div class="personaje">
     <h1> Dark Vader no es tan malo</h1>
 <img alt="Vue logo" src="../assets/dark.jpg">
 <p>Fuerza Actual: {{fuerzaActual}}</p>
 <button @click="cabrear">Cabrear a Dark Vader</button>
 </div>
</template>

<script>
import {ref} from 'vue'

export default {
    name:"Personaje",
    props:{
        fuerza:{
            type:Number,
            default:0,
            required:true
        }
    },
    setup(props){
    let fuerzaActual=ref(props.fuerza)
    const cabrear=()=>{
        fuerzaActual.value++
    }
    return{
        fuerzaActual,
        cabrear
    }
    } 
}
    
</script>

<style lang="scss" scoped>
.personaje{
  img{
    max-height: 200px;
  }
}
</style>