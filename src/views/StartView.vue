<script setup lang="ts">
</script>

<template>
  <main>
    <div>

      <div></div>
      <div id="comment">
        <p class="comment"> // Everything not saved will be lost... </p>
      </div>
      <div id="terminal-line" style="display: flex;">
        <p class="host">guilherme@moog:~$</p>
        <input class="search" type="text" v-model="terminal" name="" id="" @keyup.enter="">
      </div>

    </div>
  </main>
</template>


<script>
  import { onMounted, ref } from 'vue';


  
  const terminal = ref()
  

  export default {
    components: {
     
    },
    data() {
      return {
        terminal
      };
    },
    watch: {
      banco(newValue) {
      }
    },
      
  }
</script>

<style>

  

</style>